<div align="center">

# ⚒️ AgentForge

![AgentForge logo](assets/logo-preview.png)

### Where AI agents are forged — orchestration for Claude Code & Codex

[![Status](https://img.shields.io/badge/status-maintained_fork-6366f1?style=for-the-badge)](../../)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge)](LICENSE)
[![Based on Ruflo](https://img.shields.io/badge/based_on-Ruflo_by_rUv-8b5cf6?style=flat-square)](https://github.com/ruvnet/ruflo)

**Maintained by [Soulcynics404](https://github.com/Soulcynics404)** · Harsh Raj

</div>

---

> **Agent = Model + Harness.** The model writes; the harness gives it tools, memory, loops, sandboxes, and controls so it can actually work. **AgentForge is that harness** — the execution layer around Claude Code and Codex that adds 100+ specialized agents, coordinated swarms, self-learning memory, and enterprise guardrails. So agents don't just run, they collaborate.

AgentForge is an actively maintained fork of [Ruflo](https://github.com/ruvnet/ruflo) (formerly claude-flow) by [rUv](https://github.com/ruvnet), rebranded and maintained independently under the MIT license. All credit for the original architecture goes to the upstream project and its contributors.

## ✦ What you get

```
User --> AgentForge (CLI/MCP) --> Router --> Swarm --> Agents --> Memory --> LLM Providers
              ^                                                   |
              +---------------- Learning Loop <-------------------+
```

- 🧠 **Self-learning memory** — HNSW vector search across sessions; agents remember what worked
- 🐝 **Coordinated swarms** — hierarchical, mesh, and adaptive topologies with 100+ specialist agent types
- 🔀 **Smart routing** — 3-tier model routing (deterministic codemod → Haiku → Sonnet/Opus)
- 🪝 **Hooks + observability** — pre/post-edit hooks, session lifecycle, 12 background workers
- 🔌 **MCP server** — 300+ tools exposed to any MCP-capable client
- 🧩 **Plugin ecosystem** — ADRs, DDD, security audits, cost tracking, browser automation, and more

## ✦ Quick start

```bash
# Initialize in a project (creates .claude/, MCP config, hooks)
npx ruflo init          # runtime package name remains `ruflo` on npm

# Health check
npx ruflo doctor --fix
```

> **Note:** the npm binary name is inherited from upstream (`ruflo`); the project identity, branding, and maintenance are AgentForge's.

## ✦ Requirements

| Requirement | Why |
|---|---|
| Node.js ≥ 20 | CLI runtime |
| Claude Code or Codex CLI installed & authenticated | **Agents execute via these harnesses** — AgentForge coordinates, they build |

## ✦ Honest positioning

AgentForge is a **coordination layer**. It does not execute tasks itself — it tracks swarms, memory, and policy while Claude Code / Codex do the building. If you want single-agent work, you don't need this project.

## ✦ License

MIT — see [LICENSE](LICENSE). Original code © 2024–2026 ruvnet. Fork maintenance & rebranding © 2026 Harsh Raj (Soulcynics404).
