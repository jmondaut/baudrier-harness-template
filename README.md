# Baudrier harness repository

This repository holds one or more harnesses: versioned bundles of instructions, skills and Claude Code subagents for AI coding agents, in the Harness Protocol `harness.yaml` format.

Layout:

- `harnesses/<name>/harness.yaml` defines a harness (rename `example` and edit it).
- `harnesses/<name>/instructions/` holds its instruction files.
- `harnesses/<name>/skills/<skill>/SKILL.md` holds its local skills (the frontmatter `name` must match the directory name).
- `harnesses/<name>/agents/<agent>.md` holds its Claude Code subagents, declared under `x-agents` in `harness.yaml`
  (the frontmatter `name` must match the entry's `name`).

A GitHub Action (`.github/workflows/validate.yml`) validates every harness on each pull request.

To use it with Baudrier: install the Baudrier GitHub App on this repository, then register it in the Library (Add harness, enter `owner/name`). Baudrier finds every `harness.yaml` automatically. See `docs/onboarding.md` in the Baudrier platform repository for the full flow.
