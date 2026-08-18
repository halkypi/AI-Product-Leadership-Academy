# Prompt maintenance guide

These files are designed to be handed to separate, fresh research sessions.

## Requirements

- Every numbered domain prompt must be standalone.
- Preserve the shared academy context: audience, build-first principles, evaluation criteria, source-quality bar, and GitHub persistence contract.
- Preserve the domain boundary unless the change is deliberate and documented.
- Each prompt must name its deterministic findings path under `deep-research/`.
- Each domain prompt must use a dedicated `research/<number>-<domain>` branch.
- Each prompt must forbid direct writes to `main` and must not request a PR unless the user asks.
- Each prompt must require verification of the saved file and reporting of the commit SHA.
- Keep `00` as the master research contract and keep active domain prompts aligned with it.

## Curation, not curriculum

The domain research phase is for **finding, ranking, and defending source material**. It is not for teaching the domain or writing the Academy curriculum.

Numbered research prompts should require:

1. A short domain boundary — 3–6 bullets.
2. No more than 10 ranked candidate resources.
3. A smallest sufficient canonical set — normally 2–5 resources.
4. Comparative findings of no more than 500 words, limited to what is needed to justify rankings.
5. Explicit rejected/deferred resources and cross-domain ownership where relevant.
6. Material uncertainties/version notes only.

For each candidate, request only:
- Title
- Author / organization
- Direct URL
- Estimated time commitment
- Difficulty
- Capability gained — one sentence
- Decision: `CANON`, `REFERENCE`, `DEFER`, or `REJECT`
- Why — maximum 100 words
- Main competitor it beats or why it loses — one sentence

Target 2,000–3,000 words per findings artifact with a hard maximum of 3,500 words, excluding URLs and table markup. Brevity is part of research quality.

Prompts must explicitly prohibit mini-courses, tutorials, newly invented frameworks/checklists, exercises, implementation playbooks, and learning sequences. When the research reveals a useful framework, cite the source that teaches it rather than recreating it in the findings.

## Research-to-GitHub handoff

Persisting the artifact is part of the task, not an optional follow-up.

- Research is not complete when a Deep Research report is generated.
- Research is complete only after the final findings artifact is written to the required research branch and fetched back for verification.
- If Deep Research does not expose GitHub write actions in that run, the session must finish the research and then return to the normal connected session to perform the GitHub write.
- Do not stop after producing a local/chat research report.
- If GitHub writes are genuinely unavailable after research, state that clearly and provide the complete artifact in chat.
- Never claim completion until persistence has been verified.

## Historical artifacts

Do not rewrite completed prompts/findings merely to conform to a newer prompt template unless explicitly asked. Preserve completed research as a record; apply improved research contracts to domains that have not yet been run.

## Public-repo rule

Do not add references that require access to private repositories or private company systems. The prompt must remain usable by another person with access only to this public repository and the public web.
