# Research Decisions Log

Records non-obvious choices with rationale. Append-only; don't rewrite history.

Format: `## YYYY-MM-DD -- <short title>` with **Context**, **Decision**, **Why**.

---

## 2026-04-19 -- Repository restructure to DDD-style layout

**Context**: Root had LICENSE, README, TODO, review, docs/, notes/, paper/, survey/. paper/ mixed main.tex with draft.md (Markdown duplicate), outline.md, and build artifacts. notes/ contained literature material. survey/ contained a 4-file survey instrument.

**Decision**: 
- paper/draft.md and paper/outline.md -> planning/drafts/ (superseded forms)
- paper/supplementary.md stays in paper/ (it is part of the manuscript package)
- notes/ -> literature/ (standard bounded context)
- survey/ -> experiments/src/survey/ (instrument driving future data collection)
- docs/ stays at top level because GitHub Pages requires it there

**Why**: paper/ should contain only the canonical manuscript + supplementary. Literature notes, survey instruments, and superseded drafts each belong in their proper bounded context.
