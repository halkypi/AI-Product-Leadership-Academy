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
- Each prompt must tell the researcher to persist the full findings, not merely a chat summary.
- Keep `00` as the master research contract and `01`–`12` aligned with it.

## Public-repo rule

Do not add references that require access to private repositories or private company systems. The prompt must remain usable by another person with access only to this public repository and the public web.
