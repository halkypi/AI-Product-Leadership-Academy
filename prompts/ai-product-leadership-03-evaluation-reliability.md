# AI Product Leadership Academy — Domain 03: Evaluation, Reliability & AI Quality

## Mission

Research **Evaluation, Reliability & AI Quality only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This is a standalone research prompt.

## Academy context

Audience: Product Managers, Senior PMs, Principal PMs, and AI-minded builders. Environment: Python-first, Snowflake-centric, GitHub Copilot available, enterprise setting, strong data culture. Principles: practical, product-first, build-first, durable, and verification-oriented; avoid academic breadth and passive AI literacy.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

## Domain boundary

This domain is about defining “good,” measuring it, diagnosing failures, and making evidence-based ship/no-ship decisions for probabilistic AI systems.

Cover:
- success criteria
- representative test sets
- deterministic, rubric, human, and model-based graders
- task-specific metrics including precision/recall where relevant
- error analysis
- regression and continuous evaluation
- retrieval evaluation separately from generation
- agent outcome and trajectory evaluation
- reliability/observability insofar as they support diagnosis and quality improvement
- quality / latency / cost tradeoffs

Do not drift into generic analytics or experimentation unrelated to AI quality.

## Research task

Find and evaluate **no more than 10 candidate resources**. Rank them strongest to weakest and recommend the **smallest canonical set**. A resource must earn its place.

For each candidate include only:
- Title
- Author / organization
- Direct URL
- Estimated time commitment
- Difficulty
- Capability gained — one sentence
- Decision: `CANON`, `REFERENCE`, `DEFER`, or `REJECT`
- Why — maximum 100 words
- Main competitor it beats or why it loses — one sentence

Evaluate: capability/hour, practical applicability, durability, enterprise relevance, builder mindset, and teaching quality. Prefer primary evaluation guidance from model providers, rigorous engineering teams, researchers, and standards bodies. Use current authoritative sources and direct URLs.

## Output discipline — curation, not curriculum

This artifact is a **research librarian / curator decision record**, not a lesson, course, handbook, or domain explainer.

Do **not** teach or summarize the subject into a mini-course. Do not invent frameworks, checklists, operating models, maturity models, exercises, learning sequences, or implementation playbooks. If a useful framework emerges, identify the source that teaches it rather than recreating it.

Required findings structure:
1. **Domain boundary** — 3–6 concise bullets.
2. **Ranked candidates** — up to 10, using the fields above.
3. **Canonical set** — usually 2–5 resources, with a brief statement of why this is the minimum sufficient set.
4. **Comparative findings** — maximum 500 words total, only what is necessary to justify rankings and exclusions.
5. **Rejected / deferred** — explicitly state what lost and, when applicable, which academy domain should own it.
6. **Uncertainties / version notes** — only material caveats.

Aim for **2,000–3,000 words total; hard maximum 3,500 words** excluding URLs and table markup. Brevity is a quality criterion.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` and applicable nested `AGENTS.md` files before writing.

Research branch: `research/03-evaluation-reliability`

Prompt: `prompts/ai-product-leadership-03-evaluation-reliability.md`

Findings: `deep-research/ai-product-leadership-03-evaluation-reliability.md`

Create/reuse the research branch, never write to `main`, update rather than duplicate existing findings, and do not open a PR unless asked.

### Research-to-GitHub handoff

**Research is not complete when the Deep Research report is generated. Research is complete only when the final findings artifact is persisted to GitHub and fetched back for verification.**

If Deep Research itself does not expose GitHub write actions, finish the research first, then return to the normal connected session and use the GitHub tools there to save the completed artifact. Do not stop after producing a local/chat research report.

After writing:
1. Fetch the findings file back from the research branch.
2. Confirm the saved artifact contains the complete ranked candidate set and canonical decision.
3. Report the repository path, branch, and commit SHA.

If GitHub writes are genuinely unavailable after research, say so explicitly and provide the complete artifact in chat. Never claim the task is complete until persistence has been verified.

## Stop condition

STOP after this domain. Do not create a curriculum, timeline, learning path, or research another domain.
