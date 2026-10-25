# Hi, I'm Xiao 👋

### Agent 全栈工程师 · 独立交付线上产品

我把 LLM、工具调用和工作流做成真正可用的产品——从交互、前后端和数据，到部署、可观测与持续迭代。

*Full-stack agent engineer. I turn LLMs, tools and workflows into products that run in production, built and operated end to end.*

## 我在做什么

- **Agent 产品工程**：模型接入、工具调用、上下文管理、工作流编排与安全边界
- **全栈产品交付**：从 Next.js / React 交互到 Python / Java 服务、认证、数据与异步任务
- **生产系统建设**：Docker、CI/CD、监控告警、成本治理与自托管基础设施
- **独立产品迭代**：从真实问题出发，快速上线，用反馈持续打磨

## 代表作品

| 产品 | 解决什么问题 | 代码与体验 |
| --- | --- | --- |
| **Fusion** | 面向任务执行的 AI 工作台：模型在单个 Agent 循环里自选搜索、网页深读、地图 / 天气 / 票务、知识库与 MCP 等工具，回答来源可追溯，还能产出带版本的交付文档 | [在线体验](https://fusion.seanfield.org/) · [查看项目](https://github.com/HyxiaoGe/fusion) |
| **agent-tools** | 给 Agent 用的工具服务：生图、联网搜索、网页读取统一经网关鉴权和记账，网页读取先免费直连、慢了再并行付费服务 | [查看项目](https://github.com/HyxiaoGe/agent-tools) |
| **WatchMend** | 面向自托管服务器的轻量巡检与告警：确定性规则发现问题，可选 LLM 辅助诊断 | [查看项目](https://github.com/HyxiaoGe/watchmend) |
| **Auth Service** | 为多个独立应用提供 OAuth、邮箱验证码、PKCE、JWT / JWKS 与跨应用 SSO | [API 文档](https://auth.seanfield.org/docs) · [查看项目](https://github.com/HyxiaoGe/auth-service) |

## 做成了什么

- **Fusion 从 0 到上线由我一人完成**：2025-02 至今 3100+ 次提交、520+ 个合并 PR，后端 3100+、前端 2500+ 个测试用例；PR 门禁检查，合并后自动构建并发布
- **长回答流式输出提速约 80 倍**：模型 104 秒就生成完的 4.8 万字回答，服务端处理却要 1247 秒；定位到每个增量都对全文重新扫描的平方级开销，优化后降到 15.5 秒
- **Agent 轨迹不再丢失**：并行调用 3 个以上工具时，约 18% 的运行会丢掉整段执行轨迹；用诊断日志定位到瞬时的写入名额争用，拆开旁路写入后，并发压测 18 个运行全部完整记录
- **网页读取按实测选型**：同一批 120 个网址对比各家服务的耗时与正文质量，设计「免费直连 → 并行付费 → 兜底」的读取调度，单次读取上限 10 秒
- **自托管生产环境**：Docker 部署、Windows 构建机出镜像、Prometheus / Loki 监控与飞书告警，统一认证服务支撑多个应用单点登录

## 产品方法

- **先解决真实问题**：不为 Agent 而 Agent，先找到值得自动化、增强或重新设计的用户任务
- **让模型做擅长的事**：用 LLM 处理理解、判断与表达，用确定性系统守住权限、状态和可靠性边界
- **对完整体验负责**：一个人覆盖产品、交互、工程与运维，让原型最终成为长期可用的线上产品

主要使用 **TypeScript、React、Next.js、Python、FastAPI、Java、PostgreSQL、Redis、Docker**，并持续探索多模型 LLM / ASR、工具调用与自托管基础设施。

> Execution beats perfection. Careful, patient, persistent.

## GitHub

<p>
  <img height="165" src="https://github-readme-stats-nine-rouge-81.vercel.app/api?username=HyxiaoGe&show_icons=true&include_all_commits=true&count_private=true" alt="Xiao's GitHub stats" />
  <img height="165" src="https://github-readme-stats-nine-rouge-81.vercel.app/api/top-langs?username=HyxiaoGe&hide=javascript,css,html,php,freemarker,scss,stylus&count_private=true&layout=compact" alt="Xiao's most used languages" />
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HyxiaoGe/HyxiaoGe/gh-pages/github-snake-dark.svg" />
  <img alt="GitHub contribution grid snake animation" src="https://raw.githubusercontent.com/HyxiaoGe/HyxiaoGe/gh-pages/github-snake.svg" />
</picture>
