# AI Product Leadership Academy

An evidence-based, build-first research project for developing practical AI product leadership capability.

The project is deliberately **not a curriculum yet**. Its current goal is to identify the smallest set of high-signal resources that produces the largest increase in capability for product leaders who need to understand, build, evaluate, and lead AI-enabled products.

## Principles

- Practical over theoretical
- Product-first
- Build-first
- Python-first
- Snowflake-first
- Copilot-native
- Learn by building
- Prefer primary and practitioner-authored sources
- Optimize for capability gained per hour invested
- Avoid academic ML, deep math, certification-for-its-own-sake, prompt-engineering theater, and passive AI literacy

## Capability domains

| # | Domain |
|---|---|
| 01 | LLM & AI Engineering Fundamentals |
| 02 | AI Product Discovery & Opportunity Framing |
| 03 | Evaluation, Reliability & AI Quality |
| 04 | AI-Assisted Building: Python, Git & GitHub Copilot |
| 05 | Context Engineering, Retrieval & RAG |
| 06 | Agents, Tools & Agentic Workflows |
| 07 | Responsible AI, Security & Governance |
| 08 | Snowflake AI & Data Application Engineering |
| 09 | AI-Native Knowledge Work & Delegation |
| 10 | Human-AI Product Design |
| 11 | ML & Data Science Fundamentals for Product Leaders |
| 12 | AI Strategy, Economics & Portfolio Management |

The ordering is a priority ranking, **not a learning sequence**.

## Repository layout

- `prompts/` — standalone research prompts. `00` is the master research contract; `01`–`12` each cover one capability domain.
- `deep-research/` — persistent research findings. Domain findings use the same numbered basename as their prompt.
- `AGENTS.md` — repository-wide instructions for AI coding/research agents.
- `prompts/AGENTS.md` — rules for maintaining prompts.
- `deep-research/AGENTS.md` — rules for persistent research artifacts.
- `.githooks/` — lightweight local repository protections.
- `scripts/setup-hooks.sh` — enables the checked-in hooks for a local clone.

## Running the research

Each numbered prompt is designed to be pasted into a **separate research session** without relying on prior chat context.

For example:

- Prompt: `prompts/ai-product-leadership-05-context-engineering-rag.md`
- Research branch: `research/05-context-engineering-rag`
- Findings: `deep-research/ai-product-leadership-05-context-engineering-rag.md`

The session should research only that domain, write the complete findings to the matching file, verify the GitHub write, and stop.

## Current status

- Phase 1 capability-domain map: complete
- Domain 01 canon: researched and persisted
- Domains 02–12: standalone prompts ready for independent research sessions

See `prompts/ai-product-leadership-00-academy.md` for the full research contract.

## Local setup

After cloning the repository, enable the checked-in hooks:

```sh
./scripts/setup-hooks.sh
```

The hooks catch basic staged-file problems and prevent direct pushes to `main`. They are a local guardrail; GitHub branch protection remains the stronger remote control if enabled.

## License

MIT. See `LICENSE`.
