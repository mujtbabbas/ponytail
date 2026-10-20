# Enhancements — Standalone Edition Changelog

Upstream: https://github.com/DietrichGebert/ponytail
Maintainer of this edition: Syed Mujtaba Abbas (@mujtbabbas)

## v1.1.0 — Enhancement release (2026-10-20)
- Added "About This Standalone Edition" section to README.md with upstream
  link, base version provenance, and credit.
- Added this changelog (ENHANCEMENTS.md).
- Added .github/dependabot.yml (weekly GitHub Actions updates, plus npm
  for the root package.json, @dietrichgebert/ponytail).
- Added .markdownlint.json and .github/workflows/markdown-check.yml
  (markdown linting automation for the documentation; upstream test.yml —
  which runs npm test, rule-copy/version checks and the benchmark
  selftest — and publish.yml kept as-is, so no additional code CI was
  needed: the real test tooling is already covered upstream).
- Added .editorconfig (standard editor settings: UTF-8, LF, 2-space indent).

## v1.0.0 — Baseline (2026-10-20)
- Clean standalone baseline of DietrichGebert/ponytail at upstream release
  v5.3.2 (snapshot commit 09c434ab73ca43761c5d8b0c5d341926c2fba710,
  upstream HEAD dated 2026-10-18).
- Fork history severed; all 214 files and the MIT licence (LICENSE)
  preserved as-is. Note: 46 binary image assets under assets/ are part of
  the baseline (largest: assets/band/board.png, 1146442 bytes) — a
  connector snapshot push cannot carry binaries, so they will need a
  non-connector route at push time.
