---
project: swag-guide
url: https://swag-guide.shellnode.lol
vps: ghost
port: 80
stack: single-file HTML, nginx:alpine, SWAG
standards_version: "2.0"
security: done
ux_ui: not_started
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
- Updated Dockerfile: added explicit EXPOSE 80, CMD, RUN rm -rf, nginx.conf COPY
- Created nginx.conf with security headers, gzip, dotfile block
- Created .dockerignore
- Created .gitignore
- Created docker-compose.yml with SWAG labels
- Added README.md

### Incomplete
- UX/UI audit not started

### Blocked — Needs Matt
- None

## Backlog
- [P2] UX/UI audit

## Done
- [x] Dockerfile hardened — 2026-03-09
- [x] nginx.conf created — 2026-03-09
- [x] .dockerignore created — 2026-03-09
- [x] .gitignore created — 2026-03-09
- [x] docker-compose.yml added — 2026-03-09
- [x] README.md added — 2026-03-09

## Decisions Log
- "qa-audit/ directory and *.md reports excluded from docker image via .dockerignore — local audit artifacts, not web assets." (2026-03-09)
- "Markdown reports (frontend-architecture-report*.md, security-audit-report.md) are untracked — left as-is." (2026-03-09)

## Project Notes
- Single-file HTML bento checklist for SWAG DNS setup
- Local audit report files: security-audit-report.md, frontend-architecture-report.md, qa-audit/ — these are untracked
- Remote repo is named swag-dns-setup (different from local dir swag-guide)
