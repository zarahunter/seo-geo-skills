# Changelog

All notable changes to the AI SEO / GEO skill are documented here.

## [1.1.0] — 2026-06-20

Added the `on-page-seo` skill and packaged both skills together.

- New **`on-page-seo`** skill: search-intent matching, keyword selection and placement, title tags, meta descriptions, URL slugs, heading hierarchy, internal linking, alt text, an on-page checklist, and copy-paste templates.
- **Two-pass method**: `on-page-seo` (ranking) and `ai-seo` (GEO/citation) now cross-reference each other so a single "fully optimize this" request runs both.
- Plugin renamed `ai-seo` → **`seo-geo`** to host both skills under one install (`seo-geo@eduk8agentic`).

## [1.0.0] — 2026-06-19

Initial public release.

- AI SEO / GEO skill with six tasks: audit, optimize, create, monitor, entity presence, MENA / Arabic.
- Reference library: `content-patterns`, `platform-factors`, `measurement`, `entity-presence`, `hard-cases`, `mena-arabic`, `research-stats`.
- Full worked example (audit → before/after rewrite) for quality calibration.
- Passage-diff audit method, measurement-execution paths (live / tool-assisted / operator-paste), and hard-case coverage (uneditable listicles, wrong parametric facts, negative sentiment, local / multi-location, YMYL).
- Dual install: Claude Code plugin marketplace and manual.
