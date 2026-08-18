# AI Product Leadership Academy — Domain 06: Agents, Tools & Agentic Workflows

## Mission

Research **Agents, Tools & Agentic Workflows only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This prompt is standalone.

## Academy context

Audience: PM through Principal PM and AI-minded builders. Environment: Python-first, Snowflake-centric, GitHub Copilot available, enterprise. Practical and build-first; optimize for durable system judgment rather than framework novelty.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

The durable capability is **agentic system design and product judgment**, not mastery of one framework.

Cover:
- agent vs workflow
- deterministic orchestration vs autonomy
- tools and function calling
- state and memory
- planning and execution
- tool ergonomics/interface design
- MCP and interoperability concepts
- permissions and least privilege
- approvals and human checkpoints
- failure recovery
- autonomy boundaries
- agent evaluation
- when a simple LLM call or deterministic workflow is better than an agent

Avoid framework-first tutorials and multi-agent novelty unless they teach durable underlying patterns exceptionally well.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**.

For each candidate include only: Title; Author/organization; Direct URL; Estimated time; Difficulty; Capability gained — one sentence; Decision `CANON` / `REFERENCE` / `DEFER` / `REJECT`; Why — maximum 100 words; Main competitor it beats or why it loses — one sentence.

Evaluate capability/hour, practicality, durability, enterprise relevance, builder mindset, and teaching quality. Prefer current primary/practitioner sources.

## Output discipline — curation, not curriculum

This artifact is a **curator decision record**, not an agents handbook. Do not teach agent architectures, invent autonomy frameworks, produce tool-design checklists, prescribe implementation patterns, or create exercises. Identify the sources that best teach those capabilities instead.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10.
3. **Canonical set** — usually 2–5 resources with a brief minimum-sufficient-set rationale.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings.
5. **Rejected / deferred** — what lost and where it belongs if another domain owns it.
6. **Uncertainties / version notes** — material caveats only.

Aim for **2,000–3,000 words; hard maximum 3,500 words** excluding URLs/table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/06-agents-tools-workflows`

Prompt: `prompts/ai-product-leadership-06-agents-tools-workflows.md`

Findings: `deep-research/ai-product-leadership-06-agents-tools-workflows.md`

Create/reuse the branch, never write `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is complete only after the final findings are persisted to GitHub and fetched back for verification.** If Deep Research does not expose GitHub write actions, finish the research there, then return to the normal connected session and use GitHub tools to save the completed artifact. Do not stop at the Deep Research/chat report.

After writing, fetch the findings file back, confirm it contains the complete ranked candidates and canonical set, and report path, branch, and commit SHA. If GitHub writes are genuinely unavailable, say so explicitly and provide the complete artifact in chat; never claim completion until persistence is verified.

## Stop condition

STOP after this domain. No curriculum, timeline, learning path, or another domain.
