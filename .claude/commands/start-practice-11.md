---
description: Practice 11 — 옵시디언 소개 + 첫 vault (MW6 1교시)
allowedTools: Read, Write, Bash, Glob, Grep, AskUserQuestion
---
$ARGUMENTS

## MW6 시작 준비 (자동 실행)

아래를 순서대로 실행하세요:

### 1단계: 기존 작업물 가져오기
Bash("git pull")
→ MW5까지 push한 student-profile.md, 분석 결과 등을 복원합니다.
→ 충돌이 생기면 "강사에게 손을 들어 알려주세요"라고 안내합니다.

### 2단계: lesson-a MW6 최신화
lesson-a/ 폴더 안의 lesson-modules/, .claude/commands/, .claude/skills/ 내용이
MW6(practice-11~14)을 포함하는지 확인합니다.
start-practice-11.md, start-practice-12.md 등이 .claude/commands/에 있으면 이미 최신입니다.
없으면 사용자에게 "lesson-a 최신화가 필요합니다. 강사에게 확인해주세요."라고 안내합니다.

### 3단계: 수강생 정보 로드
Read("course-structure.json")
Read("student-profile.md")
→ student-profile.md가 있으면 수강생 이름, 부서, 업무를 파악합니다.
→ 없으면 이름과 부서를 물어봅니다.

### 4단계: Practice 11 시작
Read("lesson-modules/practice-11-obsidian-intro/CLAUDE.md")
Read(".claude/SCRIPT_INSTRUCTIONS.md")

위 파일을 읽고, 수강생 이름과 부서를 사용하여 Practice 11을 즉시 시작하세요.
"OO님, 안녕하세요! MW6 첫 번째 시간입니다." 형식으로 인사합니다.
