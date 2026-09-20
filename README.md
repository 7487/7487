<p align="right"><a href="https://github.com/7487/7487/blob/main/README.zh-CN.md">简体中文</a></p>

# BingEdward

**AI Agent & LLM Engineering**

Building reliable AI applications and the systems behind them.

My work spans AI coding tools, LLM applications, and backend engineering. My background includes cloud / IaaS and GPU-related development at **Baidu**, and AI coding tools at **Alibaba Taotian**.

**Focus:** Agent workflows · AI Code Review · SDK reliability · CI/CD · Retrieval & memory

## Selected upstream contributions

A selection of **merged pull requests**, focused on correctness, compatibility, and regression prevention.

| Project | My contribution | Merged PRs |
| :--- | :--- | :--- |
| **AMD GAIA** | Fixed a release-test gate that silently swallowed failures; corrected backend-test dependencies and added workflow contract tests. | [#3573](https://github.com/amd/gaia/pull/3573) |
| **PR-Agent** | Fixed inline-comment line resolution in the Bitbucket Cloud and Server providers, preserving the existing integer-line path. | [#3136](https://github.com/The-PR-Agent/pr-agent/pull/3136) |
| **OpenSandbox** | Bounded readiness-polling sleeps by the remaining timeout budget in the Go, JavaScript, and Kotlin SDKs; added regression coverage. | [Go #1744](https://github.com/opensandbox-group/OpenSandbox/pull/1744) · [JS #1745](https://github.com/opensandbox-group/OpenSandbox/pull/1745) · [Kotlin #1747](https://github.com/opensandbox-group/OpenSandbox/pull/1747) |
| **Semantica** | Removed redundant vector deletion during memory erasure; removed signed Neptune authentication material from logs and added regression tests. | [Memory #1379](https://github.com/semantica-agi/semantica/pull/1379) · [Security #1373](https://github.com/semantica-agi/semantica/pull/1373) |
| **Apache Superset** | Isolated table-cell formatting errors so a problematic value can fall back safely without disrupting other cells. | [#39658](https://github.com/apache/superset/pull/39658) |

[Explore more merged contributions →](https://github.com/search?q=is%3Apr+is%3Amerged+author%3A7487+-user%3A7487&type=pullrequests)

## Personal tooling

### [Harness Loop Coding](https://github.com/7487/Harness_Loop_Coding)

Workspace templates for **Claude Code** and **Codex CLI**, with separate layouts for agent instructions, MCP setup, and shell-driven coding loops.

The repository keeps the two toolchains separate: `cc/` for Claude Code and `codex/` for Codex CLI.

## How I approach engineering

**Reproduce the failure → understand the contract → make a focused change → add regression coverage.**

I care about explicit failure handling, predictable timeout behavior, backward compatibility, and tests that catch the original bug—not just exercise the happy path.

**Working stack:** Python · Go · Java · TypeScript / JavaScript · GitHub Actions

---

Open to technical discussions about agent tooling, AI-assisted development, and reliable LLM systems.
