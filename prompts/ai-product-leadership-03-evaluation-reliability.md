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

Produce no more than 10 candidates. For each provide Title, Author/organization, URL, Time commitment, Difficulty, Capability gained, canon decision, and why alternatives lose. Rank and defend them, then recommend the smallest canonical set.

## Evaluation criteria

1. Capability/hour
2. Practical applicability
3. Durability
4. Enterprise relevance
5. Builder mindset
6. Teaching quality

Prefer primary evaluation guidance from model providers, rigorous engineering teams, researchers, and standards bodies. Use current authoritative sources and direct URLs.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` before writing.

Research branch: `research/03-evaluation-reliability`

Prompt: `prompts/ai-product-leadership-03-evaluation-reliability.md`

Findings: `deep-research/ai-product-leadership-03-evaluation-reliability.md`

Create/reuse the research branch, never write `main`, update rather than duplicate existing findings, do not open a PR unless asked, verify the saved file, and report path/branch/commit SHA.

## Stop condition

STOP after this domain. Do not create a curriculum, timeline, learning path, or research another domain.
