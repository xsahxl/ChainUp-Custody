# QQC投资管理平台报价方案

## 一、项目概述

### 1.1 项目背景

QQC投资管理平台是一个基于Solana区块链的通证经济平台，采用NFT质押和节点共识机制，通过合理的通证分配和激励机制，打造可持续发展的生态系统。

### 1.2 技术方案

- **区块链**：Solana + SPL代币标准
- **托管服务**：ChainUP专业托管
- **用户端**：React H5应用
- **管理端**：Node.js后台管理系统
- **开发策略**：分两期开发，快速上线

### 1.3 通证经济模型

#### 1.3.1 通证分配方案

**公司资产管理（45%）**
- 深圳老板公司股权储备（35%）
  * 用于公司发展储备
  * 锁定期管理
  * 分批释放计划
- 董事发展（10%）
  * 团队激励池
  * 顾问持股池
  * 战略合作储备
- 每日释放量：27,397.2604枚
- 释放进度实时监控

**原始NFT管理（20%）**
- NFT发行规模：2亿枚
- 单价：2,000U/张
- 单张：1万枚
- 质押管理：18个月释放期
- 销售奖励机制：
  * 销售>10条：10%奖励
  * 销售>100条：15%奖励
  * 销售>500条：20%奖励

**铸造产出管理（35%）**
- 五年产出计划：
  * 第一年：5,000万枚（每天136,986.3013枚）
  * 第二年：6,000万枚（每天164,383.5616枚）
  * 第三年：7,000万枚（每天191,780.8219枚）
  * 第四年：8,000万枚（每天219,178.0821枚）
  * 第五年：9,000万枚（每天246,575.3424枚）

#### 1.3.2 节点等级体系

**普通用户**
- 准入要求：持有任意数量QQC
- 权益：
  * 基础收益权益
  * 推荐奖励资格
  * 特惠活动参与

**普通节点**
- 准入要求：
  * 个人持有>2,000U QQC
  * 社区规模>4,000U枚QQC
- 权益：
  * 90%推广收益权
  * 20%特惠产出分红
  * 节点专属权益

**高级节点**
- 准入要求：
  * 个人持有>5,000U枚QQC
  * 社区规模>2万U枚QQC
- 权益：
  * 100%推广收益权
  * 10%特惠产出分红
  * 高级节点特权

**超级节点**
- 准入要求：
  * 个人持有>3万U枚QQC
  * 社区规模>15万U枚QQC
- 权益：
  * 120%推广收益权
  * 10%特惠产出分红
  * 超级节点特权

#### 1.3.3 收益分配机制

**质押收益**
- 日收益率：0.1%
- 年化收益率：36.5%
- 收益实时计算
- 支持随时提取

**节点收益**
- 基于节点等级分配
- 社区规模影响收益比例
- 动态调整机制
- 透明化收益展示

**邀请奖励**
- 直接推荐奖励：5%
- 间接推荐奖励：2%
- 团队规模奖励
- 等级晋升奖励

#### 1.3.4 风控机制

**价格稳定机制**
- 智能合约自动调节
- 市场供需平衡
- 防止价格操纵
- 流动性管理

**风险控制**
- 单日交易限额
- 异常交易监控
- 资金流向追踪
- 安全预警系统

## 二、成本分析

### 2.1 开发成本明细

#### 2.1.1 人力成本（1.75个月）


| 岗位             | 人数  | 月薪     | 工期   | 小计          |
| ---------------- | ----- | -------- | ------ | ------------- |
| 前端开发工程师   | 1人   | 25,000元 | 1.75月 | 43,750元      |
| 后端开发工程师   | 1人   | 30,000元 | 1.75月 | 52,500元      |
| 区块链开发工程师 | 0.5人 | 35,000元 | 1.75月 | 30,625元      |
| 测试工程师       | 0.5人 | 20,000元 | 1.75月 | 17,500元      |
| **人力成本小计** |       |          |        | **144,375元** |

#### 2.1.2 基础设施成本（首年）


| 项目             | 费用            | 说明             |
| ---------------- | --------------- | ---------------- |
| 服务器费用       | 20,000元/年     | 阿里云ECS集群    |
| 数据库费用       | 15,000元/年     | MongoDB + Redis  |
| 区块链节点       | 10,000元/年     | Solana RPC节点   |
| 安全设施         | 8,000元/年      | 防火墙、安全组等 |
| **基础设施小计** | **53,000元/年** |                  |

#### 2.1.3 第三方服务成本


| 服务               | 费用            | 说明               |
| ------------------ | --------------- | ------------------ |
| ChainUP托管服务    | 60,000元/年     | 专业数字资产托管   |
| 域名和SSL证书      | 2,000元/年      | 域名注册和SSL证书  |
| CDN加速服务        | 5,000元/年      | 阿里云CDN          |
| 监控和日志         | 3,000元/年      | 系统监控和日志服务 |
| **第三方服务小计** | **70,000元/年** |                    |

#### 2.1.4 其他成本


| 项目             | 费用         | 说明                     |
| ---------------- | ------------ | ------------------------ |
| 开发测试环境     | 20,000元     | 开发服务器、测试环境搭建 |
| 应急费用         | 20,000元     | 不可预见费用             |
| **其他成本小计** | **40,000元** |                          |

### 2.2 运维成本（首年）


| 项目             | 月费用          | 年费用           | 说明              |
| ---------------- | --------------- | ---------------- | ----------------- |
| 系统运维         | 6,000元/月      | 72,000元/年      | 7×24小时系统监控 |
| 安全维护         | 4,000元/月      | 48,000元/年      | 安全漏洞修复      |
| 数据备份         | 2,500元/月      | 30,000元/年      | 数据备份和恢复    |
| 技术支持         | 3,000元/月      | 36,000元/年      | 用户技术支持      |
| **运维成本小计** | **15,500元/月** | **186,000元/年** |                   |

### 2.3 总成本汇总


| 成本类别   | 金额          | 占比     |
| ---------- | ------------- | -------- |
| 人力成本   | 144,375元     | 25.4%    |
| 基础设施   | 53,000元      | 9.3%     |
| 第三方服务 | 70,000元      | 12.3%    |
| 其他成本   | 40,000元      | 7.0%     |
| 运维成本   | 186,000元     | 32.7%    |
| **总成本** | **493,375元** | **100%** |

## 三、报价方案

### 3.1 成本与报价说明

**实际总成本：493,375元**
**报价溢价说明：**

- **技术风险溢价**：区块链项目技术风险较高，需要预留风险缓冲
- **质量保证溢价**：确保项目质量，包含额外的测试和优化成本
- **服务保障溢价**：提供1年免费运维支持，需要预留服务成本
- **利润空间**：合理的商业利润，确保项目可持续发展

### 3.2 基础报价方案

#### 方案A：全包服务

**总价：588,000元**

- 包含所有开发、部署、运维服务
- 提供1年免费运维支持
- 提供技术培训和文档
- **溢价：94,625元（19.2%）**

#### 方案B：开发+部署（不涉及三方服务）

**总价：438,000元**

- 包含开发和部署服务
- 提供3个月免费运维支持
- 提供技术文档
- **溢价：44,625元（11.3%）**

#### 方案C：纯开发服务

**总价：288,000元**

- 仅包含开发服务
- 提供代码交付和技术文档
- 不包含部署和运维服务
- **溢价：43,625元（17.9%）**

### 3.3 分期付款方案

#### 方案A：三期付款（推荐）

- **第一期（签约）**：40% = 235,200元
- **第二期（开发完成）**：40% = 235,200元
- **第三期（上线验收）**：20% = 117,600元

#### 方案B：四期付款

- **第一期（签约）**：30% = 176,400元
- **第二期（架构完成）**：30% = 176,400元
- **第三期（功能完成）**：25% = 147,000元
- **第四期（上线验收）**：15% = 88,200元

### 3.4 增值服务

#### 3.3.1 运维服务


| 服务等级 | 月费用      | 年费用       | 服务内容               |
| -------- | ----------- | ------------ | ---------------------- |
| 基础运维 | 8,000元/月  | 96,000元/年  | 7×24监控、基础维护    |
| 标准运维 | 12,000元/月 | 144,000元/年 | 包含安全维护、性能优化 |
| 高级运维 | 18,000元/月 | 216,000元/年 | 包含数据分析、运营支持 |

#### 3.3.2 功能扩展


| 功能模块     | 开发费用  | 工期 | 说明                   |
| ------------ | --------- | ---- | ---------------------- |
| 高级数据分析 | 80,000元  | 2周  | 用户行为分析、收益统计 |
| 风控系统     | 60,000元  | 2周  | 异常交易监控、风险预警 |
| 移动端APP    | 120,000元 | 4周  | iOS/Android原生应用    |
| 多语言支持   | 40,000元  | 1周  | 英文、韩文等多语言     |

## 四、技术方案

### 4.1 Solana代币合约设计

#### 4.1.1 QQC代币合约伪代码

```rust
// QQC代币合约 (Solana Program)
use anchor_lang::prelude::*;
use anchor_spl::token::{self, Token, TokenAccount, Transfer};

declare_id!("QQC代币程序ID");

#[program]
pub mod qqc_token {
    use super::*;

    // 初始化代币
    pub fn initialize(ctx: Context<Initialize>, total_supply: u64) -> Result<()> {
        let token_mint = &mut ctx.accounts.token_mint;
        token_mint.supply = total_supply;  // 总发行量：10亿枚
        token_mint.decimals = 9;           // 小数位数：9位
        token_mint.is_initialized = true;
        Ok(())
    }

    // 铸造代币
    pub fn mint_to(ctx: Context<MintTo>, amount: u64) -> Result<()> {
        let cpi_accounts = MintTo {
            mint: ctx.accounts.token_mint.to_account_info(),
            to: ctx.accounts.token_account.to_account_info(),
            authority: ctx.accounts.authority.to_account_info(),
        };
        let cpi_program = ctx.accounts.token_program.to_account_info();
        let cpi_ctx = CpiContext::new(cpi_program, cpi_accounts);
        token::mint_to(cpi_ctx, amount)?;
        Ok(())
    }

    // 转账代币
    pub fn transfer(ctx: Context<Transfer>, amount: u64) -> Result<()> {
        let cpi_accounts = Transfer {
            from: ctx.accounts.from.to_account_info(),
            to: ctx.accounts.to.to_account_info(),
            authority: ctx.accounts.authority.to_account_info(),
        };
        let cpi_program = ctx.accounts.token_program.to_account_info();
        let cpi_ctx = CpiContext::new(cpi_program, cpi_accounts);
        token::transfer(cpi_ctx, amount)?;
        Ok(())
    }

    // 质押代币
    pub fn stake(ctx: Context<Stake>, amount: u64) -> Result<()> {
        let stake_account = &mut ctx.accounts.stake_account;
        stake_account.owner = ctx.accounts.owner.key();
        stake_account.amount = amount;
        stake_account.start_time = Clock::get()?.unix_timestamp;
        stake_account.is_active = true;
        Ok(())
    }

    // 解除质押
    pub fn unstake(ctx: Context<Unstake>) -> Result<()> {
        let stake_account = &mut ctx.accounts.stake_account;
        stake_account.is_active = false;
        stake_account.end_time = Clock::get()?.unix_timestamp;
        Ok(())
    }

    // 计算质押收益
    pub fn calculate_rewards(ctx: Context<CalculateRewards>) -> Result<u64> {
        let stake_account = &ctx.accounts.stake_account;
        let current_time = Clock::get()?.unix_timestamp;
        let staking_duration = current_time - stake_account.start_time;
        let daily_rate = 1000; // 0.1% 日收益率
        let rewards = (stake_account.amount * daily_rate * staking_duration) / (24 * 3600 * 100000);
        Ok(rewards)
    }
}

// 账户结构定义
#[derive(Accounts)]
pub struct Initialize<'info> {
    #[account(init, payer = authority, mint = token_mint, authority = authority.key())]
    pub token_mint: Account<'info, Mint>,
    #[account(mut)]
    pub authority: Signer<'info>,
    pub system_program: Program<'info, System>,
    pub token_program: Program<'info, Token>,
    pub rent: Sysvar<'info, Rent>,
}

#[derive(Accounts)]
pub struct MintTo<'info> {
    #[account(mut)]
    pub token_mint: Account<'info, Mint>,
    #[account(mut)]
    pub token_account: Account<'info, TokenAccount>,
    pub authority: Signer<'info>,
    pub token_program: Program<'info, Token>,
}

#[derive(Accounts)]
pub struct Transfer<'info> {
    #[account(mut)]
    pub from: Account<'info, TokenAccount>,
    #[account(mut)]
    pub to: Account<'info, TokenAccount>,
    pub authority: Signer<'info>,
    pub token_program: Program<'info, Token>,
}

#[derive(Accounts)]
pub struct Stake<'info> {
    #[account(init, payer = owner, space = 8 + 32 + 8 + 8 + 1)]
    pub stake_account: Account<'info, StakeAccount>,
    #[account(mut)]
    pub owner: Signer<'info>,
    pub system_program: Program<'info, System>,
}

#[derive(Accounts)]
pub struct Unstake<'info> {
    #[account(mut)]
    pub stake_account: Account<'info, StakeAccount>,
    pub owner: Signer<'info>,
}

#[derive(Accounts)]
pub struct CalculateRewards<'info> {
    pub stake_account: Account<'info, StakeAccount>,
}

// 质押账户数据结构
#[account]
pub struct StakeAccount {
    pub owner: Pubkey,      // 质押者地址
    pub amount: u64,        // 质押数量
    pub start_time: i64,    // 开始时间
    pub end_time: i64,      // 结束时间
    pub is_active: bool,    // 是否激活
}
```

#### 4.1.2 代币分配策略

```typescript
// 代币分配配置
const TOKEN_DISTRIBUTION = {
  totalSupply: 1000000000, // 10亿枚
  decimals: 9,
  
  // 分配比例
  allocation: {
    companyReserve: 0.45,    // 45% - 公司储备
    nftStaking: 0.20,        // 20% - NFT质押
    miningRewards: 0.35      // 35% - 挖矿奖励
  },
  
  // 释放计划
  releaseSchedule: {
    dailyRelease: 27397.2604, // 每日释放量
    nftReleasePeriod: 18,     // NFT释放期(月)
    miningYears: 5            // 挖矿年限
  }
};

// 节点等级配置
const NODE_LEVELS = {
  regular_user: {
    minPersonalHolding: 0,
    minCommunitySize: 0,
    rewardMultiplier: 0
  },
  normal_node: {
    minPersonalHolding: 2000,
    minCommunitySize: 4000,
    rewardMultiplier: 0.9
  },
  advanced_node: {
    minPersonalHolding: 5000,
    minCommunitySize: 20000,
    rewardMultiplier: 1.0
  },
  super_node: {
    minPersonalHolding: 30000,
    minCommunitySize: 150000,
    rewardMultiplier: 1.2
  }
};
```

#### 4.1.3 收益计算算法

```typescript
// 收益计算服务
class RewardCalculationService {
  
  // 计算质押收益
  calculateStakeRewards(stakeAmount: number, stakeDays: number): number {
    const dailyRate = 0.001; // 0.1% 日收益率
    return stakeAmount * dailyRate * stakeDays;
  }
  
  // 计算节点收益
  calculateNodeRewards(userLevel: string, baseReward: number): number {
    const multipliers = {
      regular_user: 0,
      normal_node: 0.9,
      advanced_node: 1.0,
      super_node: 1.2
    };
    return baseReward * multipliers[userLevel];
  }
  
  // 计算邀请奖励
  calculateInviteRewards(inviteLevel: string, inviteCount: number): number {
    const rewards = {
      A: 1000,  // A级推荐：1000元/区
      B: 10000, // B级推荐：10000元/区
      C: 100000 // C级推荐：100000元/区
    };
    return rewards[inviteLevel] * inviteCount;
  }
  
  // 计算每日释放量
  calculateDailyRelease(): number {
    const totalSupply = 1000000000; // 10亿枚
    const releaseYears = 5; // 5年释放期
    const daysPerYear = 365;
    
    return totalSupply / (releaseYears * daysPerYear);
  }
}
```

### 4.2 项目交付

#### 4.2.1 技术交付

- ✅ 完整的源代码
- ✅ 技术文档和API文档
- ✅ 部署文档和运维手册
- ✅ 数据库设计文档
- ✅ 测试报告

#### 4.2.2 功能交付

- ✅ 用户端H5应用
- ✅ 管理后台系统
- ✅ Solana智能合约
- ✅ ChainUP托管集成
- ✅ 钱包连接功能

#### 4.2.3 服务交付

- ✅ 技术培训服务
- ✅ 上线部署支持
- ✅ 运维技术支持
- ✅ 基础安全指导

### 4.3 功能页面详细说明

#### 4.2.1 用户端H5功能（前端）

**首页**

- 资产总览面板（QQC余额、NFT持仓、累计收益）
- 快捷操作入口（认购、质押、邀请）
- 系统公告展示
- 实时市场行情

**认购页面**

- NFT详情展示（价格、收益、释放期）
- 认购表单（数量选择、支付确认）
- 认购进度展示
- 认购记录查询

**质押页面**

- QQC代币质押表单
- 质押收益计算器
- 质押记录管理
- 收益提取功能

**邀请页面**

- 个人邀请码生成
- 邀请链接分享
- 团队数据展示（成员数量、等级分布）
- 邀请奖励查询

**个人中心**

- 账户信息管理
- 资产明细展示
- 交易记录查询
- 安全设置选项

#### 4.2.2 管理后台功能（运维端）

**用户管理模块**

- 用户列表查看（分页、搜索、筛选）
- 用户详情查询（基本信息、资产数据、交易记录）
- 用户状态管理（启用/禁用、等级调整）
- 认购记录管理（审核、统计、导出）

**资产管理模块**

- NFT发行管理（发行计划、状态监控）
- 代币管理（铸造记录、流通统计）
- 质押管理（质押状态、收益统计）
- 交易记录审计（交易查询、异常监控）

**运营管理模块**

- 系统公告发布（编辑、发布、撤回）
- 活动配置管理（活动创建、参与统计）
- 数据统计查看（用户增长、交易量、收益统计）
- 基础风控设置（限额配置、规则设置）

**系统管理模块**

- 角色权限管理（管理员、运营员、财务员）
- 系统参数配置（代币参数、收益规则）
- 操作日志查询（用户操作、系统日志）
- 数据字典维护（状态码、配置项）

### 4.4 功能分期说明

#### 4.3.1 第一期功能（4周）

**用户端H5（MVP版本）**

- ✅ 钱包连接（Phantom、Solflare等）
- ✅ 基础认购功能（NFT认购、支付确认）
- ✅ 基础质押功能（QQC质押、收益计算）
- ✅ 基础邀请功能（邀请码、团队数据）
- ✅ 个人中心（账户信息、资产展示）

**管理后台（基础版本）**

- ✅ 用户管理（用户列表、详情查看）
- ✅ 基础运营（公告发布、数据统计）
- ✅ 系统管理（角色权限、参数配置）

#### 4.3.2 第二期功能（3周）

**用户端H5（完善版本）**

- 📊 高级数据分析（收益趋势、投资建议）
- 🎯 个性化推荐（投资机会、等级提升）
- 🔔 消息通知（系统通知、收益提醒）
- 📱 移动端优化（响应式设计、性能优化）

**管理后台（高级版本）**

- 📈 高级数据分析（用户行为、收益统计）
- 🛡️ 风控系统（异常监控、风险预警）
- 🎪 活动管理系统（活动创建、效果分析）
- 📊 报表系统（财务报表、运营报表）

### 4.5 交付时间

#### 第一期（4周）

- 第1-2周：基础架构搭建

  * 前端项目搭建（React + TypeScript）
  * 后端服务搭建（Node.js + Express）
  * 数据库设计和部署
  * ChainUP API集成
  * Solana合约部署
- 第3-4周：核心功能开发

  * 用户端H5 MVP功能开发
  * 管理后台基础功能开发
  * 钱包连接功能集成
  * 基础测试和优化
- 交付：MVP版本，可进行内部测试

#### 第二期（3周）

- 第5-6周：功能完善和优化

  * 用户端高级功能开发
  * 管理后台高级功能开发
  * 性能优化和安全加固
  * 用户体验优化
- 第7周：测试和部署

  * 全面功能测试
  * 性能测试和安全测试
  * 生产环境部署
  * 用户培训和技术文档
- 交付：正式上线版本

### 4.6 验收标准

#### 4.3.1 功能验收

- ✅ 用户注册和钱包连接
- ✅ NFT认购功能
- ✅ 代币质押功能
- ✅ 邀请系统功能
- ✅ 管理后台功能

#### 4.3.2 性能验收

- ✅ 页面加载时间 < 3秒
- ✅ 并发用户数 > 1000
- ✅ 系统可用性 > 99.9%
- ✅ 数据备份和恢复

#### 4.3.3 安全验收

- ✅ 基础安全测试通过
- ✅ 数据加密和传输安全
- ✅ 权限控制和访问管理
- ✅ 代码质量检查通过

## 五、售后服务

### 5.1 免费服务期

- **基础运维**：1年免费
- **技术支持**：1年免费
- **系统更新**：1年免费
- **功能优化**：3个月免费

### 5.2 收费服务

- **运维服务**：8,000-18,000元/月
- **功能扩展**：按需报价
- **技术咨询**：1,000元/小时
- **紧急支持**：2,000元/次

### 5.3 服务承诺

- **响应时间**：4小时内响应
- **故障修复**：24小时内修复
- **数据安全**：99.9%数据安全保证
- **系统稳定**：99.9%系统可用性

## 五、前后端页面结构

### 5.1 前端页面结构（React H5）

```
src/
├── pages/                    # 页面组件
│   ├── Home/                # 首页
│   │   ├── index.tsx       # 首页主组件
│   │   ├── AssetOverview.tsx # 资产总览
│   │   ├── QuickActions.tsx # 快捷操作
│   │   └── Announcements.tsx # 系统公告
│   ├── Subscribe/           # 认购页面
│   │   ├── index.tsx       # 认购主页面
│   │   ├── NFTDetail.tsx   # NFT详情
│   │   ├── SubscribeForm.tsx # 认购表单
│   │   └── SubscribeRecords.tsx # 认购记录
│   ├── Stake/              # 质押页面
│   │   ├── index.tsx       # 质押主页面
│   │   ├── StakeForm.tsx   # 质押表单
│   │   ├── RewardCalculator.tsx # 收益计算器
│   │   └── StakeRecords.tsx # 质押记录
│   ├── Invite/             # 邀请页面
│   │   ├── index.tsx       # 邀请主页面
│   │   ├── InviteCode.tsx  # 邀请码
│   │   ├── TeamData.tsx    # 团队数据
│   │   └── InviteRewards.tsx # 邀请奖励
│   └── Profile/            # 个人中心
│       ├── index.tsx       # 个人中心主页面
│       ├── AccountInfo.tsx # 账户信息
│       ├── AssetDetails.tsx # 资产明细
│       └── TransactionHistory.tsx # 交易记录
├── components/              # 通用组件
│   ├── WalletConnect/      # 钱包连接
│   │   ├── index.tsx       # 钱包连接组件
│   │   ├── PhantomWallet.tsx # Phantom钱包
│   │   └── SolflareWallet.tsx # Solflare钱包
│   ├── NFT/                # NFT相关组件
│   │   ├── NFTCard.tsx     # NFT卡片
│   │   ├── NFTDetail.tsx   # NFT详情
│   │   └── NFTList.tsx     # NFT列表
│   ├── Reward/             # 收益相关组件
│   │   ├── RewardCard.tsx  # 收益卡片
│   │   ├── RewardChart.tsx # 收益图表
│   │   └── RewardHistory.tsx # 收益历史
│   └── Common/             # 通用组件
│       ├── Header.tsx      # 头部导航
│       ├── Footer.tsx      # 底部导航
│       ├── Loading.tsx     # 加载组件
│       └── Modal.tsx       # 弹窗组件
├── services/               # 服务层
│   ├── api.ts             # API请求封装
│   ├── wallet.ts          # 钱包服务
│   ├── nft.ts             # NFT服务
│   ├── stake.ts           # 质押服务
│   └── reward.ts          # 收益服务
├── store/                 # 状态管理
│   ├── index.ts           # Store配置
│   ├── slices/            # Redux切片
│   │   ├── walletSlice.ts # 钱包状态
│   │   ├── userSlice.ts   # 用户状态
│   │   ├── nftSlice.ts    # NFT状态
│   │   └── rewardSlice.ts # 收益状态
│   └── hooks/             # 自定义Hooks
│       ├── useWallet.ts   # 钱包Hook
│       ├── useNFT.ts      # NFT Hook
│       └── useReward.ts   # 收益Hook
├── utils/                 # 工具函数
│   ├── constants.ts       # 常量定义
│   ├── helpers.ts         # 工具函数
│   ├── formatters.ts      # 格式化函数
│   └── validators.ts      # 验证函数
└── styles/                # 样式文件
    ├── global.css         # 全局样式
    ├── components.css     # 组件样式
    └── variables.css      # CSS变量
```

### 5.2 后端API结构（Node.js）

```
src/
├── controllers/            # 控制器层
│   ├── userController.ts  # 用户管理
│   │   ├── connectWallet.ts # 钱包连接
│   │   ├── getUserProfile.ts # 获取用户信息
│   │   ├── updateProfile.ts # 更新用户信息
│   │   └── getUserStats.ts # 获取用户统计
│   ├── subscribeController.ts # 认购管理
│   │   ├── getNFTList.ts  # 获取NFT列表
│   │   ├── purchaseNFT.ts # 认购NFT
│   │   ├── getSubscribeRecords.ts # 获取认购记录
│   │   └── getSubscribeProgress.ts # 获取认购进度
│   ├── stakeController.ts # 质押管理
│   │   ├── stakeTokens.ts # 质押代币
│   │   ├── unstakeTokens.ts # 解除质押
│   │   ├── getStakeRecords.ts # 获取质押记录
│   │   ├── withdrawRewards.ts # 提取收益
│   │   └── calculateRewards.ts # 计算收益
│   ├── inviteController.ts # 邀请管理
│   │   ├── getInviteCode.ts # 获取邀请码
│   │   ├── getTeamData.ts # 获取团队数据
│   │   ├── getInviteRewards.ts # 获取邀请奖励
│   │   └── getInviteStats.ts # 获取邀请统计
│   └── adminController.ts # 管理后台
│       ├── userManagement.ts # 用户管理
│       ├── assetManagement.ts # 资产管理
│       ├── operationManagement.ts # 运营管理
│       └── systemManagement.ts # 系统管理
├── services/              # 服务层
│   ├── chainupService.ts  # ChainUP托管服务
│   │   ├── createWallet.ts # 创建钱包
│   │   ├── getBalance.ts  # 获取余额
│   │   ├── transfer.ts    # 转账
│   │   └── getTransactionHistory.ts # 获取交易历史
│   ├── solanaService.ts   # Solana区块链服务
│   │   ├── connect.ts     # 连接Solana
│   │   ├── mintToken.ts   # 铸造代币
│   │   ├── transferToken.ts # 转账代币
│   │   ├── stakeToken.ts  # 质押代币
│   │   └── calculateRewards.ts # 计算收益
│   ├── walletService.ts   # 钱包服务
│   │   ├── connectWallet.ts # 连接钱包
│   │   ├── signTransaction.ts # 签名交易
│   │   └── signMessage.ts # 签名消息
│   └── rewardService.ts   # 收益服务
│       ├── calculateStakeRewards.ts # 计算质押收益
│       ├── calculateNodeRewards.ts # 计算节点收益
│       ├── calculateInviteRewards.ts # 计算邀请奖励
│       └── distributeRewards.ts # 分配收益
├── models/                # 数据模型
│   ├── User.ts           # 用户模型
│   │   ├── interface.ts  # 用户接口定义
│   │   ├── schema.ts     # 用户数据模式
│   │   └── methods.ts    # 用户方法
│   ├── NFT.ts            # NFT模型
│   │   ├── interface.ts  # NFT接口定义
│   │   ├── schema.ts     # NFT数据模式
│   │   └── methods.ts    # NFT方法
│   ├── Transaction.ts    # 交易模型
│   │   ├── interface.ts  # 交易接口定义
│   │   ├── schema.ts     # 交易数据模式
│   │   └── methods.ts    # 交易方法
│   └── Reward.ts         # 收益模型
│       ├── interface.ts  # 收益接口定义
│       ├── schema.ts     # 收益数据模式
│       └── methods.ts    # 收益方法
├── routes/                # 路由层
│   ├── userRoutes.ts     # 用户路由
│   │   ├── GET /api/user/profile # 获取用户信息
│   │   ├── POST /api/user/connect-wallet # 连接钱包
│   │   ├── PUT /api/user/profile # 更新用户信息
│   │   └── GET /api/user/stats # 获取用户统计
│   ├── subscribeRoutes.ts # 认购路由
│   │   ├── GET /api/subscribe/nfts # 获取NFT列表
│   │   ├── POST /api/subscribe/purchase # 认购NFT
│   │   ├── GET /api/subscribe/records # 获取认购记录
│   │   └── GET /api/subscribe/progress # 获取认购进度
│   ├── stakeRoutes.ts    # 质押路由
│   │   ├── POST /api/stake/token # 质押代币
│   │   ├── POST /api/stake/unstake # 解除质押
│   │   ├── GET /api/stake/records # 获取质押记录
│   │   ├── POST /api/stake/withdraw # 提取收益
│   │   └── GET /api/stake/rewards # 计算收益
│   ├── inviteRoutes.ts   # 邀请路由
│   │   ├── GET /api/invite/code # 获取邀请码
│   │   ├── GET /api/invite/team # 获取团队数据
│   │   ├── GET /api/invite/rewards # 获取邀请奖励
│   │   └── GET /api/invite/stats # 获取邀请统计
│   └── adminRoutes.ts    # 管理后台路由
│       ├── GET /api/admin/users # 获取用户列表
│       ├── GET /api/admin/user/:id # 获取用户详情
│       ├── PUT /api/admin/user/:id # 更新用户状态
│       ├── GET /api/admin/assets # 获取资产统计
│       ├── POST /api/admin/announcement # 发布公告
│       └── GET /api/admin/statistics # 获取统计数据
├── middleware/            # 中间件
│   ├── auth.ts           # 认证中间件
│   ├── rateLimit.ts      # 限流中间件
│   ├── validation.ts     # 验证中间件
│   └── errorHandler.ts   # 错误处理中间件
├── config/               # 配置文件
│   ├── database.ts       # 数据库配置
│   ├── redis.ts          # Redis配置
│   ├── solana.ts         # Solana配置
│   └── chainup.ts        # ChainUP配置
├── utils/                # 工具函数
│   ├── logger.ts         # 日志工具
│   ├── encryption.ts     # 加密工具
│   ├── validation.ts     # 验证工具
│   └── helpers.ts        # 辅助函数
└── tests/                # 测试文件
    ├── unit/             # 单元测试
    ├── integration/      # 集成测试
    └── e2e/             # 端到端测试
```

### 5.3 数据库结构设计

```sql
-- 用户表
CREATE TABLE users (
    id VARCHAR(36) PRIMARY KEY,
    wallet_address VARCHAR(44) UNIQUE NOT NULL,
    username VARCHAR(50),
    email VARCHAR(100),
    phone VARCHAR(20),
    node_level ENUM('regular_user', 'normal_node', 'advanced_node', 'super_node') DEFAULT 'regular_user',
    personal_holding DECIMAL(20,9) DEFAULT 0,
    community_size DECIMAL(20,9) DEFAULT 0,
    referral_code VARCHAR(20) UNIQUE,
    referred_by VARCHAR(36),
    status ENUM('active', 'inactive', 'banned') DEFAULT 'active',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    INDEX idx_wallet_address (wallet_address),
    INDEX idx_referral_code (referral_code),
    INDEX idx_node_level (node_level)
);

-- NFT表
CREATE TABLE nfts (
    id VARCHAR(36) PRIMARY KEY,
    token_id VARCHAR(100) UNIQUE NOT NULL,
    name VARCHAR(100) NOT NULL,
    description TEXT,
    price DECIMAL(20,2) NOT NULL,
    qqc_value DECIMAL(20,9) NOT NULL,
    release_period INT NOT NULL, -- 释放期(月)
    total_supply INT NOT NULL,
    sold_count INT DEFAULT 0,
    status ENUM('active', 'inactive', 'sold_out') DEFAULT 'active',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    INDEX idx_token_id (token_id),
    INDEX idx_status (status)
);

-- 认购记录表
CREATE TABLE subscribe_records (
    id VARCHAR(36) PRIMARY KEY,
    user_id VARCHAR(36) NOT NULL,
    nft_id VARCHAR(36) NOT NULL,
    amount DECIMAL(20,2) NOT NULL,
    qqc_amount DECIMAL(20,9) NOT NULL,
    payment_method ENUM('usdt', 'usdc', 'sol') NOT NULL,
    transaction_hash VARCHAR(100),
    status ENUM('pending', 'completed', 'failed', 'refunded') DEFAULT 'pending',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (user_id) REFERENCES users(id),
    FOREIGN KEY (nft_id) REFERENCES nfts(id),
    INDEX idx_user_id (user_id),
    INDEX idx_status (status),
    INDEX idx_transaction_hash (transaction_hash)
);

-- 质押记录表
CREATE TABLE stake_records (
    id VARCHAR(36) PRIMARY KEY,
    user_id VARCHAR(36) NOT NULL,
    amount DECIMAL(20,9) NOT NULL,
    start_time TIMESTAMP NOT NULL,
    end_time TIMESTAMP,
    daily_reward_rate DECIMAL(10,6) DEFAULT 0.001, -- 0.1%日收益率
    total_rewards DECIMAL(20,9) DEFAULT 0,
    status ENUM('active', 'completed', 'cancelled') DEFAULT 'active',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (user_id) REFERENCES users(id),
    INDEX idx_user_id (user_id),
    INDEX idx_status (status),
    INDEX idx_start_time (start_time)
);

-- 收益记录表
CREATE TABLE reward_records (
    id VARCHAR(36) PRIMARY KEY,
    user_id VARCHAR(36) NOT NULL,
    reward_type ENUM('stake', 'node', 'invite', 'daily_release') NOT NULL,
    amount DECIMAL(20,9) NOT NULL,
    reference_id VARCHAR(36), -- 关联的质押记录或邀请记录ID
    transaction_hash VARCHAR(100),
    status ENUM('pending', 'completed', 'failed') DEFAULT 'pending',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (user_id) REFERENCES users(id),
    INDEX idx_user_id (user_id),
    INDEX idx_reward_type (reward_type),
    INDEX idx_status (status)
);

-- 交易记录表
CREATE TABLE transactions (
    id VARCHAR(36) PRIMARY KEY,
    user_id VARCHAR(36) NOT NULL,
    transaction_type ENUM('subscribe', 'stake', 'unstake', 'withdraw', 'transfer') NOT NULL,
    amount DECIMAL(20,9) NOT NULL,
    from_address VARCHAR(44),
    to_address VARCHAR(44),
    transaction_hash VARCHAR(100) UNIQUE,
    block_number BIGINT,
    gas_fee DECIMAL(20,9),
    status ENUM('pending', 'confirmed', 'failed') DEFAULT 'pending',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (user_id) REFERENCES users(id),
    INDEX idx_user_id (user_id),
    INDEX idx_transaction_type (transaction_type),
    INDEX idx_transaction_hash (transaction_hash),
    INDEX idx_status (status)
);

-- 系统配置表
CREATE TABLE system_configs (
    id VARCHAR(36) PRIMARY KEY,
    config_key VARCHAR(100) UNIQUE NOT NULL,
    config_value TEXT NOT NULL,
    description TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    INDEX idx_config_key (config_key)
);

-- 操作日志表
CREATE TABLE operation_logs (
    id VARCHAR(36) PRIMARY KEY,
    user_id VARCHAR(36),
    operation_type VARCHAR(100) NOT NULL,
    operation_desc TEXT,
    ip_address VARCHAR(45),
    user_agent TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    INDEX idx_user_id (user_id),
    INDEX idx_operation_type (operation_type),
    INDEX idx_created_at (created_at)
);
```

### 5.4 功能页面详细说明

#### 5.4.1 用户端H5功能（前端）

**首页**
- 资产总览面板（QQC余额、NFT持仓、累计收益）
- 快捷操作入口（认购、质押、邀请）
- 系统公告展示
- 实时市场行情

**认购页面**
- NFT详情展示（价格、收益、释放期）
- 认购表单（数量选择、支付确认）
- 认购进度展示
- 认购记录查询

**质押页面**
- QQC代币质押表单
- 质押收益计算器
- 质押记录管理
- 收益提取功能

**邀请页面**
- 个人邀请码生成
- 邀请链接分享
- 团队数据展示（成员数量、等级分布）
- 邀请奖励查询

**个人中心**
- 账户信息管理
- 资产明细展示
- 交易记录查询
- 安全设置选项

#### 5.4.2 管理后台功能（运维端）

**用户管理模块**
- 用户列表查看（分页、搜索、筛选）
- 用户详情查询（基本信息、资产数据、交易记录）
- 用户状态管理（启用/禁用、等级调整）
- 认购记录管理（审核、统计、导出）

**资产管理模块**
- NFT发行管理（发行计划、状态监控）
- 代币管理（铸造记录、流通统计）
- 质押管理（质押状态、收益统计）
- 交易记录审计（交易查询、异常监控）

**运营管理模块**
- 系统公告发布（编辑、发布、撤回）
- 活动配置管理（活动创建、参与统计）
- 数据统计查看（用户增长、交易量、收益统计）
- 基础风控设置（限额配置、规则设置）

**系统管理模块**
- 角色权限管理（管理员、运营员、财务员）
- 系统参数配置（代币参数、收益规则）
- 操作日志查询（用户操作、系统日志）
- 数据字典维护（状态码、配置项）


