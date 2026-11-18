# 资料来源与设计取舍

整理日期：2026-11-16。以下资料用于提炼方法，不是运行时依赖；本技能的指令为重新编写，未复制第三方技能包、脚本或 hooks。

## 用户提供资料中的主要启发

- [PRD 与 Skills 生成 UI](https://active.blog.csdn.net/article/details/164121145)：将需求、界面实现与预览检查连起来；示例技术栈和技能名不照搬。
- [Matt Pocock 技能介绍](https://post.smzdm.com/p/a032zk7w/)与[全栈 Skills 清单](https://blog.csdn.net/2301_76711398/article/details/162277123)：提供候选工具线索，具体能力再查仓库。
- [工程化实践](https://blog.csdn.net/weixin_29056701/article/details/170479192)：沿用项目上下文与既有代码模式，明确输入、输出和验证。文章示例中的业务遗漏不能因风格合规而忽略。
- [设计师从 PRD 到交互页面](https://cloud.tencent.com/developer/article/2700065)：优先使用已有设计系统，把演示界面和真实接入区分开。
- [Rules 与 Skills](https://tianqi.csdn.net/6a48a813662f9a54cb89b8e2.html)：项目事实与专项流程分开维护；不移植文章的通用优先级、价格或自定义元数据字段。
- [Skills 最佳实践](https://artisan.blog.csdn.net/article/details/157946178)：明确触发、按需参考、验证及停止条件。
- [平台适配评估](https://blog.csdn.net/weixin_42554042/article/details/170380651)：只采用“核对实际运行能力与输入输出”的思路；未核验的平台、私有 SDK、比例和性能结论不写入指令。
- [常用 Skills 介绍](https://cloud.tencent.com/developer/article/2656568)：补充规划、界面与调试的检索线索；不继承营销表述。

## 核对过的 GitHub 原始资料

| 来源 | 本版采纳的思路 | 按本技能范围调整 |
|---|---|---|
| [Superpowers](https://github.com/obra/superpowers) | 先理解目标、调查根因、完成前验证 | 不移植每阶段批准、全任务 TDD 或多代理强制流程 |
| [Matt Pocock Skills](https://github.com/mattpocock/skills) | 可验收的纵向任务、紧凑调试回路、交接 | 需求逐步问；不自动创建外部 Issues 或启动初始化配置 |
| [Planning with Files](https://github.com/OthmanAdi/planning-with-files) | 进度落盘与会话恢复 | 只在需要时落盘，不附带 hooks 或读取历史聊天脚本 |
| [Anthropic frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | 与产品内容匹配的视觉方向 | 已有设计系统优先，不因技能偏好重设计产品 |
| [Vercel Agent Skills](https://github.com/vercel-labs/agent-skills) | 界面与交互的具体验证项 | 仅在相关技术栈与需求中使用，不绑定 Vercel |
| [arty-kk/vibe-coding](https://github.com/arty-kk/vibe-coding) | 从已有输入进入合适步骤、以证据判定完成 | 保持离线、自包含，不自动连接其 MCP 服务 |

用户提供的 3 篇知乎、2 篇百家号，以及 `IManiy/161858545` 的 CSDN 文章未取得正文；不能声称已综合这些未读内容。逐链接访问结果与纠错见 [资料研究与整合](资料研究与整合.md)，推荐依据见 [GitHub 技能调研](GitHub技能调研.md)。这些文档随分发包提供，不参与运行时技能加载。
