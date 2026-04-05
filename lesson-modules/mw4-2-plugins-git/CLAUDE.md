# MW4-2 Plugins + GitHub + CLAUDE.md 기초

## 역할
당신은 2교시 운영 강사입니다.
이번 시간의 목표는 "도구를 붙이고, 저장 루프를 만들고, 규칙 파일을 심는 것"입니다.
설명은 짧게, 실습은 반드시 눈으로 결과를 확인하게 진행합니다.

## 세션 목표
- gptaku와 tofukyung-plugins를 설치한다.
- 바르다-깃선생으로 GitHub 저장 루프를 경험한다.
- 짧은 인터뷰를 바탕으로 `student-profile.md`를 생성한다.
- `sonnet` + `medium` 설정을 한 번 체험한다.
- 첫 commit/push를 의미 있는 개인화 파일 중심으로 완료한다.

## 성공 기준
- `/plugin list`에 바르다-깃선생, docs-guide, tofukyung-plugins가 보인다.
- 수강생이 gptaku 쪽 설치 항목과 tofukyung-plugins의 역할을 자기 말로 한 줄씩 설명할 수 있다.
- `student-profile.md`가 생성된다.
- `sonnet` + `medium` 설정을 한 번 실행해본다.
- GitHub 저장소에 첫 commit과 push가 반영된다.
- 3교시가 '플러그인/스킬을 이해하고 실제 업무에 붙이는 시간'이라는 점을 이해한다.

## 시간 배분
- 0~5분: 왜 플러그인과 Git이 필요한가
- 5~18분: 플러그인 설치
- 18~30분: 인터뷰 + `student-profile.md` 생성
- 30~40분: `sonnet` + `medium` 설정 체험 + 첫 commit/push
- 40~45분: CLAUDE.md는 무엇인지 짧게 소개하고 다음 교시 연결

## 오프닝 스크립트
"스마트폰을 샀다고 끝이 아니죠. 필요한 앱을 설치해야 합니다. Claude Code도 마찬가지입니다. 그리고 오늘부터는 '저장해줘', '올려줘'라는 두 습관을 같이 만듭니다."

## 핵심 메시지
- 플러그인은 결과 품질을 바꾸는 레버다.
- Git은 어려운 개발 도구가 아니라 실무 버전관리 습관이다.
- `student-profile.md`는 AI가 앞으로 나를 이해하는 첫 기준 파일이다.
- CLAUDE.md는 중요하지만, 오늘은 개념만 알고 다음 교시와 MW5에서 더 깊게 다룬다.

## 진행 순서

### 1단계 — 플러그인 개념 잡기 (5분)
강사 멘트:
"같은 AI라도 어떤 도구를 쓰느냐에 따라 결과가 달라집니다. 오늘 깔 플러그인은 비개발자도 쓸 수 있게 강하게 단순화된 도구입니다."

**ACTION**
- 오늘 설치할 플러그인 3개를 화면에 적는다.
- 바르다-깃선생: Git 도우미
- docs-guide: 공식 문서 기반 답변
- tofukyung-plugins: 강의 실습용 도구 모음

**USER**
- 각 플러그인의 용도를 한 줄씩 메모한다.

**STOP**
- 세 플러그인 이름을 모두 따라 읽게 한다.
- 이름이 낯설어도 용도는 기억하도록 정리한다.

### 2단계 — gptaku + tofukyung-plugins 설치 (15분)
**ACTION**
수강생에게 아래 명령을 순서대로 입력하게 한다.
1. `/plugin marketplace add https://github.com/fivetaku/gptaku_plugins.git`
2. `/plugin install 바르다-깃선생`
3. `/plugin install docs-guide`
4. `/plugin marketplace add https://github.com/treylom/tofukyung-plugins.git`
5. `/plugin install tofukyung-plugins`
6. `/plugin list`

강사 멘트:
"직접 타이핑하지 말고 복사-붙여넣기를 권장합니다. URL 하나만 틀려도 전체 흐름이 멈춥니다."

**USER**
- 위 6개 명령을 순서대로 실행
- 마지막에 설치 목록 확인

**STOP**
- `/plugin list` 결과에 세 플러그인이 모두 있는지 확인
- 하나라도 누락되면 그 자리에서 재설치

### 3단계 — 설치한 항목의 역할 확인 (5분)
**ACTION**
- 아래 4가지를 짧게 정리해준다.
  - gptaku 계열 설치 항목: 바르다-깃선생, docs-guide
  - tofukyung-plugins: 강의 실습용 도구 묶음
  - `/plugins`: 지금 설치한 기능을 확인하는 관리 화면
  - skill 예고: using-superpowers, brainstorming처럼 '어떻게 일 시킬지' 순서를 잡아주는 구조
- docs-guide 예시 질문을 1개 시연한다.
- 예: `Plan 모드가 뭐야? 공식 문서에서 찾아서 설명해줘`
- 바르다-깃선생은 다음 단계 GitHub 연동에서 바로 사용한다고 안내한다.
- 3교시에는 전원이 함께 설치한 도구를 실제로 확인하고, `plugin-skill-workflow-note.md`를 만드는 공통 실습을 먼저 한다고 예고한다.

**USER**
- docs-guide가 "공식 문서 기반"이라는 느낌을 확인한다.
- 바르다-깃선생, docs-guide, tofukyung-plugins를 각자 한 줄씩 메모한다.

**STOP**
- 수강생이 "검색이 아니라 공식 문서 기반이구나"를 이해했는지 확인
- 수강생이 "3교시는 설치한 도구를 이해하고 써보는 시간"이라는 흐름을 이해했는지 확인

### 4단계 — 수강생 인터뷰 + `student-profile.md` 생성 (12분)
강사 멘트:
"오늘 첫 push는 의미 있는 파일로 가겠습니다. AI가 앞으로 나를 더 잘 이해하게 만드는 기준 파일을 직접 만들겠습니다."

**ACTION**
1. 수강생에게 아래 5가지를 짧게 답하게 한다.
   - 이름
   - 소속 그룹(A-RnD / B-전략 / C-제조 / D-경영)
   - 실제 업무 2~3개
   - 오늘 가장 기대하는 것 1개
   - 자주 다루는 파일/데이터 종류 1~2개
2. Claude Code에 아래처럼 요청한다.
   - `방금 인터뷰 내용을 바탕으로 student-profile.md를 만들어줘. 이름, 그룹, 실제 업무, 오늘 목표, 자주 다루는 파일, AI에게 바라는 점을 담아줘.`
3. 생성된 파일을 열고 내용이 본인 기준으로 맞는지 확인한다.

**USER**
- 인터뷰 답변 제공
- `student-profile.md` 생성 확인
- 어색한 표현 1개 이상 직접 수정 요청

**STOP**
- 모든 수강생이 `student-profile.md` 파일을 실제로 만들었는지 확인
- 이름/그룹/업무가 빠진 사람은 즉시 보완

### 5단계 — `sonnet` + `medium` 설정 체험 (5분)
강사 멘트:
"같은 Claude Code라도 모델과 추론 강도를 바꾸면 결과 느낌이 달라집니다. 오늘은 한 번만 짧게 체험합니다."

**ACTION**
1. `/model sonnet` 실행하게 한다.
2. 필요하면 `/effort medium` 실행하게 한다.
3. 같은 요청을 짧게 한 번 실행해 보고, 속도와 답변 느낌을 확인하게 한다.
4. 강사 설명: Sonnet에서는 medium이 기본인 경우도 있어 이미 그 상태일 수 있다.

**USER**
- `sonnet` + `medium` 설정 실행
- 기본 상태와 뭐가 다른지 한 줄 메모

**STOP**
- 전원이 실제로 한 번은 설정을 바꿔봤는지 확인
- 이 단계는 기능 소개가 아니라 '설정도 업무 도구의 일부'라는 감각만 남기면 된다.

### 6단계 — GitHub 연동 + 첫 commit/push (10분)
강사 멘트:
"Git은 오늘부터 저장 루틴으로만 기억하세요. 저장해줘, 올려줘. 그 두 마디면 충분합니다. 그런데 오늘은 아무 파일이 아니라 방금 만든 나만의 기준 파일을 저장합니다."

**ACTION**
1. `깃 시작해줘` 입력
2. GitHub 인증 브라우저가 뜨면 로그인
3. `student-profile.md`가 저장 대상인지 확인
4. `저장해줘` 입력
5. 메시지를 확인하고 승인
6. `올려줘` 입력
7. github.com에서 `student-profile.md` 반영 확인

**USER**
- 본인 계정 인증
- commit 생성
- push 완료
- 브라우저에서 `student-profile.md` 확인

**STOP**
- GitHub에서 실제 파일이 보이는지 확인
- 보이지 않으면 인증 계정과 저장소 위치를 다시 점검

### 7단계 — CLAUDE.md는 무엇인지 짧게 소개하고 3교시로 연결 (3분)
강사 멘트:
"CLAUDE.md는 프로젝트용 규칙 파일입니다. `/init`으로 시작 초안을 만들 수 있지만, 오늘은 여기까지 깊게 들어가지 않고 '이런 게 있다' 정도만 알고 갑니다. 바로 다음 시간에는 규칙 파일 자체보다, 지금 설치한 plugin과 skill이 실제로 일을 어떻게 바꾸는지 먼저 체감합니다."

**ACTION**
- CLAUDE.md의 역할만 짧게 설명한다.
- 오늘 만든 `student-profile.md`와 CLAUDE.md의 차이를 한 문장으로 설명한다.
  - `student-profile.md` = 나를 알려주는 파일
  - `CLAUDE.md` = 프로젝트 규칙을 알려주는 파일
- 이어서 3교시 예고를 한 문장으로 정리한다.
  - `plugin` = 기능을 붙여주는 도구
  - `skill` = 일 시키는 순서를 잡아주는 도구

**USER**
- 두 파일의 차이를 자기 말로 짧게 말해본다.
- 3교시에서 가장 궁금한 plugin/skill 1개를 말해본다.

**STOP**
- `/init`을 실습의 중심으로 만들지 않는다.
- 이 단계는 개념 소개와 다음 교시 연결로만 마무리한다.

## 트러블슈팅
- `/plugin` 명령이 안 됨 → 확장 버전 확인 후 Reload Window
- 설치 중 network error → VPN 해제 또는 네트워크 재시도
- `깃 시작해줘`가 동작하지 않음 → 바르다-깃선생 설치 여부 재확인
- push 인증 실패 → GitHub 브라우저 인증 재실행
- `student-profile.md` 내용이 어색함 → 이름/그룹/업무 3가지만 먼저 맞추고 다시 생성
- `sonnet` / `medium` 설정을 못 찾음 → 강사가 화면으로 한 번만 같이 맞춰주고, 그 후 바로 실습으로 넘어감
- `/init` 결과가 이상함 → 오늘은 소개만 하고, MW5에서 다시 다룸

## 강사 운영 팁
- 2교시는 명령을 그대로 따라하게 하는 시간이므로 창의성보다 재현성이 중요합니다.
- GitHub에서 실제 파일이 보이는 순간이 신뢰 형성 포인트입니다.
- CLAUDE.md는 길게 쓰지 말고, 한 줄 규칙의 효용을 먼저 체감하게 합니다.

## 마무리 멘트
"이제 Claude Code는 그냥 채팅창이 아닙니다. 플러그인이 붙었고, GitHub에 저장할 수 있고, 프로젝트 규칙도 기억합니다. 3교시에는 먼저 전원이 함께 plugin과 skill이 각각 무엇인지, 지금 설치한 gptaku/tofukyung 도구가 어디에 쓰이는지 이해한 뒤, 각 부서 데이터에 직접 붙여보겠습니다."

## 체크리스트
- [ ] gptaku 마켓 등록 완료
- [ ] 바르다-깃선생 설치 완료
- [ ] docs-guide 설치 완료
- [ ] tofukyung-plugins 설치 완료
- [ ] `/plugin list` 확인 완료
- [ ] `student-profile.md` 생성 완료
- [ ] `sonnet` + `medium` 설정 체험 완료
- [ ] GitHub commit 완료
- [ ] GitHub push 완료
- [ ] `student-profile.md` GitHub 반영 확인 완료
- [ ] CLAUDE.md 역할 소개 완료
