# Analogic Appropriation

**Cross-cultural study of children's paper combat play across three media eras**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Project Overview

전세계 아이들이 독립적으로 "종이에 캐릭터를 그려서 싸우는 놀이"를 발명했다는 가설을 검증하고,
이 놀이가 시대별 지배 매체를 따라 재매개(remediation)되는 패턴을 분석하는 연구 프로젝트.

## Target Publication

- **Preprint**: MediArXiv (media/communication studies open archive)
- **Journal**: New Media & Society (SAGE) 또는 Convergence
- **Alternative**: CHI/CSCW (HCI route — design implications 추가 시)

## Timeline

| Phase | Task | Target |
|-------|------|--------|
| Phase 1 | 이론 분석 논문 초고 | 2026 Q2 |
| Phase 2 | 교차문화 설문 실시 (10개국+) | 2026 Q2-Q3 |
| Phase 3 | 데이터 분석 + 논문 완성 | 2026 Q3 |
| Phase 4 | MediArXiv 프리프린트 게재 | 2026 Q3 |
| Phase 5 | 저널 투고 | 2026 Q4 |

## Directory Structure

```
analogic-appropriation/
├── paper/                        Domain -- manuscript source of truth
│   ├── main.tex
│   ├── references.bib
│   └── supplementary.md
├── experiments/
│   └── src/survey/               Survey instrument package
│       ├── design.md
│       ├── questionnaire_ko.md
│       ├── questionnaire_en.md
│       └── analysis_plan.md
├── literature/
│   ├── sources.md                수집된 소스/증거
│   └── cultural_evidence.md      국가별 증거 아카이브
├── planning/
│   ├── TODO.md, review.md, decisions.md
│   └── drafts/                   draft.md, outline.md (superseded)
└── docs/                         GitHub Pages landing
    └── index.html
```

## Key Thesis

1. "전투 놀이"와 "그리기"는 각각 교차문화적 보편 행동이며, 이 둘이 "종이"라는 접근성 높은 매체 위에서 결합하는 것은 독립발명(independent invention)의 전형적 사례이다.
2. 이 놀이의 구체적 형태는 각 시대의 지배적 매체 인터페이스를 모방(remediate)한다:
   - 2D RPG 시대 → 공책 RPG (스탯창, 상점, 사냥터)
   - UGC 플랫폼 시대 → 로블록스/마크 직접 제작
   - AI 생성 시대 → Italian brainrot (AI 캐릭터 창조)
3. 매체는 변하지만 핵심 충동("내 캐릭터를 만들어 싸우고 싶다")은 불변이다.
