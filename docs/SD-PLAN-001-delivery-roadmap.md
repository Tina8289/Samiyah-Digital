# SD-PLAN-001 · 实施任务与验收路线图 V1.0
日期：2026-11-16｜状态：Draft｜项目归属：仅 Tina8289/Samiyah-Digital

## P0 — 设计与工程准备（当前）
| ID | 任务 | 交付 | 状态 |
|---|---|---|---|
| SD-001 | 审核网站与业务三级架构 | SD-WEB-001 / SD-OS-001 | Draft 已有；待批准 |
| SD-002 | 统一设计系统 | SD-DS-001 | Draft 已有；待批准 |
| SD-003 | 首期页面与转化 PRD | SD-WEB-002 | Draft 已有；待批准 |
| SD-004 | 确认法律主体、品牌、域名 | 决策记录 | 待确认 |
| SD-005 | 选择技术栈/环境/内容管理方案 | ADR + 开发环境 | 未实施 |

## P1 — 公开官网 MVP
| ID | 任务 | 验收条件 |
|---|---|---|
| SD-101 | Header/Footer/Design tokens | 桌面移动及无障碍核对 |
| SD-102 | 首页 | 模块完整、CTA 有效、无虚构数字 |
| SD-103 | Services index + Detail template | 正确读取服务内容，链接正常 |
| SD-104 | Industries index + Detail template | 行业内容独立且互链 |
| SD-105 | Projects + Demo Center | 真实和 Demo 显著区分 |
| SD-106 | About / Contact / Legal | 联系方式与主体核验后发布 |
| SD-107 | Start a Project 表单 | 端到端提交、回读、错误处理和隐私验收 |
| SD-108 | SEO/Accessibility/Performance QA | 正式域名/测试报告与审批 |
| SD-109 | Staging 与生产发布 | 预览验证、回滚、批准后部署 |

## P2 — 商务与客户管理
SD-201 CRM 与 Lead Pipeline；SD-202 报价版本审批；SD-203 项目与客户门户；SD-204 合同、账单和订阅；SD-205 Support Tickets；SD-206 权限和租户隔离测试。
状态：全部规划中，未开发验收。

## P3 — AI 与可复用产品
SD-301 AI Project Consultant；SD-302 Template Library；SD-303 Website/App 专业 Agent；SD-304 独立任务编排与人工批准；SD-305 自助演示/订阅；SD-306 审计、成本和回滚。
状态：全部规划中，未开发验收。

## 发布关卡
- Gate 0：项目仓库与规范确认。
- Gate 1：品牌、设计、页面范围批准。
- Gate 2：代码评审、单元/集成/端到端检查通过。
- Gate 3：无障碍、性能、安全、隐私、案例真实性核验。
- Gate 4：业务负责人批准 staging→production，验证实际网址。
- Gate 5：发布后监控、备份和恢复演练。

## 工作规则
- 任何 Agent/自动化任务必须绑定 Digital 仓库的 Task ID、版本、负责人、审核状态。
- 未经批准不主动创建线上站点、收款、联系客户、部署生产或操作其他业务的数据。
- CEO 仓库仅记录集团层面的里程碑与审计链接；禁止复制此处技术细节过去。
