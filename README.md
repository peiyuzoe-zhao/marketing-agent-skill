
# Marketing Agent — WPP Open × CoreAI 混合架构

酒水行业 AI 营销策略引擎。Hermes Agent Skill。

## 版本

v2.0.0

## 架构

WPP Open（模块化平台）× Publicis CoreAI（数据驱动引擎）。

## 能力概览

| 层级 | 内容 |
|------|------|
| **10 个核心模块** | M0 市场洞察 / M1 品牌概念 / M2 营销模型 / M3 外部事件 / M4 媒介传播 / M5 线下门店 / M6 线下活动 / M7 品类创造 / M8 销售赋能 / M10 产品策略 |
| **7 个工作流** | 年度规划 / Campaign 编排 / 投流异常升级 / 竞品信号分级 / 销售回传→策略迭代 / 新品上市全链路 / 异常诊断→深挖 |
| **4 个横切层** | 利益相关方地图 / 度量归因体系 / ESG 框架 / 年度营销日历 |
| **16 个输出模板** | 品牌定位方案 / Campaign Brief / 投流方案 / 品鉴会方案 / 热点评估报告 / 月度复盘 / 经销商大会方案 / 新闻稿 / 媒体 Q&A / Fact Sheet / Pitch 邮件 / 危机声明 / 媒体监测 / 品牌健康度仪表盘 / Agency Brief / Brand Book |
| **8 种工作模式** | 策略推演 / 知识查询 / 事件管理 / 媒介传播 / 终端诊断 / 活动策划 / 内容生成 / 品类创造 |
| **品牌安全** | 敏感词库 + 自动审查规则 |
| **品类创造** | 6 元问题 + 心智锚点矩阵 + Phase 1.5 消费者验证 |

## 安装

```bash
# 解压到 Hermes skills 目录
tar -xzf marketing-agent-skill-v2.0.tar.gz -C ~/.hermes/skills/marketing/

# 重新加载 skills
/reload-skills
```

或通过 Hermes Hub 安装（发布后）：

```bash
hermes skills install marketing-agent
```

## 使用示例

```
"帮我做一个中端白酒品牌的年度规划"
"这个新品类该怎么定义和命名"
"投流 CPA 突然涨了 50%，帮我诊断"
"竞品在华东降价 15%，我要不要跟"
"帮我写一份品鉴会的邀请函"
"生成一份完整的 Brand Book"
```

## 文件结构

```
SKILL.md                    — 主入口（策略框架 + 工作流 + 路由）
references/
├── brand-concepts.md       — 品牌定义/定位/原型/定价/语调/使命
├── marketing-models.md     — 18 个模型 + 竞争/归因/资源分配
├── trending-events.md      — 热点匹配 + 危机预备 + 品牌安全审查
├── ad-placement.md         — paid/earned/owned 媒介策略
├── offline-retail.md       — 门店管理 + 经销商谈判
├── offline-events.md       — 活动策划 + 赞助评估
├── category-creation.md    — 品类创造 6 元问题
├── sales-enablement.md     — 销售赋能（话术/工具包/培训）
├── market-insights.md      — 5C 分析 + 竞品分层 + 消费者洞察
├── product-strategy.md     — 产品线规划 + 新品上市 + 包装策略
├── alcohol-industry.md     — 酒水行业知识 + 媒体生态 + ESG
├── content-generation.md   — 内容生成模板
└── output-templates.md     — 16 个交付物标准模板
```

## 适用场景

- 酒水行业品牌策略与定位
- 全新品类从零到一的品牌体系建设
- 投流诊断与 ROI 优化
- 线下门店动销管理
- 经销商政策设计与谈判
- 营销 Campaign 全链路策划
- 热点营销评估
- 危机预备
- 品牌安全审查

## 设计哲学

深度问题用深度框架（Peiyu 协议营销版），速度问题用快速框架，执行问题用模板。不猜测用户意图——先锚定再分析。
