# Agent instructions

This repository is the public GitHub profile landing page for `simpsonm09`. It holds a short
`README.md` that GitHub renders on the account's profile, plus an example environment file. It has no
code and no CI.

## Layout

- `README.md`: the profile text and the owner's public links. Keep it short; it is a landing page.
- `.env.example`: an example environment file; the real `.env` stays local and is ignored.
- `.worktreeinclude`: the files a worktree checkout carries over (`.env`).
- `docs/exceptions.md`: rules this repository cannot meet, with reasons and revisit dates.

## Commands

- `just` lists the recipes.
- `just install` installs the pinned tools from `mise.toml`.
- `just fmt` formats the repository; `just fmt-check` reports files that need it.
- `just agent-files` checks `.agents/skills` against `.claude/skills` (empty here).
- `just check` is the gate: `fmt-check` and `agent-files`.

## Invariants

- The repository stays a page: no application code, no workflows and no required checks.
- `.env` stays ignored; never commit real values, tokens or machine-specific paths.
- Do not add personal identifiers that the owner has not published here himself.

## Never

- Push to `main`. It is a public repository with a ruleset: work on a branch and merge a pull
  request.
- Change GitHub settings, repository visibility or access from a workflow, script or agent run.
