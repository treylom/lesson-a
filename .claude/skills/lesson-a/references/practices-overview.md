---
disable-model-invocation: true
---

# 성우하이텍 AI 마스터 과정 — 강사 참조 자료

> **구조**: 실습 단위(Practice) 기반. 교시/주차 구분 없이 강사가 유연하게 배치.
> **원칙**: 풍부하게 준비하되, 진행 속도에 따라 Practice 단위로 유연 조절. "감자 재배법" 원칙.
> **기반**: CC101 Sec01, 05, 06, 08, 10, 12 / CMG Ch03-05 / chaei 1.1-1.3, 2.1-2.5

---

## 전체 Practice 맵

| # | Practice | 커맨드 | 핵심 산출물 | 선행 조건 |
|---|---------|--------|------------|----------|
| 01 | 설치와 연결 | `/start-practice-01` | 설치 성공 + 첫 응답 | 없음 |
| 02 | 플러그인 + 나를 알려주는 파일 | `/start-practice-02` | `student-profile.md` + 첫 push | P01 |
| 03 | 도구 탐색 | `/start-practice-03` | `my-installed-tools.md` | P02 |
| 04 | 부서별 데이터 분석 | `/start-practice-04` | 부서별 분석 결과 파일 | P03 |
| 05 | 결과 다듬기 + 저장 | `/start-practice-05` | 확장 결과 파일 + push | P04 |
| 06 | CLAUDE.md 규칙 설계 | `/start-practice-06` | Always/Ask/Never CLAUDE.md | P01~05 |
| 07 | 구조가 결과를 바꾼다 | `/start-practice-07` | A/B/C 비교 + /prompt 결과 | P06 |
| 08 | 부서별 통합 파이프라인 | `/start-practice-08` | 통합 분석 보고서 | P07 |
| 09 | 배포와 공유 | `/start-practice-09` | HTML 대시보드 + Vercel URL | P08 |

---

## 교시 배분 참고 (강사 재량)

아래는 2주 8교시 배분 예시입니다. 진행 속도에 따라 유연하게 조절합니다.

### 첫째 주 (4교시)

| 교시 | 시간 | 권장 Practice | 비고 |
|------|------|--------------|------|
| 1교시 | 08:00~08:45 | Practice 01 | 설치에 시간 여유를 충분히 |
| 2교시 | 09:00~09:45 | Practice 02 | 인터뷰+Git까지 완료 |
| 3교시 | 10:00~10:45 | Practice 03 + 04 | 도구 탐색 후 바로 부서 적용 |
| 4교시 | 11:00~11:45 | Practice 05 | 확장 + 마무리 |

### 둘째 주 (4교시)

| 교시 | 시간 | 권장 Practice | 비고 |
|------|------|--------------|------|
| 1교시 | 08:00~08:45 | Practice 06 | 복습 + CLAUDE.md 설계 |
| 2교시 | 09:00~09:45 | Practice 07 | 3층 비교 실험 + /prompt |
| 3교시 | 10:00~10:45 | Practice 08 | Plan 모드 + 멀티파일 |
| 4교시 | 11:00~11:45 | Practice 09 | HTML + Vercel 배포 |

---

## 공통 강사 원칙

### 감자재배법
AI가 직접 다 해주는 것이 아니라, 수강생이 직접 질문하고, 직접 결과를 확인하고, 직접 수정하고, 직접 저장하는 방식으로 배웁니다.

### 저장해줘 → 올려줘
매 실습 끝에 반드시 commit + push 루프를 확인합니다.

### VSCode Extension 환경 인식
- 수강생은 CLI가 아닌 VSCode extension 환경입니다.
- 터미널 명령보다 GUI 기반 안내를 우선합니다.
- 도구 실패 시 유연하게 대신 수행하는 폴백 경로를 두세요.

### 자기 정체성
AI가 "나는 Claude입니다" 같은 자기 부정/혼란을 보이면, SCRIPT_INSTRUCTIONS의 자기 인식 지시문으로 돌아가세요.

---

## 부서별 데이터 파일 맵

| 그룹 | 폴더 | 주요 파일 |
|------|------|----------|
| A-RnD | `practice-data/A-RnD/` | `result.csv`, `battery_log.csv` |
| B-전략 | `practice-data/B-전략/` | `market_reports/Q1-2026.md`, `Q2-2026.md`, `kpi_data.csv` |
| C-제조 | `practice-data/C-제조/` | `defect_log.csv`, `production.csv`, `mold_history.csv` |
| D-경영 | `practice-data/D-경영/` | `budget_2026.csv`, `actual_Q1.csv`, `purchase_history.csv` |

---

## 트러블슈팅 공통

| 문제 | 해결 |
|------|------|
| 확장 안 보임 | VSCode 1.98+ 업데이트 후 재시작 |
| 로그인 브라우저 안 열림 | 팝업 차단 해제, claude.ai 직접 로그인 |
| 응답 없음 | Ctrl+N (새 대화), 또는 재로그인 |
| "구독 필요" 메시지 | Team 초대 미수락 → 이메일 확인 |
| `/plugin` 명령 안 됨 | 확장 최신 버전 확인 + Reload Window |
| push 실패 | `gh auth login` → 브라우저 인증 재시도 |
| 설치 완전 실패 | Plan B: Desktop App 또는 claude.ai/code |

---

## 새 Practice 추가 시 템플릿

새 실습을 추가할 때는 아래 구조를 따릅니다:

```
lesson-modules/practice-XX-{설명}/
  CLAUDE.md     ← 실습 메인 문서
```

CLAUDE.md 필수 섹션:
- `## 역할` — 강사 역할 정의
- `## 실습 목표` — 이번 실습에서 달성할 것
- `## 산출물` — 수강생이 만들 파일/결과물
- `## 성공 기준` — 완료 판정 기준
- `## 선행 조건` — 이 실습 전에 완료해야 할 Practice
- `## 진행 순서` — Step 1, Step 2... (각 Step에 ACTION/USER/STOP)
- `## 트러블슈팅` — 예상 문제와 해결
- `## 체크리스트` — 완료 확인 항목

커맨드 파일: `.claude/commands/start-practice-XX.md`
```
---
description: Practice XX — {설명}
allowedTools: Read, Write, Bash, Glob, Grep, AskUserQuestion
---
Read("course-structure.json")
Read("student-profile.md")
Read("lesson-modules/practice-XX-{설명}/CLAUDE.md")
Read(".claude/SCRIPT_INSTRUCTIONS.md")
```
