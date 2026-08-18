# AI Product Leadership Academy — Canonical Reading List Research Prompt

## Purpose

Construct the canonical reading/resource set for an AI Product Leadership Academy.

The goal is **not** to create a curriculum. The goal is to identify the **smallest set of resources that produces the largest increase in practical capability**.

## Problem

Product leaders are increasingly expected to lead AI-enabled products, but many lack practical experience using AI, partnering with engineering/data science, evaluating opportunities, and building solutions themselves.

## Hypothesis

A hands-on, build-first academy can produce AI-native product leaders who can:

- Use AI daily to improve effectiveness
- Identify and prioritize AI opportunities
- Lead AI-enabled products
- Partner effectively with engineering and data science
- Apply responsible AI governance
- Build working prototypes independently

## Audience

- Product Managers
- Senior PMs
- Principal PMs
- AI-minded builders

## Environment

- Python-first
- Snowflake-centric
- GitHub Copilot available
- Enterprise setting
- Strong data culture

## Principles

### Do

- Practical over theoretical
- Product-first
- Python-first
- Snowflake-first
- Copilot-native
- Learning by building
- Jeremy Howard-style projects
- Frank Kane-style hands-on labs

### Don't

- Academic ML
- Deep math
- Certifications for their own sake
- Prompt-engineering theater
- AI literacy without application

## Evaluation criteria

For every recommended resource evaluate:

1. Capability gained per hour invested
2. Practical applicability
3. Durability — likely still useful in 3+ years
4. Enterprise relevance
5. Builder mindset
6. Teaching quality

For every recommendation provide:

- Title
- Author / organization
- URL
- Time commitment
- Difficulty
- Capability gained
- Why it belongs in the canon
- Why competing resources were rejected

## Source-quality constraints

- Prefer primary sources
- Prefer practitioner-authored material
- Reject SEO content
- Reject generic influencer content
- Reject certification-focused content unless exceptional
- Reject resources below the quality bar represented by strong material from fast.ai, Anthropic Engineering, Ethan Mollick, OpenAI developer documentation/Cookbook, Snowflake Documentation, NIST AI RMF, and Frank Kane
- For fast-changing technical material, verify current facts and current URLs

## Research process

### Phase 1 — capability domains

Identify and rank the capability domains that matter.

STOP after ranking the domains.

### Phase 2 / 3 — domain-by-domain curation

For one domain at a time:

- Produce no more than 10 candidate resources
- Rank them
- Defend the ranking
- Explain why alternatives were rejected
- Recommend the smallest canonical set for that domain

Do not generate a curriculum, learning path, or timeline.

Act as a discerning curator, not an instructional designer.

## GitHub source of truth

Repository: `halkypi/AI-Product-Leadership-Academy`

Default branch: `main`

Repository guide: `AGENTS.md`

Master prompt: `prompts/ai-product-leadership-00-academy.md`

Phase 1 findings: `deep-research/ai-product-leadership-academy.md`

Domain prompts: `prompts/ai-product-leadership-01-*.md` through `prompts/ai-product-leadership-12-*.md`

Domain findings belong in matching files under `deep-research/` using the same numbered basename.

Example:

- Prompt: `prompts/ai-product-leadership-05-context-engineering-rag.md`
- Research branch: `research/05-context-engineering-rag`
- Findings: `deep-research/ai-product-leadership-05-context-engineering-rag.md`

## Required behavior for every domain research session

1. Treat the numbered prompt as standalone; do not rely on chat history.
2. Read `AGENTS.md` before mutating the repository.
3. Research that domain only.
4. Use the prompt's dedicated `research/<number>-<domain>` branch. Create it from `main` if it does not exist; reuse it if it does.
5. Never commit or push directly to `main`.
6. Write the **complete research findings** — rankings, direct URLs, rationale, rejected alternatives, uncertainty, and final canonical set — to the matching `deep-research/` file.
7. If the findings file already exists, update it rather than creating a duplicate, preserving useful prior material.
8. Do not open a pull request unless explicitly asked.
9. Verify the saved GitHub file and report its path, branch, and commit SHA.
10. Do not persist merely the prompt or a summary; persist the full research artifact.

The numbered prompts may reference this master prompt for provenance, but each must repeat enough context to run independently.
