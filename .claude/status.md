---
project: swag-guide
url: https://swag-guide.shellnode.lol
vps: ghost
port: 80
stack: single-file HTML, nginx:alpine, SWAG
standards_version: "2.0"
security: done
ux_ui: done
repo_cleanup: done
readme: done
last_session: "2026-03-09"
has_blockers: false
---

# Project Status — swag-guide

## Last Session
Date: 2026-03-09
Agent: Claude Code

### Completed
- UX/UI audit complete
- Fixed --muted contrast: #666666 → #808080 (WCAG AA compliant on both dark backgrounds)
- Added whole-row click handler: clicking checklist text now toggles checkbox
- Pushed to origin (b5e4cdd)

### Incomplete
- None

### Blocked — Needs Matt
- None

## Backlog
- [P3] Add Open Graph meta tags (og:title, og:description, og:url)
- [P3] Add inline SVG favicon

## Done
- [x] Dockerfile hardened — 2026-03-09
- [x] nginx.conf created — 2026-03-09
- [x] .dockerignore created — 2026-03-09
- [x] .gitignore created — 2026-03-09
- [x] docker-compose.yml added — 2026-03-09
- [x] README.md added — 2026-03-09
- [x] UX/UI audit: muted contrast fix + row-click fix — 2026-03-09 — commit b5e4cdd

## Decisions Log
- "qa-audit/ directory and *.md reports excluded from docker image via .dockerignore — local audit artifacts, not web assets." (2026-03-09)
- "Markdown reports (frontend-architecture-report*.md, security-audit-report.md) are untracked — left as-is." (2026-03-09)
- "Mobile overflow from QA findings already resolved in prior commits (4945a04, d25ca93) — code uses opacity:0 checkboxes, min-width:0 on cards, flex-wrap on domain-row." (2026-03-09)
- "OG tags and favicon left as P3 backlog — not worth holding up audit for P3 items." (2026-03-09)

## Project Notes
- Single-file HTML bento checklist for SWAG DNS setup
- Local audit report files: security-audit-report.md, frontend-architecture-report.md, qa-audit/ — these are untracked
- Remote repo is named swag-dns-setup (different from local dir swag-guide)
