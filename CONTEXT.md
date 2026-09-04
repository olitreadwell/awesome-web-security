# qazbnm456/awesome-web-security context
> refreshed 2026-09-04 | upstream default: master @ f2811db

## Identity & policies
- upstream: qazbnm456/awesome-web-security, default branch master, primary language Markdown (awesome list, security)
- English-first: yes (README + zh + jp generated from YAML; issues/maintainer conversation English)
- CLA/DCO: none
- AI-assisted PR policy: banned? no — no AI/trivial bans found (vetted 2026-08-24); auto-review bot grades PRs (RUBRIC.md)
- signed commits required: no
- PR template: present (.github/PULL_REQUEST_TEMPLATE.md, resource-add shape)
- external tracker: GitHub only
- Data model: YAML-first. README.md/README-zh.md/README-jp.md are GENERATED from data/categories.yml + data/entries/*.yml via `python3 scripts/generate.py`. Do NOT hand-edit READMEs. Validate: `python3 scripts/verify_schema.py`. Dead-link triage: `scripts/ci/triage_dead_links.py`.

## Conventions (verified from merged PRs)
- branch naming: mixed — `fix/*` (fix/juice-shop-repository-link), `fix-*` (fix-github-enterprise-rce-link), `add-*`, `ci/*`
- commit style: conventional commits (`fix(data):`, `ci:`, `docs:`) and plain imperative; e.g. `docs: restore 2 dead digests link(s) via Wayback`, `fix: upgrade http:// links to https://`
- how outside PRs get merged: responsive; recent external merges (SpiderSuite, Proxelar, State of TLS, dead-link fixes #182/#183); maintainer merges external dead-link/URL-fix PRs

## Maintainer picture
- maintainer: qazbnm456 (Boik Su), merges external and bot-grade PRs; active, very recent pushes (2026-08-21)
- areas in flight: CI/review pipeline (diff-sentry, pr_review.py) — avoid CI internals

## Issue-area health
- Issue #212 "Link health report" (label health/link-check): OPEN rolling issue, updated daily by bot, ~196 dead-link errors. Maintainer-engaged channel for dead-link fixes; CONTRIBUTING documents the triage_disposition (active / dead / archived-only / quarantined + archive_url).
- Other open issues: #229 (pr_review.py GitHub Models retired), #234/#232 (resource proposals) — not picks.

## Gap ledger (dedupe — READ FIRST, never re-pick)
- 2026-09-04 dead-links batch (this run) — outcome: pr-opened — fixed phrack JS paper URL; flagged theori/brokenbrowser/sigpwn-domato/hahwul entries archived-only (dead + Wayback-archived, per maintainer's documented disposition)

## Mined gaps (discovered, not yet attempted)
- 2026-09-04 dead-link batch: phrack JS engine paper URL moved to phrack.org/issues/70/...; theori escaping-chrome-sandbox, brokenbrowser SOP/UXSS, sigpwn Domato, hahwul self-XSS all dead + Wayback-archived → archived-only — status: attempted (pr-opened)
- 2026-09-04 payloadbox org + its payload-list repos all 404 (org API shows public_repos but every repo/profile 404) — candidate for a later archived-only/redirect cleanup — status: proposed (NOT in this PR)
