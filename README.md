<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1500&color=6366F1&center=true&vCenter=true&width=550&lines=Hi%2C+I'm+JING;AI+Agent+infra+%40+Python%2FJava;PromptSlim+%7C+ai-cost-sentinel+%7C+agent-orchestrator" alt="Typing SVG" />

</div>

<div align="center">

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/github/followers/JING04-PRODUCER?style=for-the-badge&logo=github&logoColor=white&label=Followers&color=6366f1&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=repositories">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_repos&style=for-the-badge&logo=github&logoColor=white&label=Repos&color=10b981&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=stars">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_gists&style=for-the-badge&logo=github&logoColor=white&label=Gists&color=f59e0b&cacheSeconds=3600" />
</a>

<br />

<a href="mailto:3573851322@qq.com">
  <img src="https://img.shields.io/badge/Email-3573851322@qq.com-blue?style=flat-square&logo=gmail&logoColor=white" />
</a>
<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/badge/GitHub-JING04--PRODUCER-181717?style=flat-square&logo=github&logoColor=white" />
</a>

</div>

<hr style="border-color: #e5e7eb;" />

## 🧠 关于我

> 计科应届，Python 主力。**LangChain / LangGraph 生态**下做过三个 AI Agent 基础设施项目：

- Prompt 压缩引擎（[PromptSlim](#promptslim)）
- LLM 成本追踪透明代理（[AI Cost Sentinel](#ai-cost-sentinel)）
- 多 Agent 编排平台，支持 **RAG + Function Calling + DAG 工作流**（[AgentOrchestrator](#agentorchestrator)）

> 熟悉 **Prompt Engineering、RAG 检索增强、向量数据库**。找 AI 基础设施 / Python 后端方向，Base 不限。

<hr style="border-color: #e5e7eb;" />

## 项目

三个东西各解决一个我实际遇到的问题：

- 调 API 烧钱 → [**ai-cost-sentinel**](#ai-cost-sentinel)
- Prompt 越来越长 → [**PromptSlim**](#promptslim)
- 多个 Agent 不好管理 → [**AgentOrchestrator**](#agentorchestrator)

---

### PromptSlim

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/promptslim?style=flat-square)](https://github.com/JING04-PRODUCER/promptslim/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/promptslim/blob/main/LICENSE)

**Prompt Engineering 的自动化工具**——调用 LLM 前压缩 prompt，剔除冗余但保留代码块和语义。实测节省 5%~75% Token。40+ 条冗余模式来自对 GPT/Claude 行为的逆向分析，也支持 LLM 语义级压缩。兼容 GPT / Claude / DeepSeek / Qwen。

🔗 [github.com/JING04-PRODUCER/promptslim](https://github.com/JING04-PRODUCER/promptslim) ｜ [掘金详解](https://juejin.cn/post/7652277909156790272)

```python
from promptslim import quick_slim
report = quick_slim("嗯那个我想说的是这个功能非常非常好用对吧")
print(f"节省 {report.savings_pct}% Token，每次省 ${report.cost_per_call_saved:.6f}")
```

---

### AI Cost Sentinel

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/ai-cost-sentinel?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/blob/main/LICENSE)

LLM 应用的**可观测性工具**——类似 LangSmith 的成本侧实现。透明代理截获 API 请求，自动记录 Token 消耗与费用。内置 20+ 模型定价、日/月预算告警、CSV 导出、Slack 通知。Spring Boot + Chart.js 可视化面板。

🔗 [github.com/JING04-PRODUCER/ai-cost-sentinel](https://github.com/JING04-PRODUCER/ai-cost-sentinel)

```python
client = OpenAI(base_url="http://localhost:8000/v1", api_key="sk-xxx")
# 之后正常用，Sentinel 代理自动记录每次调用的成本
```

---

### AgentOrchestrator

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/agent-orchestrator?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/blob/main/LICENSE)

基于 **LangChain 设计思想**自研的 Agent 编排引擎。Python FastAPI 推理核心 + Java Spring Boot 管理面板。支持 ReAct / Plan-Execute 推理模式、DAG 工作流、**Function Calling**、DuckDuckGo Web Search、**RAG 记忆系统**（向量检索 + 会话上下文）。工具注册采用 **MCP 协议风格**插件化设计，新工具不改核心代码。

🔗 [github.com/JING04-PRODUCER/agent-orchestrator](https://github.com/JING04-PRODUCER/agent-orchestrator)

```bash
curl -X POST http://localhost:8000/api/agents/code-reviewer/run \
  -d '{"task": "审查 app.py 安全问题"}'
```

<hr style="border-color: #e5e7eb;" />

<img alt="🐍 contribution snake" src="https://raw.githubusercontent.com/JING04-PRODUCER/JING04-PRODUCER/output/github-contribution-grid-snake-dark.svg?palette=github-dark" />

<hr />

## 🔑 技能关键词

> LangChain · LangGraph · RAG 检索增强 · Prompt Engineering · Function Calling · Agent 编排 · 向量数据库 · MCP 协议 · FastAPI · Spring Boot · Docker · Python · Java

## 🛠 技术栈

<div align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
<img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white" />
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" />
<img src="https://img.shields.io/badge/Anthropic-Claude-d97757?style=for-the-badge&logo=anthropic&logoColor=white" />

</div>

<hr />

<div align="center">

[个人主页](https://jing04-producer.github.io/portfolio) &nbsp;|&nbsp;
[GitHub](https://github.com/JING04-PRODUCER) &nbsp;|&nbsp;
[掘金](https://juejin.cn/user/3573851322) &nbsp;|&nbsp;
[3573851322@qq.com](mailto:3573851322@qq.com)

</div>
