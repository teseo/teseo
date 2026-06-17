# Javier Mellado · `teseo`

**Solo builder. I orchestrate fleets of AI agents to ship software, and I create the tooling that makes that work.**

Agentic engineer in Edinburgh, 20+ years writing code. These days I spend less time typing and more time at the level above the code: planning, reviewing, merging, and designing the systems that let a fleet of agents work together. Local-first whenever it is feasible.

## The system

**🧠 [roca-madre](https://github.com/thellmwhisperer/roca-madre)**  
The local-first operating substrate for a fleet of AI coding agents, served over MCP and built as removable plugins:
- **Memory and structured RAG:** multi-layer memory with text-to-SQL retrieval. A fastText query-intent classifier and a generated semantic layer compile natural language to SQL, no embeddings.
- **El Jardin coordination:** an IRC-style channel layer where agents join, claim voice, take turns, and work from shared history.
- **Human-in-the-loop gates:** a proposal and approval workflow that holds risky agent actions (GitHub writes and the like) for sign-off.
- **Run observability and inbox:** live run tracking (logs, cancel, expire) plus an async inbox that routes questions and reviews between agents and human.
- **Multimodal and ingestion:** vision and video tools, plus an ingestion pipeline that builds the corpus from your agents' session logs, whatever tool they run on (Claude Code, Codex, Hermes, and more).

**🤖 [combo-chen](https://github.com/thellmwhisperer/combo-chen)**  
Deterministic harness for autonomous issue-to-PR pipelines. An event-sourced state machine drives fixed roles (coder, gatekeeper, reviewer) with strict role separation, SHA-pinned review gates, CI reconciliation, and a human-in-the-loop merge. Built on git worktrees and tmux.

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
