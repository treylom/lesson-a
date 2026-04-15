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
수강생 부서에 맞는 주제로 /deep-research를 체험합니다.

프롬프트 예시 (부서별):
- R&D: "배터리 안전성 최신 동향을 '빠르게' 조사해서 vault에 저장해줘"
- 전략: "자동차 부품 산업 2026 전망을 '빠르게' 조사해서 vault에 저장해줘"
- 제조: "제조업 AI 품질관리 사례를 '빠르게' 조사해서 vault에 저장해줘"
- 경영: "제조업 ESG 트렌드를 '빠르게' 조사해서 vault에 저장해줘"

**"빠르게" 키워드 필수** — 토큰 절약.
결과가 vault에 저장되면 옵시디언에서 확인합니다.

### /knowledge-manager-lite 통합 실습 (필수 — deep-research 후)
지금까지 vault에 쌓인 자료(PDF 변환본 + deep-research 결과 + 기존 실습 자료)를 통합 정리합니다.

프롬프트:
```
/knowledge-manager-lite 빠르게 vault 전체를 정리하고 INDEX.md를 업데이트해줘
```

⏳ 1-3분 걸립니다. "AI가 모든 파일을 읽고 연결하는 중이에요. 잠시 기다려주세요."

완료 후 옵시디언 그래프 뷰를 열어서 연결 관계를 확인합니다.
