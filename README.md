# Javier Mellado

**Solo builder. I orchestrate fleets of AI agents to ship software, and I create the tooling that makes that work.**

Agentic engineer in Edinburgh, 20+ years writing code. These days I spend less time typing and more time at the level above the code: planning, reviewing, merging, and designing the systems that let a fleet of agents work together. Local-first whenever it is feasible.

## The system

**🤖 [combo-chen](https://github.com/thellmwhisperer/combo-chen)**  
Deterministic harness for autonomous issue-to-PR pipelines. An event-sourced state machine drives fixed roles (coder, gatekeeper, reviewer) with strict role separation, SHA-pinned review gates, CI reconciliation, and a human-in-the-loop merge. Built on git worktrees and tmux.

**☁️ [roca-cloud](https://github.com/thellmwhisperer/roca-cloud)**  
The cloud memory plane: roca's MCP-native store deployed on AWS as a single ARM64 Lambda behind API Gateway, backed by private RDS PostgreSQL and Secrets Manager, provisioned end-to-end with CDK.

**🛡️ [human.md](https://github.com/thellmwhisperer/human.md)**  
A guardrail framework for human-agent pairing: declarative rules that tell a coding agent when to defer, stop, or hand back control, enforced through hooks.

## Applied AI

**🎥 [conferenceDB](https://github.com/thellmwhisperer/conferenceDB)**  
Agent-native RAG over conference talks. Hybrid retrieval over SQLite FTS5 full-text search and sqlite-vec vector embeddings, fully local. Turns video transcripts into a queryable knowledge base.

**🏠 [land-registry-nlq](https://github.com/thellmwhisperer/land-registry-nlq)**  
Text-to-SQL over 31M UK Land Registry transactions. Plain-English questions compiled to PostgreSQL and validated against the query AST (libpg-query) before execution, with Claude Haiku in the loop.

## How I work

- I design the system and the guardrails, then let agents execute inside them.
- Local-first. I run models on my own hardware (Ollama, MLX) when it is feasible.
- Tests and review are not optional. Determinism, gates, and a human merge decision are baked into how my agents ship.

## Tooling

TypeScript · Python · Node · React / React Native · SQLite · MCP. Claude, Codex, and local models via Ollama and MLX.

---

<p align="center">
  🎵 Multi-instrumentalist · 🌧️ Scottish weather lover
</p>
