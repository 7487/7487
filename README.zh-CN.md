<p align="right"><a href="https://github.com/7487/7487/blob/main/README.md">English</a></p>

# BingEdward

**AI Agent 与大模型工程**

构建可靠的 AI 应用，以及支撑它们的工程系统。

关注 AI Coding 工具、大模型应用与后端工程。曾在 **百度** 从事云 / IaaS 与 GPU 相关开发，在 **阿里淘天** 从事 AI Coding 工具开发。

**关注方向：** Agent 工作流 · AI Code Review · SDK 可靠性 · CI/CD · 检索与记忆

## 代表性上游贡献

以下精选贡献均已合入上游，重点解决正确性、兼容性与回归防护问题。

| 项目 | 我的贡献 | 已合并 PR |
| :--- | :--- | :--- |
| **AMD GAIA** | 修复发布测试门禁吞掉失败、错误放行的问题；补齐后端测试依赖，并添加工作流契约测试。 | [#3573](https://github.com/amd/gaia/pull/3573) |
| **PR-Agent** | 修复 Bitbucket Cloud / Server Provider 的行内评论定位，将 diff 行文本解析为行号，同时保留已有的整数行号调用方式。 | [#3136](https://github.com/The-PR-Agent/pr-agent/pull/3136) |
| **OpenSandbox** | 修复 Go、JavaScript、Kotlin SDK 的就绪轮询休眠超出剩余超时预算的问题，补充回归测试。 | [Go #1744](https://github.com/opensandbox-group/OpenSandbox/pull/1744) · [JS #1745](https://github.com/opensandbox-group/OpenSandbox/pull/1745) · [Kotlin #1747](https://github.com/opensandbox-group/OpenSandbox/pull/1747) |
| **Semantica** | 避免 Agent 记忆清理时重复删除向量；移除 Neptune 签名认证信息的日志输出，并补充回归测试。 | [记忆 #1379](https://github.com/semantica-agi/semantica/pull/1379) · [安全 #1373](https://github.com/semantica-agi/semantica/pull/1373) |
| **Apache Superset** | 隔离表格单元格的格式化异常，让异常值安全降级显示，避免影响其他单元格。 | [#39658](https://github.com/apache/superset/pull/39658) |

[查看更多已合并贡献 →](https://github.com/search?q=is%3Apr+is%3Amerged+author%3A7487+-user%3A7487&type=pullrequests)

## 个人工具项目

### [Harness Loop Coding](https://github.com/7487/Harness_Loop_Coding)

面向 **Claude Code** 与 **Codex CLI** 的工作区模板，组织 Agent 指令、MCP 配置与 Shell 编码循环。

两套工具链分别维护：`cc/` 对应 Claude Code，`codex/` 对应 Codex CLI。

## 工程方法

**复现问题 → 理解现有契约 → 聚焦修改 → 补充回归验证。**

关注明确的失败处理、可预期的超时行为、向后兼容，以及能够真正捕获原始问题、而非只覆盖正常路径的测试。

**常用技术：** Python · Go · Java · TypeScript / JavaScript · GitHub Actions

---

欢迎交流 Agent 工具、AI 辅助开发与大模型系统可靠性。
