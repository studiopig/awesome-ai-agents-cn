# 🤖 Awesome AI Agents (CN)

> 中文 AI Agent 资源精选列表 — 框架、工具、论文、教程、社区
> 
> A curated list of AI Agent resources with Chinese-language focus.
> 
| [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
| [![Stars](https://img.shields.io/github/stars/studiopig/awesome-ai-agents-cn?style=social)](https://github.com/studiopig/awesome-ai-agents-cn)

> 📅 最后更新：2026-06-05 | ⚠️ Star 数和成熟度评分可能已变化，以各项目主页为准

---

## 📋 目录

- [Agent 框架](#-agent-框架)
- [MCP 生态](#-mcp-生态)
- [Coding Agent](#-coding-agent)
- [浏览器 Agent](#-浏览器-agent)
- [多 Agent 编排](#-多-agent-编排)
- [Agent 记忆与上下文](#-agent-记忆与上下文)
- [Agent 评测](#-agent-评测)
- [开源 Agent 产品](#-开源-agent-产品)
- [论文精选](#-论文精选)
- [教程与课程](#-教程与课程)
- [中文社区](#-中文社区)
- [贡献指南](#-贡献指南)

---

## 📊 评分标准

每个项目标注三项指标，帮助快速评估：

| 指标 | 选项 | 说明 |
|------|------|------|
| 🏷️ **成熟度** | 🟢 稳定 · 🟡 Beta · 🔴 实验 | 生产就绪程度。🟢=有稳定 release/大厂维护 |
| 🌏 **中文支持** | ●●● 完整 · ●● 部分 · ● 极少 | 中文文档/社区/模型兼容性 |
| 📜 **协议** | MIT · Apache-2.0 · 自定义 | 开源协议类型 |

> 💡 评分基于公开信息，有偏差请提 PR 更正。

---

## 🏗 Agent 框架

*Frameworks for building AI agents.*

> **怎么选：** 刚接触 Agent 开发？从 **LangGraph** 或 **CrewAI** 入门——文档最全、中文资料最多。需要生产级稳定性和多 Agent 协作？看 **AutoGen**（微软）或 **Dify**（国产全栈）。追求极简和可控？**MetaGPT** 模拟软件公司流程，**Smolagents** 轻到只有几个文件。如果你已经用 OpenAI/Gemini API，直接用官方 SDK 最省事。

| 项目 | Stars | 成熟度 | 中文 | 协议 | 描述 |
|------|-------|:------:|:----:|:----:|------|
| [LangGraph](https://github.com/langchain-ai/langgraph) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langgraph?style=flat) | 🟢 | ●● | MIT | 有向图编排 Agent 工作流，LangChain 出品 |
| [CrewAI](https://github.com/crewAIInc/crewAI) | ![Stars](https://img.shields.io/github/stars/crewAIInc/crewAI?style=flat) | 🟢 | ●● | MIT | 角色化多 Agent 协作框架 |
| [AutoGen](https://github.com/microsoft/autogen) | ![Stars](https://img.shields.io/github/stars/microsoft/autogen?style=flat) | 🟢 | ●● | MIT | 微软多 Agent 对话框架 |
| [MetaGPT](https://github.com/FoundationAgents/MetaGPT) | ![Stars](https://img.shields.io/github/stars/FoundationAgents/MetaGPT?style=flat) | 🟡 | ●●● | MIT | 模拟软件公司的多 Agent 协作（国产） |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | ![Stars](https://img.shields.io/github/stars/openai/openai-agents-python?style=flat) | 🟢 | ● | Apache-2.0 | OpenAI 官方 Agent SDK |
| [Google ADK](https://github.com/google/adk-python) | ![Stars](https://img.shields.io/github/stars/google/adk-python?style=flat) | 🟡 | ● | Apache-2.0 | Google Agent Development Kit |
| [Dify](https://github.com/langgenius/dify) | ![Stars](https://img.shields.io/github/stars/langgenius/dify?style=flat) | 🟢 | ●●● | Apache-2.0 | 开源 LLM 应用开发平台（国产） |
| [Smolagents](https://github.com/huggingface/smolagents) | ![Stars](https://img.shields.io/github/stars/huggingface/smolagents?style=flat) | 🟡 | ● | Apache-2.0 | HuggingFace 轻量 Code Agent |
| [Mastra](https://github.com/mastra-ai/mastra) | ![Stars](https://img.shields.io/github/stars/mastra-ai/mastra?style=flat) | 🟡 | ● | MIT | TypeScript 原生 Agent 框架 |

---

## 🔌 MCP 生态

*Model Context Protocol — AI Agent 的工具标准协议。*

> **怎么选：** 先看 **MCP 官方 SDK**——Python 和 TypeScript 都有，五分钟能跑通。需要现成的工具？从官方 Servers 仓库挑——文件系统、GitHub、数据库都是开箱即用。做多工具整合去 **MCP Market** 或 **Smithery** 搜现成的。

### MCP 官方资源
- [MCP 规范](https://modelcontextprotocol.io/) — 官方协议文档
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) — Python 实现
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) — TypeScript 实现

### 热门 MCP Server

| 项目 | 描述 |
|------|------|
| [mcp-server-browser](https://github.com/modelcontextprotocol/servers) | 浏览器自动化 |
| [mcp-server-filesystem](https://github.com/modelcontextprotocol/servers) | 文件系统操作 |
| [mcp-server-github](https://github.com/modelcontextprotocol/servers) | GitHub API |
| [mcp-server-postgres](https://github.com/modelcontextprotocol/servers) | 数据库查询 |
| [mcp-server-fetch](https://github.com/modelcontextprotocol/servers) | HTTP 请求 |
| [WebMCP](https://github.com/anomalyco/webmcp) | 通用浏览器 MCP 标准 |

### MCP 聚合平台
- [MCP Market](https://mcp.so/) — MCP Server 应用商店
- [Smithery](https://smithery.ai/) — MCP Server 托管平台
- [OpenMCP](https://openmcp.io/) — MCP 市场与聚合

---

## 💻 Coding Agent

*AI 编程助手与自主开发 Agent。*

> **怎么选：** VS Code 用户首选 **Cline** 或 **Continue**——直接装插件，零配置。终端党用 **Aider**（结对编程）或 **Codex CLI**（全自动）。需要完整自主开发能力（写PR、修Bug、部署）看 **OpenHands**。想试试"AI 软件工程师"完整体验的看 **Devin**。

| 项目 | Stars | 成熟度 | 中文 | 描述 |
|------|-------|:------:|:----:|------|
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | ![Stars](https://img.shields.io/github/stars/All-Hands-AI/OpenHands?style=flat) | 🟢 | ●● | 全栈自主编程 Agent |
| [Cline](https://github.com/cline/cline) | ![Stars](https://img.shields.io/github/stars/cline/cline?style=flat) | 🟢 | ●● | VS Code 内 AI 编程助手 |
| [Codex CLI](https://github.com/openai/codex) | ![Stars](https://img.shields.io/github/stars/openai/codex?style=flat) | 🟢 | ● | OpenAI 终端编程 Agent |
| [Continue](https://github.com/continuedev/continue) | ![Stars](https://img.shields.io/github/stars/continuedev/continue?style=flat) | 🟢 | ●● | 开源 AI 代码助手 |
| [Aider](https://github.com/Aider-AI/aider) | ![Stars](https://img.shields.io/github/stars/Aider-AI/aider?style=flat) | 🟢 | ● | 终端 AI 结对编程 |
| [OpenCode](https://github.com/anomalyco/opencode) | ![Stars](https://img.shields.io/github/stars/anomalyco/opencode?style=flat) | 🟡 | ● | 开源编程 CLI Agent |
| [Devin](https://github.com/cognition-labs/devin) | 🔒 私有 | 🟡 | ● | 首个 AI 软件工程师 |

---

## 🌐 浏览器 Agent

*Web 自动化与自主浏览 Agent。*

> **怎么选：** 做网页数据提取或表单填写？**Browser Use** 最成熟。需要 MCP 协议兼容？**Playwright MCP** 微软官方出品。做轻量网页操作看 **Stagehand**（自然语言驱动）。

| 项目 | 描述 |
|------|------|
| [Browser Use](https://github.com/browser-use/browser-use) | AI Agent 浏览器自动化框架 |
| [Playwright MCP](https://github.com/microsoft/playwright-mcp) | 微软 Playwright MCP Server |
| [Agent Browser](https://github.com/vercel-labs/agent-browser) | Vercel AI 浏览器工具 |
| [Stagehand](https://github.com/browserbase/stagehand) | 自然语言浏览器操作 |

---

## 🤝 多 Agent 编排

*Multi-Agent orchestration & patterns。*

> **怎么选：** 需要 Agent 之间互相通信？看 **Google A2A**——这是协议标准。做复杂任务分解和并行执行？**Dapr Agents**（微软）或 **TaskWeaver** 提供代码优先的编排能力。

| 项目 | 描述 |
|------|------|
| [Agency Agents](https://github.com/msitarzewski/agency-agents) | 完整 AI 代理机构，100K+ stars |
| [Agent Protocol (A2A)](https://github.com/google/A2A) | Google Agent-to-Agent 通信协议 |
| [Dapr Agents](https://github.com/dapr/dapr-agents) | 微软 Dapr Agent 框架 |
| [TaskWeaver](https://github.com/microsoft/TaskWeaver) | 微软代码优先 Agent 框架 |

---

## 🧠 Agent 记忆与上下文

*Long-term memory & context management for agents。*

> **怎么选：** 先想清楚需求——需要本地、轻量、可解释？**Mem0** 或 Memary。需要知识图谱？**Cognee**。需要上下文压缩而非存储？**Headroom**。

| 项目 | 描述 |
|------|------|
| [Headroom](https://github.com/chopratejas/headroom) | 上下文压缩，14K+ stars |
| [Mem0](https://github.com/mem0ai/mem0) | 智能记忆层 |
| [Memary](https://github.com/kingjulio8238/memary) | Agent 长期记忆 |
| [Cognee](https://github.com/topoteretes/cognee) | 知识图谱 + Agent 记忆 |

---

## 📊 Agent 评测

*Agent evaluation & benchmarking。*

> **怎么选：** 评测 Coding Agent？用 **SWE-bench**（软件工程标准）。评测通用能力？**GAIA**。评测 Web 操作？**WebArena**。中文和多维评测看清华 **AgentBench**。

| 项目 | 描述 |
|------|------|
| [SWE-bench](https://github.com/SWE-bench/SWE-bench) | 软件工程 Agent 评测 |
| [GAIA](https://github.com/gaia-benchmark/gaia) | 通用 AI Agent 评测 |
| [WebArena](https://github.com/web-arena-x/webarena) | Web Agent 评测环境 |
| [AgentBench](https://github.com/THUDM/AgentBench) | 清华 Agent 多维评测 |

---

## 🚀 开源 Agent 产品

*Production-ready open-source agent products。*

> **怎么选：** 想自建 ChatGPT 替代品？**Open WebUI** 或 **LobeChat**。要做低代码/拖拽式 Agent 编排？**Langflow** 或 **Flowise**。需要中文知识库问答？**FastGPT** 或 **MaxKB** 国产方案。

| 项目 | 描述 |
|------|------|
| [Open WebUI](https://github.com/open-webui/open-webui) | 自托管 LLM 聊天界面 |
| [LobeChat](https://github.com/lobehub/lobe-chat) | 现代化 LLM 聊天框架 |
| [Langflow](https://github.com/langflow-ai/langflow) | 低代码 Agent 编排 |
| [Flowise](https://github.com/FlowiseAI/Flowise) | 拖拽式 LLM 应用构建 |
| [FastGPT](https://github.com/labring/FastGPT) | 中文知识库 + Agent |
| [MaxKB](https://github.com/1Panel-dev/MaxKB) | 中文知识库问答系统 |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | 全栈 AI 应用 |

---

## 📄 论文精选

*Key papers in AI agent research (2023-2026)。*

> **怎么选：** 想理解"Agent 为什么能用工具"？从 **ReAct** 开始——这是思想源头。做 Coding Agent 看 **SWE-Agent** 和 **Devin**。关注多 Agent 协作？**Agent-as-a-Judge** 和 **The Agent Company** 展示了最新范式。

| 论文 | 描述 |
|------|------|
| [ReAct](https://arxiv.org/abs/2210.03629) | Reasoning + Acting 模式 |
| [AutoGPT](https://arxiv.org/abs/2308.08155) | 自主 GPT Agent |
| [BabyAGI](https://github.com/yoheinakajima/babyagi) | 任务驱动的自主 Agent |
| [SWE-Agent](https://arxiv.org/abs/2405.15793) | 软件工程 Agent |
| [Devin](https://arxiv.org/abs/2403.13081) | 首个 AI 软件工程师 |
| [Agent-as-a-Judge](https://arxiv.org/abs/2410.10934) | Agent 作为评测者 |
| [The Agent Company](https://arxiv.org/abs/2412.14161) | Agent 自主运营公司 |

---

## 📚 教程与课程

> **怎么选：** 想系统学？**HuggingFace Agents Course** 免费且全面。偏实操？**DeepLearning.AI 多 Agent 课程** 由 Andrew Ng 主讲。需要企业级模式？Anthropic 和 OpenAI 的官方 Agent 指南是最佳实践。

| 资源 | 描述 |
|------|------|
| [DeepLearning.AI Multi-Agent](https://www.deeplearning.ai/short-courses/) | Andrew Ng 多 Agent 课程 |
| [LangChain Academy](https://academy.langchain.com/) | LangChain 官方课程 |
| [Anthropic Agent Guide](https://docs.anthropic.com/en/docs/build-with-claude/agent-patterns) | Anthropic Agent 模式指南 |
| [OpenAI Agents Guide](https://platform.openai.com/docs/guides/agents) | OpenAI Agent 开发指南 |
| [HuggingFace Agents Course](https://huggingface.co/learn/agents-course) | HuggingFace Agent 课程 |

---

## 🌏 中文社区

*Chinese AI Agent communities & resources。*

| 社区 | 描述 |
|------|------|
| [WayToAGI](https://waytoagi.com/) | 通往 AGI 之路，中文 AI 知识库 |
| [AI 破局俱乐部](https://www.zhihu.com/column/c_17800000000000) | 知乎 AI Agent 专栏 |
| [机器之心 Agent](https://www.jiqizhixin.com/) | AI 前沿资讯 |
| [Prompt Engineering Guide CN](https://www.promptingguide.ai/zh) | 中文提示工程指南 |
| 即刻 - AI Agent 圈 | 即刻 App AI Agent 话题 |
| Twitter/X - #AIAgent | AI Agent 中文讨论 |

---

## 🇨🇳 国产模型适配

*主流国产大模型在 Agent 场景下的兼容情况。*

| 模型 | Agent 框架兼容 | MCP 支持 | 推荐场景 |
|------|:--:|:--:|------|
| DeepSeek V3/V4 | ✅ OpenAI 兼容 API | ✅ | 高性价比通用 Agent |
| Qwen 系列 | ✅ OpenAI 兼容 API | ✅ | 中文理解最强 |
| GLM-5 | ✅ OpenAI 兼容 API | ✅ | 编程 Agent |
| Kimi K2 | ✅ OpenAI 兼容 API | ✅ | 长上下文 Agent |
| MiMo V2.5 | ✅ OpenAI 兼容 API | 部分 | 推理密集型 Agent |
| MiniMax M2.5 | ✅ OpenAI 兼容 API | 部分 | Agent 特化场景 |
| 混元 Hy3 | ✅ OpenAI 兼容 API | ✅ | 超高性价比 Agent |

> 以上信息基于 2026-06 公开资料。国产模型大多兼容 OpenAI API 格式，可直接接入支持自定义 API 的 Agent 框架。具体兼容性以各项目最新文档为准。

---

## 🤝 贡献指南

欢迎 PR！请确保：
1. 项目与 AI Agent 直接相关
2. 有中文资源优先（但不限于中文）
3. 按分类添加到对应章节
4. 提交前检查无重复

[贡献方式](#-贡献指南) | 欢迎 PR！

---

## 🧩 Studiopig Agent Stack

Awesome AI Agents CN 是 [Studiopig Agent Stack](https://github.com/studiopig) 的一部分——一套面向中文开发者的轻量本地 AI Agent 基础设施：

- 📋 awesome-ai-agents-cn — 中文 Agent 选型入口
- 🔧 [mcp-toolkit](https://github.com/studiopig/mcp-toolkit) — 安全默认的本地 Agent 工具箱
- 🧠 [agent-memory-lite](https://github.com/studiopig/agent-memory-lite) — 本地 Agent 长期记忆层

三个项目互相独立，组合使用可覆盖本地 Agent 的发现→工具→记忆全链路。

---

## ⭐ Star History

如果这个列表对你有帮助，请给个 ⭐ 支持一下！

---

<p align="center">
  <i>Agent 不死，编排不止 🚀</i>
</p>
