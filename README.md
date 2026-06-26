# n8n 학습 가이드 — 공식 문서 기반 교육 자료

n8n(엔에이트엔) 자동화 플랫폼의 [공식 문서](https://docs.n8n.io/)를 학습 순서·실습 예제·체크리스트와 함께 정리한 **교육용 인덱스**.

> 📅 **마지막 업데이트**: 2026-06-26
> 🔗 **원본**: https://docs.n8n.io
> 🎯 **대상**: n8n 입문자 → 중급자, 강의·워크숍 교재
> 📜 **라이선스**: 본 문서는 n8n 공식 문서 링크 모음일 뿐, 원 콘텐츠는 n8n 소유

---

## 🎯 학습 목표 (Level별)

| 레벨 | 학습 내용 | 소요 시간 |
|------|----------|----------|
| 🟢 **초급** | 설치·첫 워크플로우·기본 노드 이해 | 1주 (5~10h) |
| 🟡 **중급** | 데이터 변환·흐름 논리·자격증명·서브워크플로우 | 2~3주 (15~25h) |
| 🟠 **AI 통합** | LangChain 에이전트·메모리·RAG·평가 | 1~2주 (10~15h) |
| 🔴 **고급** | 자체호스팅·확장·커스텀 노드·임베드 | 2~4주 (20~40h) |

---

## 📚 학습 로드맵

### Phase 1: 시작하기 (Week 1, 초급) 🟢

> **목표**: n8n이 뭔지 이해하고, 첫 자동화 워크플로우 만들기

**학습 순서**
1. [n8n 환영 페이지](https://docs.n8n.io/) — n8n이 뭔지 1분 이해
2. [사용 방식 선택](https://docs.n8n.io/choose-n8n/) — 클라우드 vs 자체호스팅
3. [첫 워크플로우 구축 (Try it out)](https://docs.n8n.io/try-it-out/) — 실제로 한 번 만들어보기
4. [학습 경로](https://docs.n8n.io/learning-path/) — 공식 로드맵
5. [주요 용어 사전 (Glossary)](https://docs.n8n.io/glossary/) — 헷갈리는 용어 정리
6. [코스 (Courses)](https://docs.n8n.io/courses/) — 공식 인터랙티브 코스
7. [비디오 튜토리얼](https://docs.n8n.io/video-courses/) — 영상으로 한 번 더

**🎓 실습 과제**
- 🔨 **HTTP Request 노드로 외부 API 호출 → Set 노드로 데이터 가공 → Email 노드로 전송**

**✅ 체크포인트**
- [ ] n8n을 클라우드 또는 로컬에 설치했다
- [ ] 워크플로우 1개를 만들어 실행했다
- [ ] 트리거 노드·액션 노드·정규 노드를 구분할 수 있다
- [ ] 실행 결과 화면에서 데이터 흐름을 읽을 수 있다

---

### Phase 2: 워크플로우 구축 기초 (Week 2, 중급) 🟡

> **목표**: 데이터 흐름·조건 분기·반복·자격증명 이해

**학습 순서**

#### 2-1. 워크플로우 이해
- [워크플로우 개요](https://docs.n8n.io/workflows/) — 워크플로우 구조 이해
- [노드 (Nodes)](https://docs.n8n.io/workflows/components/nodes/) — 노드가 뭔지·종류
- [연결 (Connections)](https://docs.n8n.io/workflows/components/connections/) — 노드 사이 데이터 흐름
- [캔버스 그룹](https://docs.n8n.io/workflows/components/canvas-groups/) — 노드 묶기
- [주석 (Sticky Notes)](https://docs.n8n.io/workflows/sticky-notes/) — 문서화

#### 2-2. 실행 이해
- [실행 유형 (수동/부분/자동)](https://docs.n8n.io/workflows/executions/) — 워크플로우 실행 방식
- [실행 디버깅](https://docs.n8n.io/workflows/executions/debug/) — 에러 추적
- [모든 실행 보기](https://docs.n8n.io/workflows/executions/execution-history/) — 실행 이력

#### 2-3. 흐름 논리 (Flow Logic)
- [조건부 분기 (If, Switch)](https://docs.n8n.io/flow-logic/splitting/) — 조건 따라 다른 길로
- [데이터 병합 (Merge)](https://docs.n8n.io/flow-logic/merging/) — 여러 길 합치기
- [루프 (Loops)](https://docs.n8n.io/flow-logic/looping/) — 반복
- [대기 (Wait)](https://docs.n8n.io/flow-logic/waiting/) — 지연·기다림
- [서브워크플로우](https://docs.n8n.io/flow-logic/subworkflows/) — 워크플로우 안에 워크플로우
- [오류 처리 (Error Handling)](https://docs.n8n.io/flow-logic/error-handling/) — 실패 대응
- [실행 순서 이해](https://docs.n8n.io/flow-logic/execution-order/) — 노드 실행 순서

#### 2-4. 자격증명
- [자격증명 개요](https://docs.n8n.io/credentials/) — API key·OAuth 관리
- [자격증명 추가/편집](https://docs.n8n.io/credentials/add-edit-credentials/)
- [API key vs OAuth](https://docs.n8n.io/credentials/credential-types/)

**🎓 실습 과제**
- 🔨 **Google Sheets에서 신규 행 감지 → If 노드로 조건 분기 → Slack 알림 / 이메일 발송 (2가지 길)**

**✅ 체크포인트**
- [ ] If·Switch·Merge를 사용한 워크플로우를 만들었다
- [ ] 자격증명을 등록하고 노드에 연결했다
- [ ] 에러 워크플로우(Error Trigger)를 설정했다
- [ ] 서브워크플로우를 만들고 호출했다

---

### Phase 3: 데이터 다루기 & 코드 (Week 3, 중급) 🟡

> **목표**: n8n 데이터 구조 이해 + 표현식·코드 노드로 자유롭게 데이터 변환

**학습 순서**

#### 3-1. 데이터 구조
- [n8n 데이터 구조](https://docs.n8n.io/data/) — items·json·binary 이해
- [데이터 변환](https://docs.n8n.io/data/transforming-data/) — 데이터 모양 바꾸기
- [표현식 참조 (Expressions)](https://docs.n8n.io/code/expressions/) — `{{ }}` 사용법
- [파일 및 이미지 작업](https://docs.n8n.io/data/binary-data/) — 바이너리 데이터
- [JSON 데이터 쿼리 (JMESPath)](https://docs.n8n.io/code/cookbook/jmespath/) — JSON 추출

#### 3-2. 코드 작성
- [코드 노드 사용](https://docs.n8n.io/code/code-node/) — JavaScript/Python 직접 실행
- [내장 메서드 및 변수 (Builtin)](https://docs.n8n.io/code/builtin/overview/)
- [HTTP 노드 활용](https://docs.n8n.io/code/cookbook/http-node/)
- [코드 요리책 (Cookbook)](https://docs.n8n.io/code/cookbook/) — 실전 예시 모음

**🎓 실습 과제**
- 🔨 **API에서 JSON 받기 → JMESPath로 특정 필드만 추출 → Code 노드로 가공 → Webhook으로 응답**

**✅ 체크포인트**
- [ ] 표현식으로 이전 노드 데이터를 참조할 수 있다
- [ ] Code 노드에 JavaScript를 작성하고 실행했다
- [ ] 바이너리 파일을 다운로드/업로드 노드로 처리했다

---

### Phase 4: AI 통합 (Week 4~5, AI 단계) 🟠

> **목표**: LangChain 에이전트·메모리·도구·RAG로 AI 워크플로우 구축

**학습 순서**

#### 4-1. AI 핵심 개념
- [AI 통합 개요](https://docs.n8n.io/advanced-ai/) — n8n의 AI 기능 한눈에
- [체인 (Chains)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/) — LLM을 연쇄 호출
- [에이전트 (Agents)](https://docs.n8n.io/advanced-ai/intro-tutorial/) — 자율 판단하는 AI
- [메모리 (Memory)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/#memory) — 대화 기억
- [도구 (Tools)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/#tools) — 에이전트가 호출하는 함수
- [벡터 스토어 / RAG](https://docs.n8n.io/advanced-ai/rag-in-n8n/) — 문서 검색 증강
- [에이전트 vs 체인](https://docs.n8n.io/advanced-ai/examples/agent-chain-comparison/)

#### 4-2. AI 테스트·평가
- [평가 (Evaluations) 시작](https://docs.n8n.io/advanced-ai/evaluations/)
- [메트릭 기반 품질 측정](https://docs.n8n.io/advanced-ai/evaluations/metrics/)

#### 4-3. AI 실전 예시
- [Google Sheets를 데이터 소스로](https://docs.n8n.io/advanced-ai/examples/data-google-sheets/)
- [API 호출 (도구로)](https://docs.n8n.io/advanced-ai/examples/api-workflow-tool/)
- [웹사이트 콘텐츠 활용](https://docs.n8n.io/advanced-ai/examples/web-content/)
- [Human-in-the-Loop](https://docs.n8n.io/advanced-ai/examples/human-in-the-loop/)

**🎓 실습 과제**
- 🔨 **Chat Trigger → AI Agent (OpenAI + Memory + Google Sheets Tool) → 사용자 질문에 시트 검색 후 답변**

**✅ 체크포인트**
- [ ] AI Agent 노드에 LLM·Memory·Tool 연결을 했다
- [ ] RAG 워크플로우(벡터 스토어)를 만들었다
- [ ] 평가(Evaluation) 노드로 AI 응답 품질을 측정했다

---

### Phase 5: 자체호스팅 & 운영 (Week 6, 고급) 🔴

> **목표**: n8n을 자체 서버에 띄우고 안정적으로 운영

**학습 순서**

#### 5-1. 설치
- [설치 방법 개요](https://docs.n8n.io/hosting/installation/)
- [npm으로 설치](https://docs.n8n.io/hosting/installation/npm/)
- [Docker로 설치](https://docs.n8n.io/hosting/installation/docker/)
- [Docker Compose](https://docs.n8n.io/hosting/installation/server-setups/docker-compose/)

#### 5-2. 클라우드 배포
- [Digital Ocean](https://docs.n8n.io/hosting/installation/server-setups/digital-ocean/)
- [AWS](https://docs.n8n.io/hosting/installation/server-setups/aws/)
- [Google Cloud Run](https://docs.n8n.io/hosting/installation/server-setups/google-cloud-run/)
- [Hetzner](https://docs.n8n.io/hosting/installation/server-setups/hetzner/)

#### 5-3. 구성 (Configuration)
- [환경변수 설정 개요](https://docs.n8n.io/hosting/configuration/environment-variables/)
- [데이터베이스 설정](https://docs.n8n.io/hosting/configuration/environment-variables/database/)
- [큐 모드 (Queue Mode)](https://docs.n8n.io/hosting/configuration/environment-variables/queue-mode/)
- [보안](https://docs.n8n.io/hosting/configuration/environment-variables/security/)
- [SSO (SAML/OIDC)](https://docs.n8n.io/hosting/configuration/sso-saml/)
- [SSL 설정](https://docs.n8n.io/hosting/configuration/configuration-examples/ssl/)

#### 5-4. 확장성 & 운영
- [성능 측정](https://docs.n8n.io/hosting/scaling/performance-benchmarking/)
- [큐 모드 활성화](https://docs.n8n.io/hosting/scaling/queue-mode/)
- [Grafana 메트릭](https://docs.n8n.io/hosting/logging-monitoring/monitoring/)
- [n8n 업데이트](https://docs.n8n.io/hosting/installation/updating/)

**🎓 실습 과제**
- 🔨 **Docker Compose로 n8n + PostgreSQL + Redis(큐 모드) 띄우고 SSL 인증서 적용**

**✅ 체크포인트**
- [ ] 자체 서버에 n8n을 설치했다
- [ ] 데이터베이스를 PostgreSQL로 바꿨다
- [ ] 큐 모드 활성화로 워커 분리를 했다
- [ ] HTTPS·SSO·보안 설정을 적용했다

---

### Phase 6 (선택): 커스텀 노드 개발 & 임베드 🔴

> **목표**: n8n에 없는 통합을 직접 만들고, n8n을 자기 서비스에 임베드

#### 6-1. 커스텀 노드 개발
- [노드 빌딩 개요](https://docs.n8n.io/integrations/creating-nodes/overview/)
- [노드 만들기 가이드](https://docs.n8n.io/integrations/creating-nodes/build/)
- [선언적 노드 (Declarative)](https://docs.n8n.io/integrations/creating-nodes/build/declarative-style-node/)
- [프로그래밍 방식 노드](https://docs.n8n.io/integrations/creating-nodes/build/programmatic-style-node/)
- [트리거 노드 만들기](https://docs.n8n.io/integrations/creating-nodes/build/trigger-node/)
- [노드 테스트](https://docs.n8n.io/integrations/creating-nodes/test/)
- [노드 발행 (커뮤니티 제출)](https://docs.n8n.io/integrations/creating-nodes/deploy/submit-community-nodes/)
- [노드 UI 디자인 가이드](https://docs.n8n.io/integrations/creating-nodes/plan/node-ui-design/)

#### 6-2. 임베드
- [임베드 개요](https://docs.n8n.io/embed/)
- [임베드 준비](https://docs.n8n.io/embed/prerequisites/)
- [구성](https://docs.n8n.io/embed/configuration/)
- [디플로이먼트](https://docs.n8n.io/embed/deployment/)
- [화이트라벨링](https://docs.n8n.io/embed/white-labelling/)

---

## 🔌 노드 레퍼런스 (실무에서 자주 쓰는 노드)

### 핵심 노드 Top 10 (외워두면 80% 워크플로우 해결)
| 노드 | 용도 | 링크 |
|------|------|------|
| HTTP Request | 외부 API 호출 (만능) | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) |
| Webhook | 외부에서 트리거 받기 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.webhook/) |
| Code | JavaScript/Python 직접 실행 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/) |
| If | 조건 분기 (참/거짓) | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.if/) |
| Switch | 다중 분기 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.switch/) |
| Merge | 여러 경로 합치기 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.merge/) |
| Loop Over Items | 반복 처리 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.splitinbatches/) |
| Edit Fields (Set) | 데이터 가공·매핑 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.set/) |
| Schedule Trigger | 주기 실행 (cron) | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/) |
| Execute Sub-workflow | 서브워크플로우 호출 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.executeworkflow/) |

### AI 클러스터 노드 Top 7
| 노드 | 용도 | 링크 |
|------|------|------|
| AI Agent | 자율 판단 에이전트 (메인) | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.agent/) |
| Chat Trigger | 채팅 인터페이스 | [docs](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-langchain.chattrigger/) |
| Basic LLM Chain | 단순 LLM 호출 | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainllm/) |
| Q&A Chain (RAG) | 문서 기반 Q&A | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainretrievalqa/) |
| OpenAI Chat Model | GPT 사용 | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.openai/) |
| Anthropic Chat Model | Claude 사용 | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatanthropic/) |
| Google Gemini | Gemini 사용 | [docs](https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatgooglegemini/) |

### 인기 앱 노드 Top 10
| 앱 | 링크 |
|----|------|
| Gmail | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.gmail/) |
| Google Sheets | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) |
| Google Drive | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) |
| Slack | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.slack/) |
| Discord | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.discord/) |
| Notion | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.notion/) |
| Airtable | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.airtable/) |
| HubSpot | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) |
| Telegram | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.telegram/) |
| GitHub | [docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.github/) |

---

## 🛠️ 실습 예제 모음 (강의용)

### 🟢 초급 — 워밍업
1. **이메일 알림 봇**: Schedule Trigger → HTTP Request (날씨 API) → If (비 옴?) → Gmail 발송
2. **RSS 모니터**: RSS Read Trigger → Filter → Slack 발송
3. **Google Form 응답 처리**: Webhook → Google Sheets 저장 → Email 확인

### 🟡 중급 — 실전 자동화
4. **고객 지원 티켓 분류**: Email Trigger → Code(키워드 추출) → Switch → 부서별 Slack 채널
5. **CRM 동기화**: HubSpot Trigger → Loop → Airtable Update
6. **콘텐츠 큐레이션**: 여러 RSS → Merge → 중복 제거 → Notion 페이지 생성

### 🟠 AI — 에이전트
7. **고객 챗봇**: Chat Trigger → AI Agent (OpenAI + Memory + Knowledge Base Tool) → 응답
8. **문서 Q&A RAG**: PDF 업로드 → 임베딩 생성 → Vector Store 저장 → Chat으로 질문/답변
9. **자율 리서치 에이전트**: 주제 입력 → AI Agent (Web Search Tool + Summarize) → Notion 저장

### 🔴 고급 — 프로덕션
10. **Slack 봇 풀스택**: Slack Trigger → AI Agent → DB 조회 → Slack 답장 (대화 메모리)
11. **자체호스팅 + 큐 모드**: Docker Compose로 n8n + Postgres + Redis 띄우기
12. **커스텀 노드**: 사내 API용 커스텀 노드 만들어 npm에 발행

---

## 📝 평가 체크리스트 (강사용)

### Level 1 검정
- [ ] HTTP Request 노드로 외부 API 호출
- [ ] If 노드로 조건 분기
- [ ] Schedule Trigger로 정기 실행
- [ ] 자격증명 1개 등록·사용

### Level 2 검정
- [ ] 표현식으로 이전 노드 데이터 참조
- [ ] Code 노드에 JS 작성
- [ ] 서브워크플로우 분리
- [ ] Error Trigger 구성

### Level 3 검정 (AI)
- [ ] AI Agent 노드에 Memory + Tool 연결
- [ ] RAG 워크플로우 구축
- [ ] Evaluation 노드로 응답 품질 측정

### Level 4 검정 (자체호스팅)
- [ ] Docker로 n8n 설치
- [ ] Postgres·SSL·SSO 적용
- [ ] 큐 모드 활성화

---

## 👨‍🏫 강사용 활용 팁

### 1. 시간 배분 (8시간 1일 워크숍 기준)
- 09:00~10:30 (90분): Phase 1 — n8n 소개 + 첫 워크플로우
- 10:45~12:00 (75분): Phase 2 — 흐름 논리·자격증명
- 13:00~14:30 (90분): Phase 3 — 데이터·코드 노드
- 14:45~16:15 (90분): Phase 4 — AI 에이전트 실습
- 16:30~17:30 (60분): Phase 5 맛보기 + Q&A

### 2. 핵심 실습 권장
- **반드시**: HTTP Request, If, Schedule, AI Agent (4개) — 이거 4개만 잘 가르치면 80% 강의 성공
- **선택**: Code 노드 (개발자 대상일 때만)
- **고급**: 자체호스팅 (별도 2일 워크숍 추천)

### 3. 자주 막히는 포인트
- 데이터 구조 (items vs json) → 시각화 자료로 반복 설명
- 표현식 `{{ }}` 문법 → 라이브 코딩으로 5번 이상 보여주기
- AI Agent의 Tool 연결 → 도구 호출 흐름을 그림으로
- 자격증명 OAuth 첫 등록 → 화면 녹화 캡처 미리 준비

### 4. 수강생 사전 준비물
- n8n 클라우드 무료 체험 가입 (이메일만)
- Google 계정 (Sheets/Gmail 노드 실습용)
- (선택) OpenAI API key 또는 Anthropic API key

---

## 📚 추가 리소스

- [n8n 커뮤니티 포럼](https://community.n8n.io/) — 막힐 때 검색
- [n8n 블로그](https://blog.n8n.io/) — 실전 사례·신기능 발표
- [n8n YouTube](https://www.youtube.com/@n8n-io) — 공식 영상 튜토리얼
- [n8n 워크플로우 템플릿](https://n8n.io/workflows/) — 만든 워크플로우 1000+개
- [n8n GitHub](https://github.com/n8n-io/n8n) — 소스 코드·이슈·로드맵
- [커뮤니티 노드 (npm 검색)](https://www.npmjs.com/search?q=keywords:n8n-community-node-package)

---

## 🤝 기여 (Contributing)

- 깨진 링크 발견 → Issue 또는 PR
- 새 실습 예제 추가 → PR
- 한국어 강의 자료 변형판 → fork 후 자유 사용

---

## 📜 라이선스

이 모음집(MIT) — n8n 공식 문서는 n8n GmbH 소유 (Fair-code 라이선스). 학습 목적 사용은 자유.

---

> 🏛️ **선정문목법(先定門目)** — 목차·구조 먼저 세운 뒤 실습. n8n 같은 도구는 기능이 많아서 학습 순서 없으면 길을 잃기 쉬워. 이 가이드는 그 길잡이.
