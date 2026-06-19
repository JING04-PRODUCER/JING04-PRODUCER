<div align="center">

# 👋 Hi, I'm JING

### 计科在读 | Python/Java AI Agent | 用代码解决真实痛点 🚀

</div>

<div align="center">

<!-- 数据看板 -->
<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=followers&style=flat-square&logo=github&logoColor=white&label=Followers&color=6366f1&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=repositories">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_repos&style=flat-square&logo=github&logoColor=white&label=Repos&color=10b981&cacheSeconds=3600" />
</a>
<a href="https://github.com/JING04-PRODUCER?tab=stars">
  <img src="https://img.shields.io/badge/dynamic/json?url=https://api.github.com/users/JING04-PRODUCER&query=public_gists&style=flat-square&logo=github&logoColor=white&label=Gists&color=f59e0b&cacheSeconds=3600" />
</a>
<a href="https://komarev.com/ghpvc/?username=JING04-PRODUCER">
  <img src="https://komarev.com/ghpvc/?username=JING04-PRODUCER&style=flat-square&color=ef4444&label=%F0%9F%91%80" alt="访客计数" />
</a>

<br />

<a href="mailto:3573851322@qq.com">
  <img src="https://img.shields.io/badge/%F0%9F%93%AE%203571328522@qq.com-blue?style=flat-square&logo=gmail&logoColor=white" />
</a>
<a href="https://github.com/JING04-PRODUCER">
  <img src="https://img.shields.io/badge/GitHub-JING04--PRODUCER-181717?style=flat-square&logo=github&logoColor=white" />
</a>

</div>

<hr />

## 🧠 关于我

> 计算机科学与技术 2303 班在读，专注 **Python + Java + AI Agent** 技术栈。
> 热爱开源，致力于用代码解决真实痛点。

| 🎯 方向 | 🔧 技术 | 📖 学习中 |
|:---:|:---:|:---:|
| LLM 应用开发 | Python · Java · SQL | Agent 多智能体 |
| Agent 编排框架 | FastAPI · Spring Boot | RAG 检索增强 |
| API 基础设施 | SQLite · Docker · Git | 云端部署运维 |

<hr />

## 🚀 开源项目

### 🪒 PromptSlim — AI 提示词瘦身工具包

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/promptslim?style=flat-square)](https://github.com/JING04-PRODUCER/promptslim/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/promptslim/blob/main/LICENSE)

**在 API 调用前自动剃掉冗余 Token，节省 5%~75%。** 40+ 条中英文冗余模式、代码保护避免破坏 prompt、Anthropic Prompt Caching 缓存分析、LLM 语义压缩。支持 GPT / Claude / DeepSeek / Qwen。

> 📖 [掘金详解 v0.3.0](https://juejin.cn/post/7652277909156790272)

```python
from promptslim import quick_slim
report = quick_slim("嗯那个我想说的是这个功能非常非常好用对吧")
print(f"节省 {report.savings_pct}% Token，每次省 ${report.cost_per_call_saved:.6f}")
```

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/tiktoken-Token_计数-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Anthropic-Prompt_Caching-blueviolet?style=flat-square" />
  <img src="https://img.shields.io/badge/中英文-双语支持-10b981?style=flat-square" />
</p>

---

### 🛡️ AI Cost Sentinel — 透明 API 成本追踪

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/ai-cost-sentinel?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/ai-cost-sentinel/blob/main/LICENSE)

**一行代码不改，透明追踪 AI API 调用成本。** 透明代理拦截请求，自动记录 Token 消耗与费用，20+ 模型定价、日/月预算告警、CSV 导出、模型成本对比、Slack Webhook 通知、Spring Boot + Chart.js 可视化仪表盘。

```python
# 只改这一行
client = OpenAI(base_url="http://localhost:8000/v1", api_key="sk-xxx")
# 其他代码完全不动，Sentinel 自动追踪
```

<p align="center">
  <img src="https://img.shields.io/badge/Python-FastAPI-009688?logo=fastapi&style=flat-square" />
  <img src="https://img.shields.io/badge/Java-Spring_Boot-6DB33F?logo=springboot&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/SQLite-零依赖-003B57?logo=sqlite&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Webhook-告警通知-f59e0b?style=flat-square" />
</p>

---

### 🤖 AgentOrchestrator — 跨语言 Agent 编排平台

[![GitHub stars](https://img.shields.io/github/stars/JING04-PRODUCER/agent-orchestrator?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/JING04-PRODUCER/agent-orchestrator/blob/main/LICENSE)

**Python FastAPI 推理核心 + Java Spring Boot 管理面板。** Function Calling、多 Agent 工作流（顺序/并行/DAG）、Web Search 工具、RAG 记忆系统、插件化工具注册中心，兼容所有 OpenAI 接口模型。

```bash
curl -X POST http://localhost:8000/api/agents/code-reviewer/run \
  -d '{"task": "审查 app.py 安全问题"}'
```

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12+-3776AB?logo=python&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Java-21-ED8B00?logo=openjdk&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Web_Search-DuckDuckGo-10b981?style=flat-square" />
  <img src="https://img.shields.io/badge/RAG-记忆系统-blueviolet?style=flat-square" />
</p>

<hr />

## ⚡ 动态播报

<p align="center">
  <a href="https://github.com/JING04-PRODUCER">
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=JING04-PRODUCER&theme=react-dark&hide_border=true&area=true&radius=16&custom_title=%F0%9F%93%8A+%E8%B4%A1%E7%8C%AE%E6%B4%BB%E5%8A%A8%E5%9B%BE" alt="Activity Graph" width="100%" />
  </a>
</p>

<hr />

## 📊 GitHub 统计

<div align="center">

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=JING04-PRODUCER&theme=tokyonight&hide_border=true&locale=zh_Hans&ring=6366F1&fire=6366F1&currStreakLabel=6366F1" alt="Streak" />
</a>

<br />

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=JING04-PRODUCER&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" alt="Top Languages" />
</a>

<br />

<a href="https://github.com/JING04-PRODUCER">
  <img src="https://github-profile-trophy.vercel.app/?username=JING04-PRODUCER&theme=tokyonight&no-frame=true&row=2&column=4&margin-w=4" alt="Trophy" />
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
  <i>"好的代码是写给人看的，顺便能在机器上运行。"</i>

<br /><br />

🌐 [个人主页](https://jing04-producer.github.io/portfolio) &nbsp;|&nbsp;
📧 [3573851322@qq.com](mailto:3573851322@qq.com) &nbsp;|&nbsp;
🐙 [JING04-PRODUCER](https://github.com/JING04-PRODUCER) &nbsp;|&nbsp;
📖 [掘金](https://juejin.cn/user/3573851322) &nbsp;|&nbsp;
💬 欢迎交流 AI Agent / LLM 应用开发

</div>
