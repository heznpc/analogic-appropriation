# Analogic Appropriation

Research Program: 6 (Analogy / theory layer)
Status: Draft — not submitted (NMS-format manuscript in compression pass; survey IRB pending)
Relationship to other work: Theory layer for Program 6; companions are [pythia](https://github.com/heznpc/pythia) (divination ↔ LLM analogy) and [whetstone](https://github.com/heznpc/whetstone) (education science).

---

Children in culturally distant settings — Korean *gonghchaek geim*, American Pencil Wars, Turkish *Kareli Defterde Imparatorluk Oyunu*, Indonesian *Perang-perangan* — independently create characters on paper and pit them against peers' creations in rule-governed combat. This paper proposes **analogic appropriation**: children tactically reconstruct inaccessible media interfaces into available material substrates, and the form of this play tracks the dominant media of each era while its structural core (participatory character creation + agonistic structure + peer sharing) persists. The framework synthesises Corsaro's interpretive reproduction, Caillois's agon/mimicry, and de Certeau's tactics across three media eras: analog appropriation (1970s–2000s), digital democratization (2010s–2020s), and AI-mediated folk art (2025–, e.g. Italian brainrot).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Currently implemented

- `paper/main.tex` — 630-line LaTeX manuscript (~12,200 words). Theoretical framework + cross-cultural documentary evidence from 5 core countries (Korea, US, Turkey, Indonesia, Philippines) + 2 boundary cases (Russia, India) + theoretical discussion of Japan's apparent absence + 3-era diachronic analysis.
- `experiments/src/survey/` — 4-file instrument package (`design.md`, `questionnaire_ko.md`, `questionnaire_en.md`, `analysis_plan.md`). Korean and English questionnaires complete.
- `literature/cultural_evidence.md`, `literature/sources.md` — country-by-country evidence archive driving the documentary analysis.
- `submissions/nms-2026/NOTES.md` — venue compression strategy (12,200 → 8,000 words for SAGE Harvard / NMS double-blind format) and pre-submission checklist.
- `planning/TODO.md` — argument-completion tasks, P0/P1/P2 prioritised; separated from the submission checklist by design.

## Planned

- IRB determination — Exempt Cat 2(i) (45 CFR 46.104(d)(2)(i)) via commercial IRB (Solutions IRB or Advarra) for the adult survey; minor interviews split into a separate protocol so the survey is unblocked.
- Survey translations to 6 additional languages (Japanese, German, Portuguese-Brazil, Indonesian, Hindi/English, Turkish) using team-based translation with an adjudicator role (CSDI guideline).
- Cognitive interviews per translation (5–8 per language) before Phase-1 pilot.
- 8-country pilot via Prolific (n ≈ 10/country) → core-country n = 120 (MG-CFA invariance buffer).
- MediArXiv preprint of the uncompressed 12,200-word manuscript, posted before NMS submission for timestamp.
- Word-limit compression pass to 8,000 words for NMS (methodology + analysis plan moved to supplementary; Three-Eras evidence compressed to a summary table with per-country prose tightened).
- OSF preregistration adapted from the Social Psychology template with TOST + Bayesian-TOST hybrid adaptations.

## Design intent

- **`paper/main.tex` is the single source of truth.** Venue-specific adaptations live in `submissions/<venue>/` and never edit the canonical manuscript. This keeps the 12,200-word argument intact across multiple parallel submission targets.
- **DDD-style separation.** `paper/` = domain (manuscript), `experiments/src/survey/` = application (the instrument that will drive data), `literature/` = external knowledge, `planning/` = meta-work, `docs/` = public landing. The survey package lives under `experiments/` because it *is* the future-data driver, not project documentation.
- **Three-era structure is load-bearing.** "Analogic appropriation" is named not for the analog era alone but for the cross-era invariant: each era's children appropriate the dominant media interface onto whatever substrate is locally accessible. The theoretical contribution falls apart if the framework is read as analog-only.
- **Documentary evidence first; survey second.** The manuscript stands as a theoretical paper grounded in documentary analysis; the planned cross-cultural survey is a separate, falsification-oriented test of the framework, not its evidentiary basis. This is why the IRB blocker does not gate the NMS submission.
- **Single LaTeX file deliberately.** No multi-file `\input{}` structure — keeps the manuscript trivially submittable to journal portals and reviewable as a single artifact.

## Non-goals

- **Not an ethnography.** Documentary analysis of digital archives across seven countries — not fieldwork, not participant observation.
- **Not minor-focused.** The survey targets adults' childhood-play memories (Exempt Cat 2(i) path). Direct study of children is explicitly out of scope for the immediate submission; that work is the planned, separately-IRB'd extension.
- **Not a quantitative validation of the framework.** The cross-cultural survey is the planned validation step. The current paper makes a theoretical-framework claim grounded in documentary evidence; quantitative invariance testing is a follow-up.
- **Not a digital-natives argument.** The claim is structural recurrence across analog, digital, and AI-mediated eras — not a "digital changed everything" or "analog was authentic" narrative.
- **Not a single-medium argument.** Paper-only or AI-only readings miss the cross-era invariant that the framework names.

## Redacted

- No external persons, internal cases, or institutional identifiers are involved in this repository.
