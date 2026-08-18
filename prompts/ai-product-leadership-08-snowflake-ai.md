# AI Product Leadership Academy — Domain 08: Snowflake AI & Data Application Engineering

## Mission

Research **Snowflake AI & Data Application Engineering only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader working in a Snowflake-centric enterprise.

This prompt is standalone.

## Academy context

Audience: PM through Principal PM and AI-minded builders. Environment: Python-first, Snowflake-centric, Copilot-native enterprise. Favor durable architecture and builder capability over certification or transient UI knowledge.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

Target enough Snowflake AI/data-application capability to **prototype, reason about architecture, assess feasibility, and make product decisions where governed enterprise data lives**.

Cover current durable capability around:
- Snowflake AI functions / AI SQL
- Cortex Search
- Cortex Analyst / semantic interfaces for structured data
- Cortex Agents and tool orchestration
- Python integration and executable data applications
- governed access and permissions
- security implications
- usage, latency, and cost economics
- structured + unstructured data
- product-leader prototype/app patterns
- Snowflake-native vs external-service tradeoffs

Do not turn this into certification prep or a feature-by-feature product tour. Because Snowflake changes quickly, verify current names and capabilities.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**.

For each candidate include only: Title; Author/organization; Direct URL; Estimated time; Difficulty; Capability gained — one sentence; Decision `CANON` / `REFERENCE` / `DEFER` / `REJECT`; Why — maximum 100 words; Main competitor it beats or why it loses — one sentence.

Evaluate capability/hour, practicality, durability, enterprise relevance, builder mindset, and teaching quality. Prefer official Snowflake docs/labs and exceptional practitioner material. Verify current product names, capabilities, pricing/economics where relevant, and flag fast-changing documentation.

## Output discipline — curation, not curriculum

This artifact is a **curator decision record**, not a Snowflake course or product tour. Do not explain every feature, write labs, prescribe architectures, create a learning sequence, or reproduce documentation. Identify the smallest set of sources that best builds durable capability.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10.
3. **Canonical set** — usually 2–5 resources with a brief minimum-sufficient-set rationale.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings.
5. **Rejected / deferred** — what lost and where it belongs if another domain owns it.
6. **Uncertainties / version notes** — especially changing Snowflake product names, docs, and economics.

Aim for **2,000–3,000 words; hard maximum 3,500 words** excluding URLs/table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/08-snowflake-ai`

Prompt: `prompts/ai-product-leadership-08-snowflake-ai.md`

Findings: `deep-research/ai-product-leadership-08-snowflake-ai.md`

Create/reuse the branch, never write `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is complete only after the final findings are persisted to GitHub and fetched back for verification.** If Deep Research does not expose GitHub write actions, finish the research there, then return to the normal connected session and use GitHub tools to save the completed artifact. Do not stop at the Deep Research/chat report.

After writing, fetch the findings file back, confirm it contains the complete ranked candidates and canonical set, and report path, branch, and commit SHA. If GitHub writes are genuinely unavailable, say so explicitly and provide the complete artifact in chat; never claim completion until persistence is verified.

## Stop condition

STOP after this domain. No curriculum, timeline, learning path, or another domain.
