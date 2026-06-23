<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1500&color=6366F1&center=true&vCenter=true&width=550&lines=Hi%2C+I'm+JING;AI+Agent+infra+%40+Python%2FJava;PromptSlim+%7C+ai-cost-sentinel+%7C+agent-orchestrator" alt="Typing SVG" />

</div>

<div align="center">

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=followers&style=for-the-badge&logo=github&logoColor=white&label=Followers&color=6366f1&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=repositories">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_repos&style=for-the-badge&logo=github&logoColor=white&label=Repos&color=10b981&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=stars">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_gists&style=for-the-badge&logo=github&logoColor=white&label=Gists&color=f59e0b&cacheSeconds=3600" />
</a>

<br />

<a href="mailto:3573851322@qq.com">
  <img src="https://img.shields.io/badge/Email-3573851322@qq.com-blue?style=flat-square&logo=maildotru&logoColor=white" />
</a>
<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/badge/GitHub-JING04--PRODUCER-181717?style=flat-square&logo=github&logoColor=white" />
</a>

</div>

<hr style="border-color: #e5e7eb;" />

<div align="center">
<table>
<tr>
<td width="60%" valign="top">

## 🧠 关于我

> 计算机科学与技术 2303 班在读，专注 **Python + Java + AI Agent** 技术栈。
> 热爱开源，致力于用代码解决真实痛点。

| 🎯 方向 | 🔧 技术 | 📖 学习中 |
|:---:|:---:|:---:|
| LLM 应用开发 | Python · Java · SQL | Agent 多智能体 |
| Agent 编排框架 | FastAPI · Spring Boot | RAG 检索增强 |
| API 基础设施 | SQLite · Docker · Git | 云端部署运维 |

</td>
<td width="40%" valign="top">

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://github-readme-stats.vercel.app/api?username=JING04-PRODUCER&show_icons=true&theme=transparent&hide_border=true&count_private=true&locale=cn&ring_color=6366f1&title_color=6366f1&icon_color=6366f1&text_color=666666&hide=stars,issues" width="100%" />
</a>

</td>
</tr>
</table>
</div>

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

调用 LLM 之前先压缩 prompt，去掉冗余词但保留代码块和关键语义。实测能省 5%~75% Token。内置 40+ 条中英文常见冗余模式，也支持调 LLM 做语义级压缩。兼容 GPT / Claude / DeepSeek / Qwen。

> [掘金详解 v0.3.0](https://juejin.cn/post/7652277909156790272)

```python
from promptslim import quick_slim
report = quick_slim("嗯那个我想说的是这个功能非常非常好用对吧")
print(f"节省 {report.savings_pct}% Token，每次省 ${report.cost_per_call_saved:.6f}")
```

---

### AI Cost Sentinel

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/ai-cost-sentinel?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/blob/main/LICENSE)

一个透明代理，截获 LLM API 请求自动算 Token 消耗和费用，业务代码不用动。内置 20+ 模型定价，支持日/月预算告警、CSV 导出、Slack 通知。附带一个 Spring Boot + Chart.js 的可视化面板。

```python
client = OpenAI(base_url="http://localhost:8000/v1", api_key="sk-xxx")
# 之后正常用，Sentinel 代理自动记录每次调用的成本
```

---

### AgentOrchestrator

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/agent-orchestrator?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/blob/main/LICENSE)

Python FastAPI 做推理核心，Java Spring Boot 做管理面板。支持 Function Calling、顺序/并行/DAG 工作流、DuckDuckGo 搜索、RAG 记忆。工具注册用了插件化设计，加新工具不用改核心代码。兼容 OpenAI 接口格式。

```bash
curl -X POST http://localhost:8000/api/agents/code-reviewer/run \
  -d '{"task": "审查 app.py 安全问题"}'
```

<hr style="border-color: #e5e7eb;" />

## 动态

<p align="center">
  <a href="https://github.com/JING04-PRODUCER">
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=JING04-PRODUCER&theme=react-dark&hide_border=true&area=true&radius=16&custom_title=%F0%9F%93%8A+%E8%B4%A1%E7%8C%AE%E6%B4%BB%E5%8A%A8%E5%9B%BE" alt="Activity Graph" width="100%" />
  </a>
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/JING04-PRODUCER/JING04-PRODUCER/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/JING04-PRODUCER/JING04-PRODUCER/output/github-contribution-grid-snake.svg" />
  <img alt="🐍 Snake eating my contributions" src="https://raw.githubusercontent.com/JING04-PRODUCER/JING04-PRODUCER/output/github-contribution-grid-snake.svg" />
</picture>

<hr />

## 📊 语言 & 贡献统计

<div align="center">

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=JING04-PRODUCER&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" alt="Top Languages" />
</a>

</div>

<hr />

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
