# SD-OS-001 · 数字科技业务总框架 V1.0（三级树）

日期：2026-11-16｜状态：Draft；以下是完整规划，不表示已实施。

## 系统整体结构：L1-L8 → 子系统 → 功能
### L1 品牌与商业体系
- 品牌定位
  - 全球跨行业数字科技服务；品牌与其他业务完全独立
  - 网站、App、企业软件、AI、创意、增长与咨询服务
- 产品与服务目录
  - 服务目录 / 子服务 / 定制功能包
  - 标准交付物 / 服务边界 / 能力核验
- 收入与商业模式
  - 项目开发费 / 订阅费 / 维护费
  - 定制报价 / 多币种与税务方案（待合规评估）
- 目标客户与市场
  - 行业细分 / 公司规模 / 区域和语言
  - B2B 直接客户 / 代理商 / 长期企业合同

### L2 公开网站体系
- 网站信息架构
  - Home / Services / Industries / Projects / About
  - Language / Client Login / Start a Project
- 内容与 CMS
  - 服务 / 行业 / 模板 / 案例 / FAQs / 资源
  - 版本 / 审核 / 多语言 / 内链
- 设计与体验
  - 品牌设计系统 / 响应式 / 无障碍
  - Demo / 询盘 CTA / 性能
- 搜索与合规
  - SEO/GEO/AEO / 结构化数据
  - Cookie / Privacy / Terms / 真实声明

### L3 客户与交易体系
- 线索与销售
  - 询盘表单 / AI 需求初审 / CRM
  - 销售分配 / 跟进 / 来源归因
- 需求与方案
  - RFQ / PRD / 范围管理
  - 报价版本 / 人工审批 / 客户确认
- 合同与财务接口
  - 合同 / 里程碑付款 / 发票
  - 订阅 / 续费 / 收款对账
- 客户关系
  - 企业组织 / 多联系人 / 角色
  - 客户门户 / 客户通知 / 沟通历史

### L4 项目交付体系
- 项目启动
  - 项目编号 / 范围 / 时间表
  - 负责人 / 风险 / 变更管理
- 设计与开发
  - UI/UX / 内容 / 前后端
  - 代码评审 / 集成 / 资产管理
- 测试与验收
  - 功能 / 安全 / 性能 / 移动端
  - 客户 UAT / 审批 / 发布回滚
- 交付后服务
  - 账号与源码移交 / 文档
  - 维护 / SLA / 工单 / 续约

### L5 产品与模板体系
- Website & App Templates
  - 行业模板 / 主题与可配置组件
  - 模板预览 / 版本 / 许可范围
- Reusable Business Modules
  - CMS / Auth / RFQ / Booking / Payments
  - CRM / Inventory / Notification Connectors
- AI & Automation Products
  - Chatbot / Knowledge Base / Agent Workflows
  - Prompt & Model Config / Human Handoff
- Demo & Product Catalog
  - Demo 环境 / 试用权限
  - 产品定价 / 版本 / 适用场景

### L6 AI Agent 与自动化体系
- 编排与调度
  - COO / Task IDs / 工作队列
  - Agent 权限边界 / 超时重试 / 失败回退
- 专业 Agent
  - Website / App / Software / Design
  - SEO / Creative / QA / Support / Sales
- 人工审核与安全
  - 客户资料保护 / 审批动作
  - 发布、收费、删除、外发须授权
- 可观测与知识沉淀
  - 执行日志 / 质量评分 / 版本
  - 知识库 / 复盘 / 告警

### L7 中央数据与技术体系
- 数据结构与隔离
  - Organizations / Tenants / Users / Roles
  - Leads / Projects / Quotes / Deliverables / Subscriptions
- 基础设施
  - 前端 / API / 数据库 / 对象存储
  - 代码仓库 / CI-CD / Staging / Production
- 安全与可靠性
  - RBAC / 审计 / 备份恢复 / 秘钥管理
  - 数据分类 / 保留与删除 / 漏洞管理
- 外部集成
  - 支付 / 邮件 / CRM / ERP / AI Providers
  - Webhooks / API Versioning / Rate Limits

### L8 运营与增长体系
- 获客与市场
  - SEO/GEO/AEO / 广告 / 社交 / 伙伴渠道
  - 归因 / 漏斗 / 转化试验
- 客户成功与支持
  - Onboarding / 教程 / 工单
  - 使用情况 / 健康度 / 续费
- 经营分析
  - Pipeline / MRR / 利润 / 毛利
  - 项目效率 / Agent 成本 / SLA
- 治理与持续改进
  - SOP / 质量体系 / 风险
  - 财务核对 / 法律及地区合规评估

## 架构约束
- 本系统仅服务 Samiyah Digital；与所有其他业务独立，不复制其他业务专属菜单或数据。
- 不得默认为已有客户、真实案例、证书、交付规模或自动化功能已经存在。
- 权限范围、租户隔离与审计是开发前提，不可依靠前端隐藏来隔离数据。
- 外部发布、客户消息、资金动作、生产环境变更必须建立审核策略。
- 技术选型尚未确认；不得把规划方案误当成部署事实。

## 交付阶段
1. Phase 1：品牌、官网、核心服务、跨行业演示、项目表单、基础 SEO/法律页面。
2. Phase 2：CRM、报价合同、客户门户、项目交付、维护订阅、客户支持。
3. Phase 3：模板市场、AI Agent 自动交付、多租户软件、白标伙伴与自助服务。

## 对应文件
- 网站信息架构：SD-WEB-001
- 决策基线与变更：DECISIONS.md
