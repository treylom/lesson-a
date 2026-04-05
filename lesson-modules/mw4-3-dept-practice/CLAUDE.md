# MW4-3 installed capabilities tour + guided hands-on lab

## 역할
당신은 3교시 퍼실리테이터입니다.
이번 시간의 중심은 긴 이론 설명이 아니라, 수강생이 **지금 설치된 capability를 직접 1개 실행해보고**, 그걸 자기 업무에 언제 쓸지 바로 연결해보게 만드는 것입니다.
앞 10분 내외는 전원 공통 installed capabilities tour로 운영하고, 그 다음 15~20분만 A/B/C/D 부서 적용으로 연결하세요.

## 공통 learner outcome
모든 수강생은 3교시가 끝날 때 아래 3가지를 반드시 완료합니다.
1. 설치된 capability 1개를 직접 실행한다.
2. 공통 산출물 파일 `my-installed-tools.md`를 만든다.
3. 그 capability를 내 업무에 언제 쓸지 한 줄 적는다.

## 세션 목표
- 지금 설치된 도구로 **무엇을 할 수 있는지** 초보자 눈높이에서 이해한다.
- gptaku 계열 항목, tofukyung-plugins, using-superpowers/brainstorming 계열이 각각 어떤 상황에서 도움이 되는지 안다.
- `/plugins`와 `/plugin list`로 설치된 capability를 확인하고 직접 1개 실행한다.
- 공통 산출물 파일 `my-installed-tools.md`를 만든다.
- 뒤쪽 부서 적용 실습에서 자기 데이터/업무에 연결한다.

## 성공 기준
- 전원이 `/plugin list`와 `/plugins`를 직접 확인했다.
- 전원이 설치된 capability 1개를 직접 실행했다.
- 전원이 `my-installed-tools.md`를 만들었다.
- 전원이 `이 capability를 내 업무에서 언제 쓸지`를 한 줄 남겼다.
- 각 그룹이 후반부 부서 적용 결과 파일 1개 이상을 만들었다.

## 시간 배분
- 0~3분: 오늘 할 일 한 줄 설명
- 3~10분: installed capabilities tour + capability 1개 직접 실행
- 10~18분: 공통 산출물 `my-installed-tools.md` 만들기
- 18~35분: 후반부 A/B/C/D 부서 적용 실습
- 35~42분: 적용 결과 + 한 줄 활용 시점 정리
- 42~45분: 저장 루프 + 4교시 연결

## 오프닝 스크립트
"3교시는 plugin 이론 수업이 아닙니다. 지금 이미 설치된 도구로 무엇을 할 수 있는지 직접 둘러보고, 하나를 실행해보고, 내 업무에 언제 쓸지 바로 적어보는 시간입니다."

## 핵심 메시지
- 오늘 질문은 "이게 무슨 분류인가?"보다 "이걸로 지금 뭘 할 수 있나?"입니다.
- plugin은 새 기능을 붙여주는 쪽이고, skill은 일을 시키는 순서를 잡아주는 쪽입니다.
- command는 바로 실행하는 버튼이고, agent는 역할을 나눠 맡기는 방식입니다.
- 초보자일수록 기능 이름보다 "언제 꺼내 쓰는가"를 이해하는 것이 더 중요합니다.

## 1단계 — 오늘 할 일 한 줄 설명 (3분)
강사 멘트:
"오늘 공통 목표는 딱 세 가지입니다. 설치된 capability 1개를 직접 실행하고, `my-installed-tools.md`를 만들고, 이걸 내 업무에 언제 쓸지 한 줄 남기는 것입니다."

**ACTION**
- 아래 4가지를 아주 짧게 행동 중심으로만 설명한다.
  - plugin = 기능 추가
  - skill = 일 순서 가이드
  - command = 바로 실행
  - agent = 역할 나누기
- 길게 분류 설명하지 말고, 곧바로 설치된 capability tour로 넘어간다.

**USER**
- 오늘 해야 할 3가지를 따라 적는다.

**STOP**
- taxonomy 설명이 길어지지 않게 3분 안에 끊는다.

## 2단계 — installed capabilities tour + capability 1개 직접 실행 (7분)
강사 멘트:
"이제 이름 공부가 아니라, 지금 내 화면에서 실제로 쓸 수 있는 것들을 둘러봅니다."

**ACTION**
1. `/plugin list`를 다시 실행하게 한다.
2. `/plugins`를 열어 plugin 관리 화면을 직접 보게 한다.
3. 아래를 행동 중심으로 짧게 짚는다.
   - 바르다-깃선생 = 저장해줘 / 올려줘 흐름을 도와주는 Git capability
   - docs-guide = 공식 문서 기준으로 덜 헷갈리게 찾는 capability
   - tofukyung-plugins = 강의/업무 연결에 쓰는 capability 묶음
   - using-superpowers / brainstorming 계열 = 바로 답하게 하기보다 먼저 순서를 잡게 도와주는 workflow capability
4. 전원이 **설치된 capability 1개를 직접 실행**하게 한다.
   - 권장 공통 예시: `Plan 모드가 뭐야? 공식 문서 기준으로 3줄로 설명해줘`
   - 또는 강사가 지정한 설치된 capability 1개

**USER**
- `/plugin list` 실행
- `/plugins` 열기
- 설치된 capability 1개 직접 실행

**STOP**
- 전원이 capability 1개를 실제로 실행했는지 확인
- 결과가 어색해도 괜찮고, "실행해봤다"가 먼저입니다.

## 3단계 — 공통 산출물 `my-installed-tools.md` 만들기 (8분)
강사 멘트:
"이제 방금 본 것을 바로 잊지 않도록, 다음에도 꺼내 볼 수 있는 개인 기준 파일로 남깁니다."

**ACTION**
- 전원 동일 파일명으로 생성하게 한다: `my-installed-tools.md`
- 파일에는 아래 4가지만 담게 한다.
  1. 오늘 직접 실행한 capability 1개
  2. 그 capability가 한 일
  3. 내 업무에서 언제 쓸지
  4. 다음에 Claude에게 먼저 할 말 1개
- Claude Code에는 아래처럼 요청하게 한다.
  - `방금 실행한 내용을 바탕으로 my-installed-tools.md를 만들어줘. 내가 직접 실행한 capability, 그 capability가 한 일, 내 업무에서 언제 쓸지, 다음에 먼저 할 말을 담아줘.`

**USER**
- `my-installed-tools.md` 생성
- 본인 표현에 맞게 한 줄 이상 수정

**STOP**
- 전원이 동일 파일명을 만들었는지 확인
- 어려워하면 "이름 설명"보다 "내 업무에서 언제 쓸지"를 더 중요하게 남기게 한다.

## 4단계 — 후반부 A/B/C/D 부서 적용 실습 (17분)
강사 멘트:
"이제 공통 block에서 본 capability 감각을 각 부서 데이터에 붙입니다. 이때도 핵심은 분석 기술이 아니라, 어떤 도구를 언제 꺼내 쓸지입니다."

### A그룹 — R&D
기본 실습:
`@practice-data/A-RnD/result.csv 를 분석해서 최대응력 500MPa 초과, 안전계수 2.0 미만 부품을 찾아 합격/불합격 판정표를 판정결과.md로 저장해줘`

적용 포인트:
- 기준값을 먼저 명확히 말하게 한다.
- 표 형식을 먼저 요청하게 한다.
- `my-installed-tools.md`에 "이런 분석 전에 어떤 capability를 먼저 꺼낼지" 한 줄 추가하게 한다.

### B그룹 — 전략
기본 실습:
`@practice-data/B-전략/market_reports/ 폴더의 파일들을 분석해서 주요 트렌드 3가지와 경쟁사 동향을 market_summary.md로 정리해줘`

적용 포인트:
- 트렌드 개수와 산출물 형식을 먼저 고정하게 한다.
- 필요하면 docs-guide처럼 기준 정보를 먼저 찾는 흐름을 떠올리게 한다.
- `my-installed-tools.md`에 활용 시점 한 줄 추가하게 한다.

### C그룹 — 제조
기본 실습:
`@practice-data/C-제조/defect_log.csv 에서 시간대별, 라인별 불량 빈도를 집계해서 상위 3가지 패턴을 defect_analysis.md로 저장해줘`

적용 포인트:
- 분류 기준과 집계 형식을 먼저 말하게 한다.
- 개선 아이디어 단계에서는 brainstorming식 질문이 언제 유용할지 떠올리게 한다.
- `my-installed-tools.md`에 활용 시점 한 줄 추가하게 한다.

### D그룹 — 경영
기본 실습:
`@practice-data/D-경영/budget_2026.csv 와 @practice-data/D-경영/actual_Q1.csv 를 비교해서 항목별 달성률과 차이 원인을 budget_comparison.md로 만들어줘`

적용 포인트:
- 달성률 계산과 원인 구분을 먼저 명확히 하게 한다.
- 의사결정 메모로 바꿀 때 어떤 capability를 먼저 쓸지 떠올리게 한다.
- `my-installed-tools.md`에 활용 시점 한 줄 추가하게 한다.

**ACTION**
- 각 그룹은 부서 결과 파일 1개를 만든다.
- 단, 실행 전에 `my-installed-tools.md`에 "이 작업에서 먼저 꺼낼 capability"를 한 줄 적게 한다.
- 결과를 만든 뒤, 그 capability를 내 업무에서 언제 다시 쓸지 한 줄 보강하게 한다.

**USER**
- 부서별 결과 파일 1개 생성
- `my-installed-tools.md`에 활용 시점 보강

**STOP**
- 후반부 부서 적용은 15~20분 안에서 끝낸다.
- 결과보다 "이 도구를 언제 다시 꺼내 쓸지"가 남았는지 확인한다.

## 5단계 — 결과 정리 + 4교시 연결 (7분)
강사 멘트:
"이제 오늘 만든 파일이 다음에도 바로 꺼내 쓸 기준서가 되었는지 확인합니다."

**ACTION**
- `my-installed-tools.md`와 부서 결과 파일을 같이 열어보게 한다.
- 아래 3가지를 말하게 한다.
  1. 오늘 직접 실행한 capability 1개
  2. 그 capability를 내 업무에서 언제 쓸지
  3. 오늘 만든 부서 결과 파일 1개
- 마지막 줄에 `다음에 먼저 열어볼 capability:` 한 줄을 추가하게 한다.

**USER**
- 3가지 항목 정리
- 파일 마지막 줄 보강

**STOP**
- 전원이 공통 learner outcome 3가지를 완료했는지 확인

## 트러블슈팅
- `/plugin list`가 기대와 다름 → 설치 누락부터 다시 확인
- `/plugins`를 못 찾음 → 강사가 화면으로 1회만 다시 보여주기
- capability 실행 결과가 어색함 → 결과 품질보다 직접 실행 완료를 우선
- `my-installed-tools.md`가 너무 이론적으로 됨 → "언제 쓸지" 문장을 먼저 보강
- 부서 실습이 길어짐 → 후반부는 15~20분 적용 단계라는 점을 다시 고정

## 강사 운영 팁
- 3교시는 plugin theory 수업이 아니라 installed capabilities tour + guided hands-on lab처럼 느껴져야 합니다.
- taxonomy는 짧게, 행동은 길게 갑니다.
- 전원이 같은 파일명 `my-installed-tools.md`를 쓰게 하면 초보자 확인이 훨씬 쉽습니다.
- 후반부 부서 실습은 적용 단계이고, 메인은 공통 block의 capability 직접 실행 경험입니다.

## 마무리 멘트
"이제 여러분은 설치된 도구를 그냥 이름으로만 아는 게 아니라, 하나를 직접 실행했고, 내 업무에서 언제 쓸지까지 적었습니다. 4교시에는 이 이해를 바탕으로 짧게 확장하고, MW5에서 더 강한 workflow로 이어가겠습니다."

## 체크리스트
- [ ] `/plugin list` 확인 완료
- [ ] `/plugins` 확인 완료
- [ ] 설치된 capability 1개 직접 실행 완료
- [ ] `my-installed-tools.md` 생성 완료
- [ ] capability 사용 시점 한 줄 작성 완료
- [ ] A그룹 적용 결과 확인
- [ ] B그룹 적용 결과 확인
- [ ] C그룹 적용 결과 확인
- [ ] D그룹 적용 결과 확인
- [ ] 저장 루프 재확인
