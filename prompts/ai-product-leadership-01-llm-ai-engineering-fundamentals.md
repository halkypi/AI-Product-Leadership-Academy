# AI Product Leadership Academy — Domain 01: LLM & AI Engineering Fundamentals

## Mission

Research **LLM & AI Engineering Fundamentals only** and identify the smallest canonical set of resources that produces the largest increase in practical capability for an AI-minded product leader.

This is a standalone research prompt. Do not require prior chat context.

## Academy context

Audience: Product Managers, Senior PMs, Principal PMs, and AI-minded builders.

Environment: Python-first, Snowflake-centric, GitHub Copilot available, enterprise setting, strong data culture.

Principles: practical over theoretical; product-first; build-first; Python-first; Snowflake-first; Copilot-native; learn by building. Avoid academic ML, deep math, certifications for their own sake, prompt-engineering theater, and passive AI literacy.

The academy optimizes for the **smallest set of resources that produces the largest increase in capability**, not completeness.

Master prompt: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/prompts/ai-product-leadership-00-academy.md`

Phase 1 domain map: `https://github.com/halkypi/AI-Product-Leadership-Academy/blob/main/deep-research/ai-product-leadership-academy.md`

Do not depend on reading either file before proceeding; the essential context is included here.

## Domain boundary

The target is **systems literacy rather than ML theory**.

Cover the mental models needed to design, prototype, debug, evaluate, and discuss an LLM application, including:

- models and inference
- tokens and context
- APIs
- structured outputs
- tool/function calling
- multimodality
- embeddings conceptually
- model selection
- latency and cost
- nondeterminism
- prompting as one control surface among several
- the major levers for changing system behavior

Exclude transformer mathematics, gradient derivations, pretraining theory, model-architecture surveys, and deep ML coursework unless a resource is exceptional enough to justify its time cost for this audience.

## Research task

Produce **no more than 10 candidate resources**. For each provide Title, Author/organization, URL, Time commitment, Difficulty, Capability gained, why it belongs or does not belong, and why competing resources were rejected.

Rank all candidates, defend the ranking, and recommend the **smallest canonical set**. A resource should earn its place; do not fill a quota.

## Evaluation criteria

1. Capability gained per hour invested
2. Practical applicability
3. Durability — likely useful in 3+ years
4. Enterprise relevance
5. Builder mindset
6. Teaching quality

Prefer primary and practitioner-authored sources. Reject SEO content, generic influencer content, prompt libraries, and certification-focused material unless exceptional. Use current authoritative sources and direct URLs.

## Required GitHub output

Repository: `halkypi/AI-Product-Leadership-Academy`

Read `AGENTS.md` before writing.

Research branch: `research/01-llm-ai-engineering-fundamentals`

This prompt: `prompts/ai-product-leadership-01-llm-ai-engineering-fundamentals.md`

Write the complete findings to: `deep-research/ai-product-leadership-01-llm-ai-engineering-fundamentals.md`

Create the research branch from `main` if it does not exist; reuse it if it does. Never write directly to `main`. If the findings file exists, update it while preserving useful prior material. Do not open a pull request unless explicitly asked.

After writing, verify the file and report path, branch, and commit SHA.

## Stop condition

STOP after completing and saving this domain. Do not generate a curriculum, learning path, timeline, or research for another domain.
