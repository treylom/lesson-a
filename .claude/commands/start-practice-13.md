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

1. **Anthropic 최신 연구**: https://www.anthropic.com/research/how-ai-is-transforming-work-at-anthropic
   → "이 글을 요약해서 External-Research/Anthropic/ 폴더에 저장해줘"

2. **OpenAI 개발자 블로그**: https://developers.openai.com/blog/openai-for-developers-2025
   → "이 글을 요약해서 External-Research/OpenAI/ 폴더에 저장해줘"

3. **Google DeepMind 최신 연구**: https://deepmind.google/blog/accelerating-mathematical-and-scientific-discovery-with-gemini-deep-think/
   → "이 글을 요약해서 External-Research/DeepMind/ 폴더에 저장해줘"

수강생에게 위 프롬프트를 하나씩 복사해서 입력하게 안내합니다.
각 결과가 vault에 저장되면 옵시디언 사이드바에서 External-Research/ 폴더가 생겼는지 확인하게 합니다.

### 추가 아카이빙 실습 — 제조업 분야 (수강생이 골라서 2-3개 선택)

아래 리스트에서 **본인 부서와 관련된 글 2-3개를 골라서** 같은 방식으로 아카이빙합니다.
수강생에게 리스트를 보여주고 선택하게 하세요.

**🏭 제조업 자료 (15개)**

| # | 제목 | 링크 | 한 줄 설명 |
|---|------|------|-----------|
| 1 | Deloitte 2025 스마트 제조 조사 | https://www.deloitte.com/us/en/insights/industry/manufacturing/2025-smart-manufacturing-survey.html | 스마트 팩토리 도입 현황, 생산성 10-20% 개선 효과 |
| 2 | Siemens 산업 AI + 디지털 제조 | https://blogs.sw.siemens.com/nx-manufacturing/sps-2025-siemens-showcases-the-future-of-industrial-ai-and-digital-manufacturing/ | AI 디지털 트윈, 가상 컨트롤러(vPLC), Audi 협력 사례 |
| 3 | BMW 디지털 트랜스포메이션 | https://www.cio.com/article/3975188/how-bmw-is-digitizing-automotive-production.html | BMW 가상 팩토리 운영, 비용 30% 절감 |
| 4 | McKinsey Battery 2035 | https://www.mckinsey.com/features/mckinsey-center-for-future-mobility/our-insights/battery-2035-building-new-advantages | EV 배터리 2035 전략, 글로벌 기가팩토리 동향 |
| 5 | Bosch 배터리 제조 자동화 | https://www.boschrexroth.com/en/us/factory-automation/battery-manufacturing-automation/ | 배터리 생산 자동화 솔루션, 수율 개선 기술 |
| 6 | MIT Tech Review: 제조업 AI 혁신 | https://www.technologyreview.com/2025/11/19/1128067/scaling-innovation-in-manufacturing-with-ai/ | 50% 제조업체 AI 도입, 인재 양성 과제 |
| 7 | AI 비전 품질검사 + 합성데이터 | https://www.automate.org/industry-insights/quality-inspection-ai-vision-synthetic-data-testing-training | AI 비전 품질검사, 결함 검출 95-99% |
| 8 | AI 머신 비전의 품질 관리 역할 | https://www.qualitymag.com/articles/98187-machine-vision-and-the-role-of-ai-in-quality-control | 검사 속도 및 정확도 개선 사례 |
| 9 | Deloitte 2025 제조업 전망 | https://www.deloitte.com/us/en/insights/industry/manufacturing-industrial-products/manufacturing-industry-outlook/2025.html | 인력, AI 투자, 공급망, 녹색 기술 5대 트렌드 |
| 10 | 2025 공급망 트렌드 | https://www.supplychaindive.com/news/supply-chain-trends-risks-2025-retail-manufacturing/736817/ | 리쇼어링, 지역화, 디지털 혁신 동향 |
| 11 | IFR 2026 글로벌 로봇 트렌드 | https://ifr.org/ifr-press-releases/news/top-5-global-robotics-trends-2026 | 산업용 로봇 542,076대, 협업 로봇 성장, AI 통합 |
| 12 | 테슬라 상하이 95% 자동화 | https://electrek.co/2024/07/17/tesla-claims-automated-production-gigafactory-shanghai/ | 40초 사이클 타임, 용접 100% 자동화 |
| 13 | Audi AI 이미지 처리 품질 개선 | https://www.automotivemanufacturingsolutions.com/smart-factory/audi-wants-to-define-new-standards-for-ai-image-processing/46716.article | Audi AI 이미지 처리, 공정 품질 개선 |
| 14 | K-배터리 3중 충격 (한경) | https://magazine.hankyung.com/business/article/202505282219b | LG에너지솔루션·삼성SDI·SK온 점유율 하락, CATL·BYD 추월 |
| 15 | 디지털 트윈 엣지 AI 논문 (Nature) | https://www.nature.com/articles/s41598-025-28466-9 | 엣지 AI+페더레이션 러닝 기반 실시간 디지털 트윈 |

**선택 후 프롬프트**: "이 글을 요약해서 External-Research/제조업/ 폴더에 저장해줘: [선택한 URL]"

### 추가 아카이빙 실습 — AI 분야 (수강생이 골라서 2-3개 선택)

| # | 제목 | 링크 | 한 줄 설명 |
|---|------|------|-----------|
| 1 | Claude 모델 공식 비교 | https://platform.claude.com/docs/en/about-claude/models/overview | Opus, Sonnet, Haiku 성능·가격·문맥 창 비교 |
| 2 | Gemini 2.0 Flash 발표 | https://blog.google/innovation-and-ai/models-and-research/google-deepmind/google-gemini-ai-update-december-2024/ | 실시간 오디오/비디오, 멀티모달 AI 에이전트 |
| 3 | Meta Llama 공식 페이지 | https://www.llama.com/ | Llama 3.3/4 오픈소스 모델, 다운로드 방법 |
| 4 | GitHub Copilot 공식 | https://github.com/features/copilot | AI 페어 프로그래머, 2,000만+ 사용자 |
| 5 | AI 코딩 에이전트 비교 2025 | https://martinterhaak.medium.com/best-ai-coding-agents-summer-2025-c4d20cd0c846 | Cursor, Claude, Copilot 등 실제 개발자 비교 |
| 6 | AI 코딩 에이전트 벤치마크 | https://render.com/blog/ai-coding-agents-benchmark | Cursor vs Claude vs OpenAI vs Gemini 실제 테스트 |
| 7 | RAG 2025 연말 리뷰 | https://ragflow.io/blog/rag-review-2025-from-rag-to-context | RAG→Context 진화, GraphRAG, 에이전틱 오케스트레이션 |
| 8 | RAG 기업 실무 가이드 | https://www.glean.com/blog/rag-retrieval-augmented-generation | RAG 정의, 작동 원리, 기업 응용 종합 설명 |
| 9 | 프롬프트 엔지니어링 가이드 | https://www.promptingguide.ai/ | 기초~고급 프롬프트 기법, Chain-of-Thought, AI Agents |
| 10 | OpenAI 프롬프트 모범사례 | https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api | 효과적 프롬프트 작성 원칙, Few-shot 기법 |
| 11 | McKinsey AI 현황 2025 | https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai | 기업 AI 채택률 88%, AI 에이전트 실험 62% |
| 12 | 기업 생성AI 현황 2025 | https://menlovc.com/perspective/2025-the-state-of-generative-ai-in-the-enterprise/ | 기업 AI 투자 $11.5B→$37B (3.2배), 부서별 지출 동향 |
| 13 | AI Safety Index 2025 | https://futureoflife.org/ai-safety-index-summer-2025/ | Anthropic·OpenAI·Google 안전 성숙도 6항목 평가 |
| 14 | EU AI Act 공식 | https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai | 위험 기반 분류, 2026년 전체 적용, 벌금 최대 EUR 35M |
| 15 | NVIDIA 한국 AI 인프라 구축 | https://investor.nvidia.com/news/press-release-details/2025/NVIDIA-South-Korea-Government-and-Industrial-Giants-Build-AI-Infrastructure-and-Ecosystem-to-Fuel-Korea-Innovation-Industries-and-Jobs/default.aspx | 한국 정부+NVIDIA 협력, 50,000+ GPU, 네이버·카카오·업스테이지 |

**선택 후 프롬프트**: "이 글을 요약해서 External-Research/AI/ 폴더에 저장해줘: [선택한 URL]"

### 연결 확인 실습 (아카이빙 완료 후)
모든 아카이빙이 끝나면, vault 통합 정리 + 연결 확인:

```
/knowledge-manager-lite vault 전체를 정리하고 INDEX.md를 업데이트해줘
```

⏳ 1-3분 걸립니다. "AI가 모든 파일의 연결 관계를 분석 중이에요."

완료 후 옵시디언 그래프를 열어서 확인:
- "방금 아카이빙한 자료들이 서로 연결됐죠? 제조업 글과 AI 글이 '자동화', '품질' 같은 키워드로 이어져 있어요."
- "이게 여러 자료를 vault에 넣었을 때의 힘이에요. ChatGPT에서는 각각 따로 물어봐야 하지만, 여기선 자동으로 연결됩니다."

```
vault에서 "자동화"와 관련된 노트를 모두 찾아서 요약해줘
```

```
vault에서 내가 만든 student-profile.md와 연결된 노트가 뭐가 있는지 보여줘
```
