# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/lang/zh-CN/).

## [1.1.0] - 2026-08-24

### Added

- 新增 `.codex-plugin/plugin.json`，支持 Codex 与 ChatGPT 插件加载
- 新增 `.agents/plugins/marketplace.json`，支持从 GitHub 或本地仓库安装 Codex 插件

### Changed

- CodeBuddy、Claude Code 与 Codex 插件清单版本统一升级至 1.1.0
- 移除聚合 `SKILL.md` 中 Codex 不支持的 `version` frontmatter 字段
- 事实核查与横纵分析改用宿主无关的联网工具表述
- README 增加三平台支持矩阵及 Codex 安装、升级与卸载说明

## [1.0.0] - 2026-08-21

### Added

- 初始发布版本
- 12 个核心思维与决策框架 Skill，覆盖五大场景：
  - **问清问题**：苏格拉底式提问
  - **学习与深度研究**：双层解释法、反向拆解、横纵分析法、事实核查
  - **解决问题**：专家会诊、第一性原理、跨领域借解
  - **理性决策**：双向钢人论证、用最小实验替代空想
  - **认识自己**：挖掘隐藏天赋、人生设计术
- 聚合套件入口 `SKILL.md`，提供五大场景导航与全局路由
- 全局交互规则 `rules/AGENTS.md`，定义 4 条硬约束：
  - 渐进式多轮状态机（严格单问单答）
  - 区分事实、解释与价值判断
  - 拒绝空洞赞美，保持敏锐洞察
  - 证据标注与工具调度原则
- 人生设计术 Skill 附带 `references/` 参考文档：
  - `gravity_vs_real_problem.md`（重力问题 vs 真问题）
  - `odyssey_plan_guide.md`（奥德赛计划指南）
- 遵循 Agent Plugins 规范 v1.0.0
- MIT 许可证

### Acknowledgements

基于 [数字生命卡兹克] 沉淀的思维框架重构。感谢原作对核心认知与决策方法论的整理与分享。
