# 深度思考与认知工作法套件 (Thinking Toolkit ZH)

> 基于"数字生命卡兹克"沉淀的 12 个核心思维与决策框架重构，兼容 **CodeBuddy、Claude Code 与 Codex** 插件规范。
> 专为中文用户打造，原生支持自然语言意图激活、渐进式加载（Progressive Disclosure）与多轮对话状态机。

> **致谢**：本套件基于 [数字生命卡兹克] 沉淀的思维框架重构。感谢原作对核心认知与决策方法论的整理与分享。

---

## 🚀 安装与使用

| 平台 | 支持方式 |
| --- | --- |
| CodeBuddy / WorkBuddy | `.codebuddy-plugin/plugin.json` |
| Claude Code | `.claude-plugin/plugin.json` 与 Claude Marketplace |
| Codex | `.codex-plugin/plugin.json` 与仓库级 Codex Marketplace |

### Codex：从 GitHub 安装

```bash
codex plugin marketplace add Winsaney/thinking-toolkit-zh
codex plugin add thinking-toolkit-zh@thinking-toolkit-zh
```

安装后重启 Codex 或开启一个新任务，使新 Skill 进入上下文。

### Codex：本地开发安装

Clone 仓库后，将绝对路径注册为本地 Marketplace，再安装插件：

```bash
codex plugin marketplace add /absolute/path/to/thinking-toolkit-zh
codex plugin add thinking-toolkit-zh@thinking-toolkit-zh
```

更新本地插件后，移除已缓存版本并重新安装：

```bash
codex plugin remove thinking-toolkit-zh@thinking-toolkit-zh
codex plugin add thinking-toolkit-zh@thinking-toolkit-zh
```

从 GitHub 安装的用户可先刷新远程 Marketplace，再重新安装：

```bash
codex plugin marketplace upgrade thinking-toolkit-zh
codex plugin add thinking-toolkit-zh@thinking-toolkit-zh
```

卸载插件和 Marketplace：

```bash
codex plugin remove thinking-toolkit-zh@thinking-toolkit-zh
codex plugin marketplace remove thinking-toolkit-zh
```

### CodeBuddy / WorkBuddy

将此目录放置于项目（`.workbuddy/plugins/`）或系统全局配置目录（`~/.workbuddy/plugins/`）即可自动生效。

在与 Agent 对话时直接用自然语言描述需求（如"帮我双层解释这个概念"、"挖掘我的天赋"），Agent 将按需自动激活对应 Skill。

---

## 🌟 核心场景与 12 大思维框架

### 一、问清问题
- **[苏格拉底式提问](./skills/苏格拉底式提问/SKILL.md)**：通过最多 6 轮单问单答问诊，剥离伪需求与假设，帮你找到真正值得回答的真问题。
  - *触发示例*："我对这个事很困惑，帮我做一次苏格拉底式问诊"、"帮我把这个问题想清楚"。

### 二、学习与深度研究
- **[双层解释法](./skills/双层解释法/SKILL.md)**：小白版生活化类比 + 专家版底层机制与适用边界，附带理解自测题。
  - *触发示例*："这个技术名词我完全听不懂，用双层解释法帮我讲讲"。
- **[反向拆解](./skills/反向拆解/SKILL.md)**：拆解优秀作品/案例，剖析结构流程、拉开质量差距的关键选择与可复用规律。
  - *触发示例*："帮我反向拆解这个优秀产品/网页/方案"。
- **[横纵分析法](./skills/横纵分析法/SKILL.md)**：纵轴看历史演化与路径依赖，横轴看竞品对比，推演未来 3 条路径，生成万字研报。
  - *触发示例*："对[某技术/公司/行业]做一次横纵深度分析"。
- **[事实核查](./skills/事实核查/SKILL.md)**：拆解事实/推论/价值判断，联网核查信源，审计推理漏洞并输出补强版本。
  - *触发示例*："核查这个说法/文章是真的吗"、"帮我做事实核查与论证审计"。

### 三、解决问题
- **[专家会诊](./skills/专家会诊/SKILL.md)**：组建 3 种互补视角的专家团，让不同视角互相质疑，挖掘分歧背后的隐藏假设与退出条件。
  - *触发示例*："帮我针对这个难题做一次跨视角专家会诊"。
- **[第一性原理](./skills/第一性原理/SKILL.md)**：推倒重来，剥离表面修补，从无法绕开的基本事实、目标与约束推导底层新路径。
  - *触发示例*："用第一性原理重新拆解这个架构/流程"。
- **[跨领域借解](./skills/跨领域借解/SKILL.md)**：抽象核心矛盾，从 3 个遥远领域调取成熟解法机制，转化为当前处境的低成本可逆方案。
  - *触发示例*："跨领域借鉴思路，看看其他行业怎么解决这个问题的"。

### 四、决策
- **[双向钢人论证](./skills/双向钢人论证/SKILL.md)**：为两个互斥选项分别建立最强辩护，找出核心分歧变量，提问 1 个关键决胜问题。
  - *触发示例*："我在方案 A 和方案 B 之间纠结，帮我做双向钢人论证"。
- **[用最小实验替代空想](./skills/用最小实验替代空想/SKILL.md)**：提炼最核心的未验证假设，设计 7 天内低成本、可逆的最小验证实验。
  - *触发示例*："纸上谈兵没用了，帮我设计一个最小实验"。

### 五、认识自己
- **[挖掘隐藏天赋](./skills/挖掘隐藏天赋/SKILL.md)**：融合盖洛普/心流/荣格心理学，4 条主线多轮深度追问，生成万字《个人天赋使用说明书》。
  - *触发示例*："挖掘我的隐藏天赋"、"帮我梳理我的底层天赋与能量地图"。
- **[人生设计术](./skills/人生设计术/SKILL.md)**：基于斯坦福人生设计方法，4 维仪表盘 + 正北指南针 + 3 个五年奥德赛计划 + 原型行动。
  - *触发示例*："帮我做一次斯坦福人生设计"、"规划未来 5 年的可能路径"。

---

## 📦 目录结构

```
thinking-toolkit-zh/
├── .agents/plugins/
│   └── marketplace.json         ← Codex 仓库 Marketplace 清单
├── .codex-plugin/
│   └── plugin.json              ← Codex 插件清单与展示元数据
├── .codebuddy-plugin/
│   └── plugin.json              ← 插件清单（name/version/12个skill路径）
├── .claude-plugin/
│   ├── plugin.json              ← Claude Code 插件清单
│   └── marketplace.json         ← Claude Marketplace 清单
├── SKILL.md                     ← 聚合套件入口（索引12个skill + 五大场景导航）
├── README.md                    ← 用户文档（场景/触发示例）
├── LICENSE                      ← MIT 许可证
├── CHANGELOG.md                 ← 版本变更记录
├── .gitignore
├── rules/
│   └── AGENTS.md                ← 全局交互规则（4条硬约束）
└── skills/                      ← 12 个独立 skill 目录
    ├── 苏格拉底式提问/SKILL.md
    ├── 双层解释法/SKILL.md
    ├── 反向拆解/SKILL.md
    ├── 横纵分析法/SKILL.md
    ├── 事实核查/SKILL.md
    ├── 专家会诊/SKILL.md
    ├── 第一性原理/SKILL.md
    ├── 跨领域借解/SKILL.md
    ├── 双向钢人论证/SKILL.md
    ├── 用最小实验替代空想/SKILL.md
    ├── 挖掘隐藏天赋/SKILL.md
    └── 人生设计术/
        ├── SKILL.md
        └── references/          ← 参考文档子目录
            ├── gravity_vs_real_problem.md
            └── odyssey_plan_guide.md
```

---

## 📜 许可证

[MIT](./LICENSE) — 自由使用、修改与分发。
