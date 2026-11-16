# SD-DS-001 · Samiyah Digital 官网设计系统 V1.0
日期：2026-11-16｜状态：Draft / 待设计验收｜归属：Samiyah Digital 独立业务

## 1. 品牌与设计原则
- 品牌：Samiyah Digital；面向全球各行业的数字产品、AI 与企业技术解决方案。
- 参考方向：Clay（视觉与作品展示）＋Netguru（服务信息架构）＋Vention（技术可信度），只学习组织原则，不复制视觉资产、源码、商标、客户案例。
- 视觉关键词：International / Premium / Modern / Clear / Trustworthy / Technology-led。
- 不出现任何其他业务、卫浴产品、其他业务客户权益或赠送措辞；不以某行业为首页主角。
- 首页任何业绩数字、客户 Logo、认证与评价必须有可验证证据；否则隐藏；所有演示明确标注 Demo。

## 2. 视觉 Token（候选，待品牌审核）
| Token | Value | 用途 |
|---|---|---|
| color.navy.950 | #0B1023 | Hero、深色区块 |
| color.navy.900 | #111B39 | 次级深色背景 |
| color.blue.500 | #4967F5 | 主要品牌行动色 |
| color.violet.500 | #8056EA | 渐变辅助，不用作大段正文 |
| color.surface | #FFFFFF | 内容主背景 |
| color.surface.soft | #F6F8FC | 卡片与交错区块 |
| color.text.primary | #172033 | 浅色背景正文 |
| color.text.inverse | #FFFFFF | 深色背景正文 |
| color.text.muted | #5C677B | 辅助正文 |
| color.border | #DFE5EF | 卡片与分割线 |
| radius.card | 20px | 卡片 |
| radius.button | 12px | CTA |
| container.max | 1200px | 桌面内容主宽 |
| spacing.section.desktop | 96px | 主要区块间距 |
| spacing.section.mobile | 56px | 手机端区块间距 |

色彩对比度必须在实际页面验收，文本目标 WCAG AA；不得以设计稿视觉替代可访问性测试。

## 3. 字体与排版
- 英文首选 Inter（获许可、优化加载）；中文回退使用系统中文无衬线字体；不分散加载大量字重。
- 仅一个 H1；H2、H3 按语义组织；正文桌面建议 16–18px，移动端 16px 起。
- Hero 主标题建议 52–68px 桌面、34–42px 手机；限制每行字符宽度。
- 按钮文案用明确动作：Explore Services、View Demo、Start a Project、Contact Sales。

## 4. 响应式
- 手机 <768px：单列 Hero，导航折叠，卡片 1 列，CTA 不溢出；触控目标≥44px。
- 平板 768–1023px：2 列卡片；导航折叠或受控适配。
- 桌面≥1024px：Hero 左文字右产品界面，核心服务 3 列，行业卡 3–4 列。
- 禁止横向滚动、低对比图中文字、移动端图片压住 CTA。

## 5. 组件清单（先做）
- Header / MobileMenu / LanguageSwitcher / ProjectCTA
- Hero / ServiceCard / IndustryCard / CaseStudyCard / DemoCard
- Logo/Trust area（未验证数据时不渲染客户 Logo）
- ProcessSteps / FAQAccordion / Testimonial（仅真实内容）
- LeadForm / FileUpload（上传类型与容量需校验）/ Footer / CookieControls
- Loading / Empty / Error / Success 状态；键盘焦点与表单错误提示

## 6. 内容与图片规范
- 优先用自有或已许可的数字产品、UI、工作场景视觉；禁止以卫浴作为示例。
- 默认 WebP/AVIF，保持尺寸和 responsive srcset，首屏主视觉做预加载策略评审。
- 禁止假客户案例、虚构 KPI、未经授权品牌 Logo；原型以 Demo / Concept 标记。
- 所有图像需要实际内容相关的 alt；纯装饰图使用空 alt。

## 7. 页面性能与 SEO 设计验收
- Core Web Vitals 参考目标：LCP≤2.5s、INP≤200ms、CLS≤0.1（在真实用户和合适分位数验证）。
- 语义 HTML、可访问导航、唯一 URL、canonical、sitemap、robots、metadata；具体实施后验证。
- 页面出站动作、语言切换、联系表单的事件跟踪需获取适当同意；不得无同意采集不必要个人信息。

## 8. 设计交付与审核门槛
1. 桌面/手机首页高保真稿。
2. 服务详情页、行业详情页和案例页模板。
3. 组件 Token、交互状态、空/错/成功状态。
4. 真实数据与 Demo 内容分离；移动端、键盘、对比度、性能审查。
5. CEO 确认设计稿后才进入生产发布。
