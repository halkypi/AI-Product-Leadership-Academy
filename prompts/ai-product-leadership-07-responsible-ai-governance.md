# AI Product Leadership Academy — Domain 07: Responsible AI, Security & Governance

## Mission

Research **Responsible AI, Security & Governance only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This prompt is standalone.

## Academy context

Audience: PM through Principal PM and AI-minded builders. Environment: Python-first, Snowflake-centric, Copilot-native enterprise. Practical product risk management over detached ethics/compliance theory.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

Cover practical product risk management across the AI lifecycle:
- risk identification and appropriate-use decisions
- data governance and privacy
- prompt injection and information-security risks
- private-data leakage
- access control and least privilege
- human approval / human-in-the-loop
- transparency and provenance where relevant
- incident thinking and operational response
- red teaming and safety evaluation
- model/system guardrails
- working with legal, security, privacy, compliance, and model-risk teams
- lifecycle governance rather than one-time gates

Do not reduce this to abstract ethics philosophy or regulation memorization detached from product and engineering decisions.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**.

For each candidate include only: Title; Author/organization; Direct URL; Estimated time; Difficulty; Capability gained — one sentence; Decision `CANON` / `REFERENCE` / `DEFER` / `REJECT`; Why — maximum 100 words; Main competitor it beats or why it loses — one sentence.

Evaluate capability/hour, practicality, durability, enterprise relevance, builder mindset, and teaching quality. Prefer standards bodies, primary safety/security guidance, and rigorous practitioner sources. Verify current standards and guidance.

## Output discipline — curation, not curriculum

This artifact is a **curator decision record**, not a governance handbook. Do not restate standards at length, invent a governance framework, create compliance checklists, prescribe controls, or write a risk-management playbook. Identify the best sources that teach those things instead.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10.
3. **Canonical set** — usually 2–5 resources with a brief minimum-sufficient-set rationale.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings.
5. **Rejected / deferred** — what lost and where it belongs if another domain owns it.
6. **Uncertainties / version notes** — especially changing standards, laws, or provider guidance.

Aim for **2,000–3,000 words; hard maximum 3,500 words** excluding URLs/table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/07-responsible-ai-governance`

Prompt: `prompts/ai-product-leadership-07-responsible-ai-governance.md`

Findings: `deep-research/ai-product-leadership-07-responsible-ai-governance.md`

Create/reuse the branch, never write `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is complete only after the final findings are persisted to GitHub and fetched back for verification.** If Deep Research does not expose GitHub write actions, finish the research there, then return to the normal connected session and use GitHub tools to save the completed artifact. Do not stop at the Deep Research/chat report.

After writing, fetch the findings file back, confirm it contains the complete ranked candidates and canonical set, and report path, branch, and commit SHA. If GitHub writes are genuinely unavailable, say so explicitly and provide the complete artifact in chat; never claim completion until persistence is verified.

## Stop condition

STOP after this domain. No curriculum, timeline, learning path, or another domain.
