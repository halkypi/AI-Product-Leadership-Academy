# AGENTS.md

## Purpose

This repository is the public source of truth for the **AI Product Leadership Academy** research program.

The current objective is to curate the smallest set of resources that produces the largest increase in practical AI product leadership capability. This repository contains research prompts and persistent findings; it is not yet a finished curriculum.

## Repository safety

- Never commit or push directly to `main`.
- Create a feature/research branch before making tracked changes.
- Preferred branch prefixes:
  - `research/<number>-<domain>` for domain research
  - `docs/<topic>` for documentation
  - `chore/<topic>` for repository maintenance
- Never force-push unless the user explicitly requests it and understands the consequence.
- Do not open, merge, or close a pull request unless explicitly requested.
- Verify GitHub writes after mutations and report changed paths plus commit SHA.
- Preserve existing substantive research when revising a findings file. Do not silently discard prior conclusions or citations.

## Public-repository boundary

This repository is public.

- Never copy unrelated material from private repositories.
- Never include company-confidential information, PII, customer data, internal credentials, API keys, tokens, or private URLs.
- Do not expose local filesystem paths, secrets, or private connector content in research artifacts.
- If source material cannot safely be published, summarize only what is publicly supportable or omit it.

## Research integrity

Accuracy outranks tone and completeness.

- Never invent citations, URLs, authors, publication dates, benchmarks, product capabilities, or quotations.
- Prefer primary sources and practitioner-authored material.
- For fast-changing technologies, verify current facts rather than relying on memory.
- Distinguish clearly between:
  - sourced fact
  - curator judgment
  - inference
  - unresolved uncertainty
- Use direct durable URLs in persistent Markdown artifacts.
- Avoid transient chat-only citation tokens in repository files.
- Do not quote sources excessively; summarize faithfully.

## Canon criteria

Evaluate recommended resources primarily on:

1. Capability gained per hour invested
2. Practical applicability
3. Durability — likely useful in 3+ years
4. Enterprise relevance
5. Builder mindset
6. Teaching quality

Prefer the smallest sufficient canonical set. A resource must earn its place.

## Research boundaries

- Do not turn domain research into a curriculum, timeline, or learning path unless explicitly requested.
- Do not expand a domain merely because adjacent material is interesting.
- Respect the domain boundary in the numbered prompt.
- Defer good material to another domain when that is the cleaner fit.
- Reject low-signal SEO content, generic influencer content, prompt libraries, and certification-driven material unless unusually strong.

## Artifact contract

Prompts live in `prompts/`.

Research findings live in `deep-research/`.

For domains `01`–`12`, prompt and findings filenames must share the same numbered basename.

Example:

- `prompts/ai-product-leadership-05-context-engineering-rag.md`
- `deep-research/ai-product-leadership-05-context-engineering-rag.md`

Each domain research session should use its dedicated `research/<number>-<domain>` branch, write the full artifact, verify it, report the commit SHA, and stop.

## Working style

- Prefer concise Markdown and explicit decisions.
- Keep research artifacts useful to humans first.
- Do not add process, tooling, frameworks, or dependencies without a concrete need.
- When uncertainty remains, state it rather than smoothing it away.
- Read the closest nested `AGENTS.md` before editing files inside `prompts/` or `deep-research/`.
