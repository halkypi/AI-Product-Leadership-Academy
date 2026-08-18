# AI Product Leadership Academy — Domain 12: AI Strategy, Economics & Portfolio Management

## Mission

Research **AI Strategy, Economics & Portfolio Management only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This prompt is standalone.

## Academy context

Audience: PM through Principal PM and AI-minded builders. Environment: Python-first, Snowflake-centric, Copilot-native enterprise. Strategy must be grounded in actual system capability and economics, not futurism.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

Cover:
- build vs buy
- model/provider choice
- proprietary vs commodity advantage
- data advantage
- switching costs and portability
- quality / latency / cost tradeoffs
- central AI platform vs embedded product teams
- workflow redesign
- automation vs augmentation
- organizational adoption
- portfolio prioritization
- where durable differentiation resides
- consumption economics and operational cost
- strategic consequences of rapidly changing model capabilities

Reject generic “AI transforms every industry” material, executive futurism, and strategy detached from hands-on system realities.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**.

For each candidate include only: Title; Author/organization; Direct URL; Estimated time; Difficulty; Capability gained — one sentence; Decision `CANON` / `REFERENCE` / `DEFER` / `REJECT`; Why — maximum 100 words; Main competitor it beats or why it loses — one sentence.

Evaluate capability/hour, practicality, durability, enterprise relevance, builder mindset, and teaching quality. Prefer primary provider economics/architecture guidance, empirical research, respected practitioner writing, and rigorous economic/business analysis. Verify current economics and capabilities.

## Output discipline — curation, not curriculum

This artifact is a **curator decision record**, not an AI strategy playbook. Do not write an executive strategy essay, invent portfolio frameworks, prescribe an operating model, create transformation checklists, or build a learning sequence. Identify the strongest sources that teach durable strategic judgment instead.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10.
3. **Canonical set** — usually 2–5 resources with a brief minimum-sufficient-set rationale.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings.
5. **Rejected / deferred** — what lost and where it belongs if another domain owns it.
6. **Uncertainties / version notes** — especially fast-changing provider capabilities and economics.

Aim for **2,000–3,000 words; hard maximum 3,500 words** excluding URLs/table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/12-ai-strategy-economics`

Prompt: `prompts/ai-product-leadership-12-ai-strategy-economics.md`

Findings: `deep-research/ai-product-leadership-12-ai-strategy-economics.md`

Create/reuse the branch, never write `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is complete only after the final findings are persisted to GitHub and fetched back for verification.** If Deep Research does not expose GitHub write actions, finish the research there, then return to the normal connected session and use GitHub tools to save the completed artifact. Do not stop at the Deep Research/chat report.

After writing, fetch the findings file back, confirm it contains the complete ranked candidates and canonical set, and report path, branch, and commit SHA. If GitHub writes are genuinely unavailable, say so explicitly and provide the complete artifact in chat; never claim completion until persistence is verified.

## Stop condition

STOP after this domain. No curriculum, timeline, learning path, or another domain.
