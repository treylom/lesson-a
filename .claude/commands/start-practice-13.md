---
description: Practice 13 — 1-5주차 위키 자동 정리 + ChatGPT/Gemini 비교 (MW6 3교시)
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
Read("lesson-modules/practice-13-knowledge-manager/CLAUDE.md")
Read(".claude/SCRIPT_INSTRUCTIONS.md")

위 파일을 순서대로 읽고, student-profile.md가 있으면 수강생 이름/부서/업무를 파악한 뒤, Practice 13을 즉시 시작하세요.
git pull 충돌이 생기면 "강사에게 손을 들어 알려주세요"라고 안내합니다.

## 추가 지시 (Practice 13 전용)

### Obsidian MCP 우선 사용
파일 생성, 검색, vault 조작 시 **반드시 Obsidian MCP 도구(mcp__obsidian__*)를 우선 사용**하세요.
Write/Read 도구는 MCP가 실패했을 때만 폴백으로 사용합니다.

### 외부 리서치 실습 (필수 — 건너뛰지 말 것)
Practice 13 실습 중 외부 자료 수집 단계에서, 아래 3개 링크를 /knowledge-manager-lite로 처리하는 실습을 **반드시** 진행하세요:

1. **Anthropic 최신 연구**: https://www.anthropic.com/research
   → "이 페이지에서 가장 최근 글 하나를 '빠르게' 요약해서 External-Research/Anthropic/ 폴더에 저장해줘"

2. **OpenAI 최신 블로그**: https://openai.com/blog
   → "이 페이지에서 가장 최근 글 하나를 '빠르게' 요약해서 External-Research/OpenAI/ 폴더에 저장해줘"

3. **Google DeepMind 최신 연구**: https://deepmind.google/discover/blog/
   → "이 페이지에서 가장 최근 글 하나를 '빠르게' 요약해서 External-Research/DeepMind/ 폴더에 저장해줘"

수강생에게 위 프롬프트를 하나씩 복사해서 입력하게 안내합니다.
**"빠르게" 키워드를 빼먹지 않도록 강조하세요** — 토큰 절약에 중요합니다.

각 결과가 vault에 저장되면 옵시디언 사이드바에서 External-Research/ 폴더가 생겼는지 확인하게 합니다.
