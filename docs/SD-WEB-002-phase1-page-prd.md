# SD-WEB-002 · 官网 Phase 1 页面与转化 PRD V1.0
日期：2026-11-16｜状态：Draft / 规划建议｜适用：Samiyah Digital

## 0. 目标与边界
交付一个可信、国际化、面向全球所有行业的数字科技官网，便于了解服务、查看 Demo、提交项目需求。此阶段不声称客户门户、支付、AI 自动交付已上线，不暗示任何免费或其他业务特殊权益。

## 1. 顶部信息架构（已确认）
Home / Services / Industries / Projects / About
右侧：Language / Client Login / Start a Project。
在 Client Portal 开发前，Client Login 应明确展示“尚未开放”或隐藏入口，禁止死链与虚假登录。
Pricing、Resources、Partners、Security、Contact 从二级页面及 Footer 可到达，不增加主导航。

## 2. 首页模块和目的
| 顺序 | 模块 | 必备内容 | CTA |
|---|---|---|---|
| 01 | Hero | Digital Solutions for Every Industry；网站、App、AI、软件价值主张 | Explore Services / Start a Project |
| 02 | Core Services | Website、App、Business Software、AI Solutions、Creative Studio、Digital Marketing | View Service |
| 03 | Industries | Manufacturing、Retail、Wholesale、Hospitality、Healthcare、Real Estate 等跨行业入口 | Explore Industry |
| 04 | Featured Projects & Demos | 真实案例优先；无真实案例只放显著 Demo 标注 | View Demo |
| 05 | Why Choose Us | 流程、透明交付、技术能力，避免未经验证的奖项和数据 | How We Work |
| 06 | AI & Integration | AI Agent、自动化、系统集成的具体使用场景 | Explore AI |
| 07 | How We Work | Discover → Plan → Design → Build → QA → Launch → Support | Start a Project |
| 08 | Engagement Options | Fixed-scope Project / Custom Development / Managed Service；价格待核定 | Request Proposal |
| 09 | Insights / FAQ | 可验证内容、常见采购顾虑 | Read More |
| 10 | Final CTA | 项目咨询表单入口 + 合法联系方式 | Start a Project |

## 3. 页面模板
### 3.1 Services index /services
- 6 个一级服务卡片为首页展示入口；详细目录可扩展为 8–12 类。
- 支持分类介绍、典型成果、服务详情链接、行业关联与 FAQ。
### 3.2 Service details /services/:slug
- Hero、适用客户、功能/交付范围、技术能力（只展示已核实支持）、演示/作品、开发流程、常见问题、咨询 CTA。
- 一个主关键词，相关子关键词，自然内链，不堆词。
### 3.3 Industries /industries 与 /industries/:slug
- 每个行业写业务痛点 → 适用服务 → 演示 → 典型流程 → 联系入口；避免同文改行业名批量复制。
### 3.4 Projects /projects 与 /projects/:slug
- 标签：Real Project（有授权与证据）或 Demo / Concept。
- 案例字段：行业、问题、交付范围、技术、效果（如可验证）、截图版权、发布日期、状态。
### 3.5 About /about
- 定位、合法主体待确认的信息占位、交付流程、安全承诺的实际边界、Contact。
### 3.6 Start Project /start-project
- 流程：服务→行业/规模→需求→预算区间（可跳过）→资料附件→联系人→同意及提交。
- 形成唯一 Lead ID、后端校验、反垃圾机制、隐私告知、失败重试和防重复提交；不得向公共日志输出完整联系资料。
- 正式发信、写 CRM、存储附件需对外部集成做权限与隐私验收。
### 3.7 Footer & trust
- Contact、Pricing（咨询型）、Resources、Partners、Privacy、Terms、Security；未完成的页面不应展示为可用链接。

## 4. 多语言策略
- Phase 1 英文主站；语言切换只有在目标语言页面真正存在时才出现可用选项。
- 采用国际化路由规划；hreflang、canonical 与语言版本实际 URL 一一对应，不生成空页面。

## 5. 内容数据模型（概念，不等于已建数据库）
- Service(id, slug, title, summary, status, category, seo, updated)
- Industry(id, slug, painPoints, solutionRefs, status, seo)
- Project(id, slug, labelRealOrDemo, evidence, industryRefs, serviceRefs, mediaRights)
- FAQ(id, relatedPage, question, answer)
- Lead(id, organization, serviceRefs, requirements, contact, consent, source, state)
- Media(id, owner, usageRights, alt, variants)
- PageRevision(id, entity, version, reviewer, approval, publishedAt)

## 6. 阶段验收
- 五主导航及移动菜单功能正常；Footer 无死链。
- 关键模板英文内容完整，无单一行业主视觉，无其他业务交叉权益。
- 每张 CTA 可走通实际目标；提交表单可成功并在授权环境回读，错误态可恢复。
- 真案例证据/授权可查；Demo 标签清楚；不含虚构合作、成绩和认证。
- SEO metadata、索引、sitemap、canonical、移动性能、无障碍基础检查通过。
- 测试与负责人审批记录保存在 Digital 仓库；未通过不得标注上线。
