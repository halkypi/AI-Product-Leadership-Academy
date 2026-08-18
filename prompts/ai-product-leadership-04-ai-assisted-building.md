# AI Product Leadership Academy — Domain 04: AI-Assisted Building — Python, Git & GitHub Copilot

## Mission

Research **AI-Assisted Building: Python, Git & GitHub Copilot only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This prompt is standalone.

## Academy context

Audience: PM through Principal PM and AI-minded builders. Environment: Python-first, Snowflake-centric, GitHub Copilot available, enterprise, strong data culture. Optimize for practical build capability, not academic breadth.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

The target is **prototype-grade engineering literacy**, not turning PMs into professional software engineers.

Cover:
- Python for scripts, notebooks, APIs, and small applications
- libraries and dependency management
- environment configuration and secrets hygiene
- Git and repositories
- tests and debugging
- API integration
- GitHub workflows where directly relevant
- effective use of GitHub Copilot/coding agents for repository research, planning, implementation, and review
- verification of AI-generated code

Exclude CS surveys, interview algorithms, object-oriented overengineering, and broad “learn Python” material without direct build leverage.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**.

For each candidate include only: Title; Author/organization; Direct URL; Estimated time; Difficulty; Capability gained — one sentence; Decision `CANON` / `REFERENCE` / `DEFER` / `REJECT`; Why — maximum 100 words; Main competitor it beats or why it loses — one sentence.

Evaluate capability/hour, practical applicability, durability, enterprise relevance, builder mindset, and teaching quality. Prefer primary docs and hands-on practitioner material. Use current authoritative sources and direct URLs.

## Output discipline — curation, not curriculum

This artifact is a **curator decision record**, not a lesson or coding course. Do not teach Python/Git/Copilot, create exercises, build projects, write implementation guides, or invent a learning sequence. Identify the best sources that teach those capabilities instead.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10.
3. **Canonical set** — usually 2–5 resources, with a brief minimum-sufficient-set rationale.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings.
5. **Rejected / deferred** — what lost and where it belongs if another domain owns it.
6. **Uncertainties / version notes** — material caveats only.

Aim for **2,000–3,000 words; hard maximum 3,500 words** excluding URLs/table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/04-ai-assisted-building`

Prompt: `prompts/ai-product-leadership-04-ai-assisted-building.md`

Findings: `deep-research/ai-product-leadership-04-ai-assisted-building.md`

Create/reuse the branch, never write `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is complete only after the final findings are persisted to GitHub and fetched back for verification.** If Deep Research does not expose GitHub write actions, finish the research there, then return to the normal connected session and use GitHub tools to save the completed artifact. Do not stop at the Deep Research/chat report.

After writing, fetch the findings file back, confirm it contains the complete ranked candidates and canonical set, and report path, branch, and commit SHA. If GitHub writes are genuinely unavailable, say so explicitly and provide the complete artifact in chat; never claim completion until persistence is verified.

## Stop condition

STOP after this domain. No curriculum, learning path, timeline, or other-domain research.
