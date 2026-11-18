# GitHub Vibe Coding 技能调研

核对日期：2026-11-16。通过 GitHub 仓库首页、原始 README 和下列实际 `SKILL.md` 阅读比对。推荐按适用性、可组合性、验证机制与宿主依赖判断；没有按 Star 数量排序，也没有对第三方技能做安装或运行基准。

## 推荐清单

| 仓库 | 类型与适合场景 | 阅读到的依据 | 选择时的限制 |
|---|---|---|---|
| [mattpocock/skills](https://github.com/mattpocock/skills) | 可组合工程技能；适合需求不清、任务分解、调试和交接 | README；`grilling`、`grill-me`、`diagnosing-bugs`、`to-tickets`、`handoff` | 一些入口依赖其他技能和项目初始化；当前 `grilling` 会一轮提多个可问问题，`to-tickets` 可发布外部工单，不宜无范围直接照搬 |
| [obra/superpowers](https://github.com/obra/superpowers) | 较完整开发流程；适合希望统一规划、开发、调试和审查的项目 | README；`brainstorming`、`systematic-debugging` | 流程较强，包含设计批准与后续技能调用；README 描述多代理路径，与其他流程同时启用需要处理重叠 |
| [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | 文件化任务规划；适合跨会话研究、长开发任务 | README；`planning-with-files/SKILL.md` | 当前版本含生命周期 hooks 和任务目录选择逻辑，单独复制正文不等于完整恢复能力；小修改未必需要 |
| [anthropics/skills → frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | 界面视觉专项；适合缺少设计方向的新页面 | 具体 `frontend-design/SKILL.md` | 视觉指导不能替代需求、数据和业务验收；已有品牌与设计系统优先 |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | 框架与界面专项；适合 React／Next.js 性能、交互与可访问性检查 | README；`web-design-guidelines/SKILL.md` | React 性能规则有技术栈前提；界面检查技能会获取远程最新规则，离线能力不同于静态技能 |
| [arty-kk/vibe-coding](https://github.com/arty-kk/vibe-coding) | 直接以 Vibe Coding 命名的工作流库；适合按映射、任务、评审、修复等选择入口 | README；`vibe-task/SKILL.md` | 包含本地插件与可选远程 MCP 两种路径；不是一个孤立的万能提示词，需区分所选分发形式 |

**对这次个人中文技能的建议：**以本地 `vibe-coding` 作为统一入口，保留轻量引导；需要专项能力时优先挑 Matt Pocock 的相关模块。偏重前端时再选择 `frontend-design`，长任务确实容易断上下文时再考虑文件规划。Superpowers 适合明确希望采用一整套流程时使用。这个组合建议是基于阅读的判断，不是对效果的实测排名。

## 具体原文入口

- Superpowers：[README](https://github.com/obra/superpowers/blob/main/README.md)、[brainstorming](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md)、[systematic-debugging](https://github.com/obra/superpowers/blob/main/skills/systematic-debugging/SKILL.md)。
- Matt Pocock：[README](https://github.com/mattpocock/skills/blob/main/README.md)、[grilling](https://github.com/mattpocock/skills/blob/main/skills/productivity/grilling/SKILL.md)、[diagnosing-bugs](https://github.com/mattpocock/skills/blob/main/skills/engineering/diagnosing-bugs/SKILL.md)、[to-tickets](https://github.com/mattpocock/skills/blob/main/skills/engineering/to-tickets/SKILL.md)、[handoff](https://github.com/mattpocock/skills/blob/main/skills/productivity/handoff/SKILL.md)。
- Planning with Files：[README](https://github.com/OthmanAdi/planning-with-files/blob/master/README.md)、[SKILL.md](https://github.com/OthmanAdi/planning-with-files/blob/master/skills/planning-with-files/SKILL.md)。
- Anthropic：[frontend-design](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md)。
- Vercel：[README](https://github.com/vercel-labs/agent-skills/blob/main/README.md)、[web-design-guidelines](https://github.com/vercel-labs/agent-skills/blob/main/skills/web-design-guidelines/SKILL.md)。
- Arty：[README](https://github.com/arty-kk/vibe-coding/blob/main/README.md)、[vibe-task](https://github.com/arty-kk/vibe-coding/blob/main/plugins/vibe-coding/skills/vibe-task/SKILL.md)。

这些是可变分支链接，本次未取得用于固定审计的 GitHub API 提交快照，不把链接视为不可变版本。安装时应再查看当前原仓库文档、依赖和具体文件；本次没有执行文章中的第三方安装命令，也没有安装推荐列表。

## 额外发现

[gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) 的仓库首页在本次读取时显示于 2026-06-26 归档。它可作为规范与上下文工程的历史参考；不把搜索结果里的发布说明直接作为当前可维护安装方案。若选择该体系，需要继续核对维护去向。

## 本版实际采纳与未采纳

采纳：目标对齐、纵向任务、短反馈回路、按证据结束、最少上下文落盘、按场景加载。

未采纳：强制大问卷、所有任务先写完整 PRD、逐步审批、全任务 TDD、多代理默认启用、自动发 Issues、远程 MCP 默认连接、全局 hooks 与无上限的修复循环。

本地技能自包含，可单独工作；推荐清单用于选型，没有形成安装依赖。
