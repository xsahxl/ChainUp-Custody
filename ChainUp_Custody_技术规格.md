# ChainUp Custody 技术规格文档

## 目录

1. [技术架构概述](#技术架构概述)
2. [MPC技术详解](#mpc技术详解)
3. [API集成规范](#api集成规范)
4. [安全技术标准](#安全技术标准)
5. [集成指南](#集成指南)

---

## 技术架构概述

### 系统架构

ChainUp Custody采用分布式架构设计，确保高可用性和安全性：

```
┌─────────────────────────────────────────────────────────────┐
│                    ChainUp Custody 平台                      │
├─────────────────────────────────────────────────────────────┤
│  Web界面  │  移动端APP  │  API服务  │  SDK工具包  │  Co-Signer │
├─────────────────────────────────────────────────────────────┤
│                    MPC核心引擎                               │
├─────────────────────────────────────────────────────────────┤
│   私钥分片1   │   私钥分片2   │   私钥分片3   │   TSS签名    │
│   (本地)     │   (亚马逊云)   │   (微软云)    │   (3-3配置)  │
├─────────────────────────────────────────────────────────────┤
│                  区块链网络层                                │
│  Bitcoin │ Ethereum │ BSC │ Polygon │ ... (200+主链)        │
└─────────────────────────────────────────────────────────────┘
```

### 核心技术栈

- **MPC技术**：Secure Multi-Party Computation
- **TSS技术**：Threshold Signature Scheme
- **加密算法**：ECDSA, EdDSA, RSA
- **云服务**：AWS, Microsoft Azure
- **区块链支持**：200+主链，1000+代币

---

## MPC技术详解

### MPC-TSS技术原理

#### 什么是MPC？
多方安全计算（MPC）是一种密码学技术，允许多个参与方在不泄露各自私有输入的情况下，共同计算某个函数。

#### TSS门限签名方案
- **3-3配置**：需要3个私钥分片全部参与签名
- **分布式存储**：私钥分片分别存储在不同的安全环境中
- **无单点故障**：任何单个分片丢失都不会影响资产安全

#### 技术优势

| 传统多签 | MPC-TSS |
|---------|---------|
| 链上实现 | 链下实现 |
| 地址格式特殊 | 地址格式标准 |
| 交易费用较高 | 交易费用标准 |
| 支持链有限 | 支持所有链 |

### 私钥生成与管理

```javascript
// 私钥生成流程示例
const generateMPCKey = async () => {
  // 1. 生成随机种子
  const seed = crypto.randomBytes(32);
  
  // 2. 分布式密钥生成
  const keyShares = await mpc.generateKeyShares(seed, {
    threshold: 3,
    totalShares: 3
  });
  
  // 3. 分发密钥分片
  const distribution = {
    local: keyShares[0],
    aws: keyShares[1],
    azure: keyShares[2]
  };
  
  return distribution;
};
```

---

## API集成规范

### API架构设计

#### RESTful API设计原则
- **统一的URL结构**：`/api/v1/resource`
- **标准HTTP方法**：GET, POST, PUT, DELETE
- **JSON数据格式**：请求和响应均使用JSON
- **状态码规范**：遵循HTTP状态码标准

#### 认证与授权

```javascript
// API认证示例
const headers = {
  'Authorization': 'Bearer ' + accessToken,
  'Content-Type': 'application/json',
  'X-API-Key': apiKey,
  'X-Signature': signature,
  'X-Timestamp': timestamp
};
```

### 主要API端点

#### 钱包管理
```javascript
// 创建钱包
POST /api/v1/wallets
{
  "name": "企业钱包",
  "type": "MPC",
  "chains": ["BTC", "ETH", "BSC"]
}

// 获取钱包列表
GET /api/v1/wallets?page=1&limit=20

// 获取钱包详情
GET /api/v1/wallets/{walletId}
```

#### 交易管理
```javascript
// 创建交易
POST /api/v1/transactions
{
  "fromAddress": "0x123...",
  "toAddress": "0x456...",
  "amount": "1000000000000000000",
  "chain": "ETH",
  "token": "USDT"
}

// 查询交易状态
GET /api/v1/transactions/{transactionId}

// 获取交易历史
GET /api/v1/transactions?wallet={walletId}&limit=50
```

#### 地址管理
```javascript
// 生成新地址
POST /api/v1/addresses
{
  "walletId": "wallet123",
  "chain": "BTC",
  "label": "收款地址1"
}

// 获取地址列表
GET /api/v1/addresses?wallet={walletId}&chain={chain}
```

### SDK集成示例

#### JavaScript SDK
```javascript
import { ChainUpCustody } from '@chainup/custody-sdk';

const custody = new ChainUpCustody({
  apiKey: 'your-api-key',
  secretKey: 'your-secret-key',
  baseUrl: 'https://api.custody.chainup.com'
});

// 创建钱包
const wallet = await custody.createWallet({
  name: 'My Wallet',
  type: 'MPC'
});

// 发送交易
const transaction = await custody.createTransaction({
  from: wallet.address,
  to: '0x123...',
  amount: '1.5',
  chain: 'ETH'
});
```

#### Python SDK
```python
from chainup_custody import CustodyClient

client = CustodyClient(
    api_key='your-api-key',
    secret_key='your-secret-key',
    base_url='https://api.custody.chainup.com'
)

# 创建钱包
wallet = client.create_wallet(
    name='My Wallet',
    type='MPC'
)

# 发送交易
transaction = client.create_transaction(
    from_address=wallet['address'],
    to_address='0x123...',
    amount='1.5',
    chain='ETH'
)
```

---

## 安全技术标准

### 加密技术规范

#### 哈希算法
- **SHA-256**：用于交易哈希和数据完整性验证
- **Keccak-256**：用于以太坊相关操作
- **RIPEMD-160**：用于比特币地址生成

#### 签名算法
- **ECDSA**：椭圆曲线数字签名算法
- **EdDSA**：爱德华兹曲线数字签名算法
- **支持的曲线**：secp256k1, secp256r1, ed25519

#### 加密传输
- **TLS 1.3**：所有API通信使用TLS 1.3加密
- **证书验证**：强制验证SSL证书
- **HSTS**：HTTP严格传输安全

### 访问控制

#### 多重身份验证
- **API密钥**：每个API请求需要有效的API密钥
- **签名验证**：请求签名验证防止数据篡改
- **时间戳验证**：防止重放攻击
- **IP白名单**：限制API访问来源

#### 权限管理
```javascript
// 权限控制示例
const permissions = {
  wallet: {
    create: ['admin', 'manager'],
    view: ['admin', 'manager', 'viewer'],
    delete: ['admin']
  },
  transaction: {
    create: ['admin', 'manager'],
    approve: ['admin', 'approver'],
    view: ['admin', 'manager', 'viewer']
  }
};
```

---

## 集成指南

### 快速开始

#### 1. 获取API凭证
```bash
# 在ChainUp Custody平台申请API凭证
# 获取：API Key, Secret Key, 回调URL
```

#### 2. 环境配置
```bash
# 安装SDK
npm install @chainup/custody-sdk

# 或者使用Python
pip install chainup-custody
```

#### 3. 初始化客户端
```javascript
const custody = new ChainUpCustody({
  apiKey: process.env.CUSTODY_API_KEY,
  secretKey: process.env.CUSTODY_SECRET_KEY,
  environment: 'sandbox' // 测试环境
});
```

### 最佳实践

#### 错误处理
```javascript
try {
  const result = await custody.createTransaction(transactionData);
  console.log('交易创建成功:', result);
} catch (error) {
  if (error.code === 'INSUFFICIENT_BALANCE') {
    console.log('余额不足');
  } else if (error.code === 'INVALID_ADDRESS') {
    console.log('地址格式错误');
  } else {
    console.log('未知错误:', error.message);
  }
}
```

#### 回调处理
```javascript
// 设置交易回调
app.post('/custody/callback', (req, res) => {
  const { transactionId, status, hash } = req.body;
  
  // 验证回调签名
  const isValid = custody.verifyCallback(req.body, req.headers);
  
  if (isValid) {
    // 处理交易状态更新
    updateTransactionStatus(transactionId, status, hash);
    res.status(200).send('OK');
  } else {
    res.status(400).send('Invalid signature');
  }
});
```

#### 监控与日志
```javascript
// 交易监控
const monitorTransaction = async (transactionId) => {
  const maxAttempts = 60; // 最大重试次数
  let attempts = 0;
  
  while (attempts < maxAttempts) {
    const transaction = await custody.getTransaction(transactionId);
    
    if (transaction.status === 'confirmed') {
      console.log('交易确认:', transaction);
      break;
    }
    
    await new Promise(resolve => setTimeout(resolve, 10000)); // 等待10秒
    attempts++;
  }
};
```

### 支持的区块链网络

#### 主要公链支持
- **比特币生态**：BTC, BCH, BSV, LTC
- **以太坊生态**：ETH, ETC, ERC-20代币
- **BSC生态**：BNB, BEP-20代币
- **Polygon生态**：MATIC, Polygon代币
- **Tron生态**：TRX, TRC-20代币
- **其他公链**：ADA, DOT, SOL, AVAX等

#### 测试网络
- Bitcoin Testnet
- Ethereum Ropsten/Goerli
- BSC Testnet
- Polygon Mumbai

---

## 技术支持

### 开发者资源
- **API文档**：https://custodydocs-zh.chainup.com/
- **SDK仓库**：https://github.com/chainup-custody
- **示例代码**：https://github.com/chainup-custody/examples

### 联系技术支持
- **邮箱**：custody@chainup.com
- **技术支持**：24/7在线支持
- **社区论坛**：https://forum.chainup.com

---

**ChainUp Custody** - 为开发者提供企业级的数字资产托管技术解决方案。 