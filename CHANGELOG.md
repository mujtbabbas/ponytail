# Changelog

All notable changes to this standalone edition of ponytail are documented in this file.

## v1.1.0 — Standalone enhancements (2026-10-20)

- Converted the repository from a fork into a standalone edition with its own history, keeping full upstream credit.
- Added an "About This Standalone Edition" section to `README.md` with the upstream link, base-version provenance, and credit.
- Added `ENHANCEMENTS.md` documenting everything changed in this edition.
- Added `.github/dependabot.yml` for weekly GitHub Actions updates, plus npm updates for the root `package.json` (`@dietrichgebert/ponytail`).
- Added markdown linting automation (`.markdownlint.json` and the Markdown check workflow) for the documentation; the check was later scoped via `.markdownlint-cli2.yaml` so it covers this edition's own documentation instead of failing on upstream content. Upstream's `test.yml` (npm test, rule-copy/version checks, benchmark selftest) and `publish.yml` were kept as-is, so no additional code CI was needed.
- Added `.editorconfig` with standard editor settings (UTF-8, LF, 2-space indent).

## v1.0.0 — Upstream baseline (2026-10-20)

- Clean standalone baseline of [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) at upstream release v5.3.2 (snapshot commit `09c434ab73ca43761c5d8b0c5d341926c2fba710`, upstream HEAD dated 2026-10-18).
- Fork history severed; all 214 files and the MIT licence (`LICENSE`) preserved as-is, including the 46 binary image assets under `assets/`.
