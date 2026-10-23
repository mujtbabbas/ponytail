# Reader's Guide — ponytail

## What this project is

**Ponytail** is a plugin that gives your AI coding agent the instincts of a
lazy senior developer: *"He says nothing. He writes one line. It works."*
Where most agents over-build — new abstractions, boilerplate, speculative
options — Ponytail pushes back toward the smallest change that solves the
problem, and ships rebuilt **review** and **audit** workflows around the same
philosophy. The README backs the pitch with numbers and before/after
examples. It works with around 20 agent tools.

## How the content is organised

- `skills/` — the skill set, one folder per skill: `ponytail` (the main
  behaviour), `ponytail-review`, `ponytail-audit`, `ponytail-debt`,
  `ponytail-gain` and `ponytail-help`.
- `commands/` — the slash commands the plugin adds; `hooks/` — its lifecycle
  hooks; `__init__.py` — the plugin's Python core.
- **Per-tool packaging folders** — the same plugin packaged for each host:
  `.claude-plugin/`, `.codex-plugin/`, `.cursor/`, `.windsurf/`,
  `.clinerules/`, `.opencode/`, `.agents/`, `.kiro/`, `.qoder/`,
  `.devin-plugin/`, `.grok-plugin/`, `.kimi-plugin/`, `.openclaw/`, plus
  `gemini-extension.json`, `opencode.json`, `plugin.json`/`plugin.yaml` and
  `pi-extension/`.
- [`README.md`](README.md) — the pitch and manual: **Numbers**,
  **Before / after**, **How it works**, **The prompt** (the actual behaviour
  text, readable in the repo), **Install**, **Commands**, **FAQ**.
  [`INSTALL.md`](INSTALL.md) carries the long per-tool install instructions,
  with `after-install.md` for the finishing steps.
- `benchmarks/` — the measurements behind the README's numbers; `examples/`
  and `docs/` — worked examples and documentation; `i18n/` — translations;
  `tests/` — the test suite.

## How to use it

1. Find your agent tool in [`INSTALL.md`](INSTALL.md) and install the matching
   package (or use the README's short **Install** path).
2. Work as normal — the `ponytail` skill steers the agent toward minimal,
   working diffs; call the review/audit commands when you want the same lens
   applied to existing code.
3. Read **The prompt** section of the README if you want to understand (or
   borrow) exactly what the agent is being told.

## About this standalone edition

This repository is a standalone edition of
[DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail),
converted from a fork into its own repository and enhanced in place. See
[`ENHANCEMENTS.md`](ENHANCEMENTS.md) for what this edition adds and
[`CHANGELOG.md`](CHANGELOG.md) for its version history (v1.0.0 upstream
baseline, v1.1.0 enhancements). All original work belongs to the upstream
contributors; licence MIT (see `LICENSE`).
