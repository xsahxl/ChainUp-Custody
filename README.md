# ChainUp Custody 文档中心

# `app_id`、商户、工作站三者的关系：

---

## 1. `app_id` 的定义

在ChainUp Custody的API文档中，`app_id` 被称为**商户唯一标识**，它是API调用时必须传递的参数，用于标识和认证调用方的身份。

- `app_id` = 商户（Merchant）的唯一ID

---

## 2. 工作站（Workstation）的概念

在ChainUp Custody的产品体系中，**工作站**（有时也叫“站点”或“子账户”）通常是商户下的一个业务单元或操作环境。比如，一个集团公司可能有多个业务部门，每个部门可以有独立的钱包、审批流和权限配置，这些就可以通过“工作站”来实现隔离和管理。

---

## 3. `app_id` 与工作站的关系

- **通常情况下**，一个 `app_id` 只对应一个商户的主工作站（即一个商户一个工作站）。
- **部分定制场景**，ChainUp Custody 支持一个商户下有多个工作站（比如多业务线、多子公司），但**标准API体系下，`app_id` 只代表一个工作站**。

也就是说：
- **标准API调用时，`app_id` 既是商户ID，也是工作站ID**。
- 如果需要多工作站（多业务线隔离），需要联系ChainUp Custody开通多`app_id`，每个`app_id`对应一个独立的工作站和API密钥。

---

## 4. 一个商户能否有多个工作站？

- **标准SaaS模式下**：一个商户只有一个`app_id`，即一个工作站。
- **定制/企业版场景**：可以为一个商户分配多个`app_id`，每个`app_id`就是一个独立的工作站，数据完全隔离，权限独立。

---

## 5. 总结

- `app_id` 是商户的唯一标识，也是API层面的“工作站”标识。
- 一个标准商户通常只有一个工作站（即一个`app_id`）。
- 如需多工作站（多业务线/多子公司/多环境），需申请多个`app_id`，每个`app_id`就是一个独立的工作站。

---

**参考文档：**  
[ChainUp Custody API - 创建MPC钱包](https://custodydocs-zh.chainup.com/api-references/mpc-apis/apis/sub-wallet/subwallet-create)

如需多工作站或多业务线支持，建议联系ChainUp Custody官方进行定制化开通。