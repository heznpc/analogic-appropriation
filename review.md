# analogic-appropriation — Review (2026-04-11)

## 1. 커밋 톤이 주장을 일관되게 지지하는가?

**판정: 매우 일관됨 + 가장 잘 정리된 commit history (10 commits, 2026-03-17 → 04-07).**

```
b7622af chore: add .zenodo.json for DOI minting                    (2026-04-07)
fbb9331 feat: word reduction markers, comparison table, citations  (2026-03-26)
5f5d9ac chore: gitignore local files                               (2026-03-24)
33aa4e5 Strengthen draft for NMS submission                        (2026-03-22)
b7bc318 Update draft                                               (2026-03-18)
c169d37 Add i18n support: 8 languages                              (2026-03-17)
dd4367e Trigger GitHub Pages build                                 (2026-03-17)
308bf02 Add GitHub Pages landing page                              (2026-03-17)
62b5d6d Add CC BY 4.0 license and update README header             (2026-03-17)
2bc2a07 Initial commit: paper draft, survey instruments            (2026-03-17)
```

진화 패턴:
- **Day 0 (3/17)**: 7,200단어 draft + survey 도구 + 8개국 cultural evidence + GitHub Pages 랜딩 + CC BY 4.0 + i18n(8개 언어) — *모든 인프라가 한 번에 들어옴*. 최초 하루 안에 학술/공개/국제화 모두 셋업.
- **Day 5 (3/22)**: "Strengthen draft for NMS submission" — 11개 변경(abstract 150단어 압축, Era 3 commercialization 데이터 추가, 9개 신규 인용 통합, Russia를 boundary case로 재분류, KADOKAWA 일본 부재 보강, COPPA 2025, alphabetize references 등). **단일 commit에 11개 학술적 결정** — 이는 학술 워크플로에서 매우 드물게 빈도 높은 self-revision.
- **Day 9 (3/26)**: "word reduction markers, comparison table, new citations" — 12,200 → 8,000단어 압축 작업 시작. supplementary.md 분리(301줄). **MOVE/COMPRESS 마커를 직접 본문에 박아서 reviewer는 못 보지만 author는 추적 가능**한 워크플로. 새 citation에는 "NEEDS VERIFICATION" 플래그까지 명시.
- **Day 21 (4/07)**: Zenodo DOI 발행 준비 — preprint timestamp 확보 의지.

톤의 일관성:
- 핵심 가설(analogic appropriation, 3 eras, dominant interface effect, scope conditions)이 **모든 commit에서 단조 강화**. 새로운 evidence가 들어와도 framework 자체는 흔들리지 않음.
- *Self-correction 디시플린이 발군*: Russia를 "evidence absent → counterexample"로 reclassify, Japan absence를 KADOKAWA로 nuanced explanation, scope condition (b)를 "restricted access → expressive gap"으로 폭넓게 재정의 등. 모두 *반증 가능성을 인정하면서도 framework를 강화*하는 방향.
- TODO.md(183줄)에 P0/P1/P2/Experiments까지 4단 우선순위로 자기 관리. **IRB exempt 경로(45 CFR 46.104(d)(2)(i))까지 사전 식별**하고 commercial IRB 옵션도 준비. 학술 인프라 인식이 매우 높음.

전체적으로 본 survey 21개 paper 레포 중 **commit discipline TOP 3 후보**.

## 2. 부가 서비스 품질

**판정: 부가 서비스 존재 — GitHub Pages 랜딩 + i18n + Zenodo DOI 준비. 품질 양호.**

서비스 1: **GitHub Pages 랜딩 (`docs/index.html`, 599줄)**
- vanilla JS only, zero dependencies
- dark mode auto, responsive layout, Georgia/Times serif
- Open Graph 메타데이터 포함 (소셜 공유 시 카드 표시)
- abstract + 3-era framework + 7-country evidence + repo links 모두 포함
- **i18n 8개 언어 지원**: EN, KO, JA, PT, TR, ID, DE, HI — *survey 대상 8개국과 정확히 매칭*. 브라우저 lang 자동 감지 + localStorage persistence + data-i18n 속성으로 모든 콘텐츠 번역.

서비스 2: **Zenodo DOI 발행 준비 (`.zenodo.json`)**
- 21줄 깔끔한 메타데이터: title, creators, keywords 6개, CC BY 4.0, preprint type, open access
- 첫 release 시 자동 DOI 발행 가능

서비스 3: **Survey instruments (4 docs)**
- `design.md` 291줄: exploratory sequential mixed-method 설계, Phase 1+2+3 분리, Prolific 핵심 5국 + 대학 네트워크 보충 3국, $2.50/명 보상, 8개 언어 protocol
- `analysis_plan.md` 298줄: TOST equivalence testing, MG-CFA 측정 불변성, Bayesian 사전등록 계획
- `questionnaire_ko.md`, `questionnaire_en.md` 각 199줄: 2-stage screener (자유 회상 → 유도 재인) — 회상 편향 통제

품질 평가:
- 순수 *논문* 레포가 아니라 **소형 academic project hub**로 운영. 본 survey 21개 paper 중 가장 *완성도 높은 부속 인프라*.
- 약점: 서비스가 모두 정적/문서. 데이터 수집·분석 코드(R/Python script)는 0개. survey 자체가 아직 IRB 통과 전이라 실제 데이터 0건.
- i18n 8개 언어 *UI*는 완성됐지만 *설문지* 8개 언어 번역은 아직 KO/EN만 — design.md 명시. 즉 landing은 ready, instrument는 not yet.

## 3. 고도화 가능 파트

높은 우선순위 (NMS 투고 직결):
1. **Word count 8,000 압축 완료** — 현재 12,200→8,000으로 줄여야 NMS "will not be considered" 회피. supplementary.md(301줄)에 분리된 내용 외 추가 1,500-2,000단어 축소가 필요. main.tex(630줄)와 draft.md(365줄)의 동기화도 필요(현재 둘이 별도 진화).
2. **IRB exempt 신청** — TODO P0 #1. Solutions IRB 또는 Advarra 통한 1-2주 exempt determination이 commercial 경로. Prolific은 IRB 증빙 없이는 패널 사용 불가.
3. **설문지 6개 언어 번역** — JA/DE/PT/ID/HI/TR. team-based translation (CSDI) 권장. 현재 EN/KO만 완성. **landing UI는 8개 다 됐는데 instrument는 2개**가 비대칭.
4. **Pilot 80명 (8개국 × 10명) 실행** — TODO P1 #5. 본조사 1,000명 전 단계.
5. **MediArXiv 프리프린트 게재** — Word limit 무제한이라 12,200 전체 버전을 timestamp 확보 차원에서 즉시 게재 가능. NMS와 별개 진행 가능.

중간 우선순위:
6. **A-β1 일본 부재 심화 조사** — 2ch/Pixiv/Amazon 텍스트 마이닝 + 일본 세대별 인터뷰. KADOKAWA 백과사전 데이터를 본문에서 단 2문장으로 처리하고 있는데, *부재가 부재가 아닐 수 있다*는 발견은 framework의 중요한 falsifier. 후속 paper로 분리 가능.
7. **A-β2 성별 차원 교차분석** — 현재 framework가 "남아 중심" 편향을 인정하고 있음. KADOKAWA 여아 데이터로 균형 회복 필요. 최소한 supplementary에 1쪽 분량.
8. **A-β3 Roblox 게임 design 마이크로민족지** — Era 2 evidence가 textual인데, 실제 Roblox top 500 combat games 메타데이터 분석으로 Era 2 evidence를 *증강*. CSV 1개로 reviewer 신뢰도 +1.
9. **Africa/MENA gap을 *부재의 분석적 의미*로 정식화** — Section 5.3에 이미 언급되지만 1쪽으로 expand. Chinyowa(2024) 인용 + Khashkhashah/Tawleh 전통게임 cf.

낮은 우선순위:
10. OSF preregistration (TOST/Bayesian template).
11. supplementary.md의 method section을 영문 LaTeX appendix로 통합.
12. 한국 ddakji, flipbook battles, 텍스트 RPG 변종을 분류 도입.

## 4. 학술적 / 시장 가치 (글로벌, 2026-04-11 기준)

### 학술적 가치: **상위권 (working paper 기준 상위 ~10%, 분야 한정 시 top 5%)**

타이밍:
- **Italian brainrot은 2025-2026의 정점 trend**: KADOKAWA 일본 출판, Steal a Brainrot Roblox 60B visits, Skifidol/Spin Master IP — 이 모든 데이터가 *paper 안에* 통합돼 있음. 해당 분야에서 *현재 시점*에 가장 잘 정리된 학술적 분석.
- New Media & Society의 최근 편집 방향(Divon & Ebbrecht-Hartmann 2025 "playability")과 정확히 align. NMS reviewer가 자연스럽게 호의적일 가능성.
- "analogic appropriation"이라는 용어가 *unoccupied*. 인용 가능한 새 vocabulary 확보.

차별점:
- **Cross-cultural scope (7개국 + 2 boundary + 1 absent)** — Burn & Richards 2014의 영국 단일국가를 직접 확장. 학술적 lineage가 명확.
- **Three-era diachronic analysis (1970s~2000s / 2010s~2020s / 2025~)** — 시대 비교 framework가 단순 anecdote 아닌 systematic.
- **Strong theoretical synthesis**: Corsaro(interpretive reproduction) + Caillois(agon/mimicry) + de Certeau(tactics) + Vygotsky(ZPD) + Bolter & Grusin(remediation) + Burn & Richards (predecessor). 6개 framework를 1개의 새 개념으로 통합.
- **Methodological maturity**: TOST equivalence testing + MG-CFA + Bayesian + LCA를 사전 명시. 단순 ethnography가 아니라 양적 검증 계획까지.
- **Self-aware boundary cases**: Russia/India를 evidence가 안 맞을 수 있는 case로 *프레임 내부에* 포함. Japan을 *부재의 부재*로 nuanced. reviewer가 "왜 이건 안 다뤘냐"고 묻기 어려운 구조.

위험:
- **NMS word limit (8,000)**이 결정적 게이트. 현재 12,200 → 50% 초과. 압축 작업이 *실질적*으로 끝나지 않으면 desk reject.
- **IRB 미통과 + 데이터 0건** — 현재 paper는 *theoretical*이고 "planned 8-country survey"는 약속. NMS reviewer가 "empirical data 없이는 reject"라고 할 수 있음. *Theoretical paper로서 value*를 명시적으로 강화 필요(현재 conclusion에서 약함).
- **Independent researcher 단독 저자** — 현재 영문 명의 "heznpc". real name 노출이 NMS 표준. anonymization 단계에서 정식 명의 결정 필요.
- **8개국 균형 표집 위험** — Prolific은 한국·인도네시아·인도·터키 패널이 부족. 보충 3국이 *대학 네트워크*인데 IRB 협력이 추가 부담.

게재 전망:
- *New Media & Society* (IF 8.6, top media journal): **realistic, 50-60%**. Burn & Richards 후속 + cross-cultural + 시의성 + framework 명료. word limit만 넘기면 강력한 후보.
- *Convergence* (SAGE, IF 4): **70-80%**. transmedia/remediation 앵글에 적합.
- *International Journal of Cultural Studies* (SAGE, ~8,000): **65-75%**. cross-cultural 포지셔닝.
- *Journal of Children and Media* (Routledge): **70-80%**. 직접 적합.
- CHI 2027: design implications 추가 시 가능.

### 시장 가치: **중상위 (학술적 임팩트는 강하지만 market product화는 어려움)**

- **언론/대중 어필**: "전세계 아이들이 종이에 캐릭터 그리고 싸우는 놀이를 독립 발명했다"는 한 줄 명제는 NYT/Atlantic/Guardian/Aeon이 픽업하기 좋은 톤. Italian brainrot이 *세대 식별자*로 자리 잡고 있어 픽업 가능성 높음.
- **교육·디자인 컨설팅**: CHI 트랙으로 가면 children's media design, edtech UX에 직결. KADOKAWA 같은 IP 회사 자문 가능.
- **놀이 박물관·연구소**: Strong Museum of Play(Rochester), 한국의 어린이대공원, 일본 게임 박물관 등 cultural heritage 영역에서 인용 가능.
- **GitHub Pages 랜딩 + 8개 언어 i18n**의 *visibility 인프라*가 잘 깔려 있어 viral potential이 있음. 이 organisation 수준은 working paper 중에 매우 드묾.
- 한계: paper 그 자체가 product이지 별도 SaaS/tool이 없음. survey instrument를 reusable open-science kit으로 패키징하면 가치 +1.

### 종합 평점 (2026-04-11)

| 축 | 점수 | 코멘트 |
|---|---|---|
| Originality of framing | 9/10 | "analogic appropriation" + 3 eras |
| Literature integration | 9/10 | 6개 framework 통합 + 직접 predecessor 인정 |
| Empirical contribution | 4/10 | survey 설계는 완성, 데이터 0건 |
| Theoretical maturity | 9/10 | 6 framework synthesis + scope conditions |
| Self-criticism / falsifiability | 9/10 | boundary cases + Japan absence + NEEDS VERIFICATION 플래그 |
| Repo health | 9/10 | GitHub Pages, i18n, Zenodo, IRB plan, 10 commits |
| Cross-cultural balance | 7/10 | Africa/MENA gap 인정, 보강 필요 |
| Timing | 10/10 | Italian brainrot 정점 |
| Submission readiness | 6/10 | NMS word limit 미달성 |
| **Overall (working paper)** | **8.0/10** | "투고 직전 단계의 잘 갖춰진 연구" |

핵심 격언: **"Word limit 8,000과 IRB exempt 두 개의 게이트만 통과하면 NMS top venue에 진짜로 도착한다."** 본 survey 21개 중 *학술 인프라 organisation* 가장 잘 된 케이스. Italian brainrot 모멘텀이 살아 있을 때 압축 + IRB + 파일럿 80명 → 6개월 안에 게재 시도 가능.
