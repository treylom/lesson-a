---
description: Practice 14 — 서브에이전트 + 토큰 절약 + MW7 예고 (MW6 4교시)
allowedTools: Read, Write, Bash, Glob, Grep, AskUserQuestion, mcp__obsidian__*
---
$ARGUMENTS

Bash("git pull")

## Obsidian MCP 설치 확인 (필수)
.claude/settings.json을 읽고, mcpServers.obsidian 설정이 있는지 확인하세요.
없으면 아래 설정을 .claude/settings.json에 추가합니다:
```json
"mcpServers": {
  "obsidian": {
    "command": "npx",
    "args": ["-y", "obsidian-mcp@1.0.6"],
    "env": {
      "OBSIDIAN_VAULT_PATH": "."
    }
  }
}
```

Read("course-structure.json")
Read("student-profile.md")
Read("lesson-modules/practice-14-subagent-codex/CLAUDE.md")
Read(".claude/SCRIPT_INSTRUCTIONS.md")

위 파일을 순서대로 읽고, student-profile.md가 있으면 수강생 이름/부서/업무를 파악한 뒤, Practice 14를 즉시 시작하세요.
git pull 충돌이 생기면 "강사에게 손을 들어 알려주세요"라고 안내합니다.

## 추가 지시 (Practice 14 전용)

### Obsidian MCP 우선 사용
파일 생성, 검색, vault 조작 시 **반드시 Obsidian MCP 도구(mcp__obsidian__*)를 우선 사용**하세요.

### Codex 토론은 후순위
Practice 14 CLAUDE.md에 Codex 관련 내용이 있으면, 실습 후반부에 "시간 여유 시" 옵션으로 배치하세요.
**아래 실습을 먼저 진행합니다.**

### PDF 변환 실습 (필수 — 실습 초반)
수강생에게 본인 PC에 있는 PDF 파일 1개를 선택하게 합니다. 없으면 강사가 준비한 샘플 PDF를 사용합니다.

프롬프트:
```
이 PDF를 마크다운으로 변환해서 vault에 저장해줘: [PDF 파일 경로]
```

변환된 .md 파일이 옵시디언 사이드바에 나타나는지 확인합니다.
"이게 AI가 PDF를 읽을 수 있는 형태로 바꾼 거예요. 이제 검색도 되고, 다른 노트와 연결도 됩니다."

### /deep-research 실습 (필수 — PDF 변환 후)
수강생 부서에 맞는 **복합적이고 깊이 있는 주제**로 /deep-research를 체험합니다.
아래 부서별 프롬프트를 수강생에게 **그대로 복사해서 입력**하게 안내합니다.

**MW1-5 연관 주제로 deep-research를 진행합니다.**
기존 vault의 MW1-5 실습 노트와 자동 연결되는 것을 체험하는 게 목적입니다.

수강생에게 아래 프롬프트를 **그대로 복사해서 입력**하게 안내합니다:

**1차 deep-research (전원 공통):**
```
/deep-research
"AI 코드 어시스턴트(Claude Code, GitHub Copilot, Cursor 등)를 실무에 도입한 비개발자 사례"를 조사해줘.
제조업, 마케팅, 재무 등 비개발 직군에서 AI 코딩 도구를 어떻게 활용하는지,
실제 생산성 향상 수치와 도입 시 겪는 어려움을 정리해줘.
결과를 vault의 External-Research/deep-research/ 폴더에 저장해줘.
```

**2차 deep-research (전원 공통):**
```
/deep-research
"CLAUDE.md와 같은 AI 규칙 파일(System Prompt, Custom Instructions)이 결과 품질에 미치는 영향"을 조사해줘.
프롬프트 엔지니어링 vs 규칙 파일 기반 접근법의 차이,
실제 기업에서 AI 규칙 파일을 관리하는 사례를 정리해줘.
결과를 vault의 External-Research/deep-research/ 폴더에 저장해줘.
```

⏳ **deep-research는 각 2-5분 걸립니다.** "AI가 여러 소스를 검색하고 분석하는 중이에요. 잠시 기다려주세요."

완료 후 옵시디언 그래프를 열어서 **새 리서치 노트가 기존 MW1-5 실습 노트와 연결된 것**을 확인합니다.
"여러분이 1-5주차에 만든 노트와 자동으로 연결됐죠? 이게 vault의 힘이에요."

### 추가 실습: vault 검색 체험 (반복 — 체화용)
deep-research 결과가 저장된 후, 수강생에게 vault 검색을 체험하게 합니다:

```
vault에서 "프롬프트"와 관련된 노트를 모두 찾아줘
```

```
vault에서 내가 MW4에서 만든 분석 결과와 오늘 리서치한 내용의 공통점을 정리해줘
```

이 검색이 vault 안에서만 작동하며, 기존 노트끼리 연결되는 과정을 눈으로 확인하게 합니다.

### /knowledge-manager-lite 통합 실습 (필수 — deep-research 후)
지금까지 vault에 쌓인 자료(PDF 변환본 + deep-research 결과 + 기존 실습 자료)를 통합 정리합니다.

프롬프트:
```
/knowledge-manager-lite vault 전체를 정리하고 INDEX.md를 업데이트해줘
```

⏳ 1-3분 걸립니다. "AI가 모든 파일을 읽고 연결하는 중이에요. 잠시 기다려주세요."

완료 후 옵시디언 그래프 뷰를 열어서 연결 관계를 확인합니다.
