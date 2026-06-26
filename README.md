# n8n 공식 문서 링크 모음집

n8n(엔에이트엔) 자동화 플랫폼의 [공식 문서](https://docs.n8n.io/) 카테고리별 빠른 접근 인덱스.

> 📅 **마지막 업데이트**: 2026-06-26
> 🔗 **원본**: https://docs.n8n.io
> 📜 **라이선스**: 본 문서는 n8n 공식 문서 링크 모음일 뿐, 원 콘텐츠는 n8n 소유

---

## 🚀 시작하기 (Get Started)

- [환영 페이지](https://docs.n8n.io/) — n8n 메인 문서 홈
- [사용 방식 선택 (클라우드 vs 자체호스팅)](https://docs.n8n.io/choose-n8n/)
- [첫 워크플로우 구축](https://docs.n8n.io/try-it-out/)
- [학습 경로](https://docs.n8n.io/learning-path/)
- [주요 용어 사전 (Glossary)](https://docs.n8n.io/glossary/)
- [코스 (Courses)](https://docs.n8n.io/courses/)
- [비디오 튜토리얼](https://docs.n8n.io/video-courses/)

---

## ☁️ n8n 클라우드 (Cloud)

- [무료 체험 시작](https://docs.n8n.io/manage-cloud/start-cloud-trial/)
- [관리자 대시보드 사용](https://docs.n8n.io/manage-cloud/use-admin-dashboard/)
- [클라우드 IP 주소](https://docs.n8n.io/manage-cloud/cloud-data-management/)
- [동시성 이해](https://docs.n8n.io/manage-cloud/concurrency/)

---

## 🏠 자체호스팅 (Self-Hosting)

### 설치 옵션
- [설치 방법 개요](https://docs.n8n.io/hosting/installation/)
- [npm으로 설치](https://docs.n8n.io/hosting/installation/npm/)
- [Docker로 설치](https://docs.n8n.io/hosting/installation/docker/)
- [Docker Compose 사용](https://docs.n8n.io/hosting/installation/server-setups/docker-compose/)

### 클라우드 제공자 배포
- [Digital Ocean](https://docs.n8n.io/hosting/installation/server-setups/digital-ocean/)
- [Heroku](https://docs.n8n.io/hosting/installation/server-setups/heroku/)
- [Hetzner](https://docs.n8n.io/hosting/installation/server-setups/hetzner/)
- [AWS](https://docs.n8n.io/hosting/installation/server-setups/aws/)
- [Azure](https://docs.n8n.io/hosting/installation/server-setups/azure/)
- [Google Cloud Run](https://docs.n8n.io/hosting/installation/server-setups/google-cloud-run/)
- [Google Kubernetes Engine](https://docs.n8n.io/hosting/installation/server-setups/google-kubernetes/)

### 구성 (Configuration)
- [환경변수 설정 개요](https://docs.n8n.io/hosting/configuration/environment-variables/)
- [데이터베이스 설정](https://docs.n8n.io/hosting/configuration/environment-variables/database/)
- [자격증명 (Credentials)](https://docs.n8n.io/hosting/configuration/environment-variables/credentials/)
- [큐 모드 (Queue Mode)](https://docs.n8n.io/hosting/configuration/environment-variables/queue-mode/)
- [보안](https://docs.n8n.io/hosting/configuration/environment-variables/security/)
- [작업 러너 (Task Runners)](https://docs.n8n.io/hosting/configuration/environment-variables/task-runners/)
- [SSO](https://docs.n8n.io/hosting/configuration/environment-variables/sso/)
- [사용자 관리](https://docs.n8n.io/hosting/configuration/environment-variables/user-management/)
- [OpenTelemetry](https://docs.n8n.io/hosting/configuration/environment-variables/opentelemetry/)

### 보안
- [보안 정책 관리](https://docs.n8n.io/hosting/securing/security-audit/)
- [SSL 설정](https://docs.n8n.io/hosting/configuration/configuration-examples/ssl/)
- [SSO 구성 (SAML)](https://docs.n8n.io/hosting/configuration/sso-saml/)
- [SSO 구성 (OIDC)](https://docs.n8n.io/hosting/configuration/sso-oidc/)
- [SSRF 보호](https://docs.n8n.io/hosting/configuration/environment-variables/security/#ssrf-protection)
- [공개 API 비활성화](https://docs.n8n.io/hosting/securing/disable-public-api/)

### 확장성 & 운영
- [성능 측정 (Benchmark)](https://docs.n8n.io/hosting/scaling/performance-benchmarking/)
- [큐 모드 활성화](https://docs.n8n.io/hosting/scaling/queue-mode/)
- [실행 데이터 관리](https://docs.n8n.io/hosting/scaling/execution-data/)
- [Grafana로 메트릭 시각화](https://docs.n8n.io/hosting/logging-monitoring/monitoring/)
- [n8n 업데이트](https://docs.n8n.io/hosting/installation/updating/)

### 아키텍처
- [n8n 작동 원리](https://docs.n8n.io/hosting/architecture/overview/)
- [데이터베이스 구조](https://docs.n8n.io/hosting/architecture/database/)
- [커뮤니티 에디션 기능](https://docs.n8n.io/hosting/community-edition-features/)

---

## 🛠️ 워크플로우 구축 (Build)

### 워크플로우 이해
- [워크플로우 개요](https://docs.n8n.io/workflows/)
- [워크플로우 구성 요소](https://docs.n8n.io/workflows/components/)
- [노드 (Nodes)](https://docs.n8n.io/workflows/components/nodes/)
- [연결 (Connections)](https://docs.n8n.io/workflows/components/connections/)
- [캔버스 그룹](https://docs.n8n.io/workflows/components/canvas-groups/)
- [주석 및 문서화](https://docs.n8n.io/workflows/sticky-notes/)
- [워크플로우 ID 찾기](https://docs.n8n.io/workflows/workflow-id/)

### 실행 (Executions)
- [실행 유형 (수동/부분/자동)](https://docs.n8n.io/workflows/executions/)
- [더티 노드 이해](https://docs.n8n.io/workflows/executions/dirty-nodes/)
- [실행 디버깅](https://docs.n8n.io/workflows/executions/debug/)
- [모든 실행 보기](https://docs.n8n.io/workflows/executions/execution-history/)
- [실시간 응답 스트리밍](https://docs.n8n.io/workflows/executions/streaming/)

### 워크플로우 생성 및 관리
- [워크플로우 생성/실행/발행](https://docs.n8n.io/workflows/create/)
- [자격증명 생성/편집](https://docs.n8n.io/credentials/)
- [워크플로우 설정 구성](https://docs.n8n.io/workflows/settings/)
- [태그 지정](https://docs.n8n.io/workflows/tags/)
- [변경 이력 보기](https://docs.n8n.io/workflows/history/)
- [내보내기/가져오기](https://docs.n8n.io/workflows/export-import/)
- [공유 (Sharing)](https://docs.n8n.io/workflows/sharing/)

### 흐름 논리 (Flow Logic)
- [조건부 분기 (If, Switch)](https://docs.n8n.io/flow-logic/splitting/)
- [데이터 병합 (Merge)](https://docs.n8n.io/flow-logic/merging/)
- [루프 (Loops)](https://docs.n8n.io/flow-logic/looping/)
- [대기 (Wait)](https://docs.n8n.io/flow-logic/waiting/)
- [서브워크플로우](https://docs.n8n.io/flow-logic/subworkflows/)
- [오류 처리 (Error Handling)](https://docs.n8n.io/flow-logic/error-handling/)
- [실행 순서 이해](https://docs.n8n.io/flow-logic/execution-order/)

### 데이터 작업
- [n8n 데이터 구조](https://docs.n8n.io/data/)
- [데이터 변환](https://docs.n8n.io/data/transforming-data/)
- [표현식 참조 (Expressions)](https://docs.n8n.io/code/expressions/)
- [파일 및 이미지 작업](https://docs.n8n.io/data/binary-data/)
- [날짜 및 시간 작업](https://docs.n8n.io/data/data-mapping/data-mapping-ui/)
- [JSON 데이터 쿼리](https://docs.n8n.io/code/cookbook/jmespath/)

### 코드 작성
- [코드 노드 사용](https://docs.n8n.io/code/code-node/)
- [내장 메서드 및 변수 (Builtin)](https://docs.n8n.io/code/builtin/overview/)
- [JMESPath](https://docs.n8n.io/code/cookbook/jmespath/)
- [LangChain 코드](https://docs.n8n.io/code/cookbook/langchain/)
- [HTTP 노드](https://docs.n8n.io/code/cookbook/http-node/)
- [코드 요리책 (Cookbook)](https://docs.n8n.io/code/cookbook/)

---

## 🤖 AI / LangChain

### 핵심 개념
- [AI 통합 개요](https://docs.n8n.io/advanced-ai/)
- [체인 (Chains)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/)
- [에이전트 (Agents)](https://docs.n8n.io/advanced-ai/intro-tutorial/)
- [메모리 (Memory)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/#memory)
- [도구 (Tools)](https://docs.n8n.io/advanced-ai/langchain/langchain-overview/#tools)
- [벡터 스토어 / RAG](https://docs.n8n.io/advanced-ai/rag-in-n8n/)
- [에이전트 vs 체인](https://docs.n8n.io/advanced-ai/examples/agent-chain-comparison/)

### AI 테스트·평가
- [평가 (Evaluations) 시작](https://docs.n8n.io/advanced-ai/evaluations/)
- [메트릭 기반 품질 측정](https://docs.n8n.io/advanced-ai/evaluations/metrics/)

### AI 예시
- [Google Sheets를 데이터 소스로](https://docs.n8n.io/advanced-ai/examples/data-google-sheets/)
- [API 호출 (도구로)](https://docs.n8n.io/advanced-ai/examples/api-workflow-tool/)
- [웹사이트 콘텐츠 활용](https://docs.n8n.io/advanced-ai/examples/web-content/)
- [Human-in-the-Loop](https://docs.n8n.io/advanced-ai/examples/human-in-the-loop/)
- [AI 워크플로우 휴먼 폴백](https://docs.n8n.io/advanced-ai/examples/human-fallback/)

---

## 🔌 노드 (Nodes)

- [핵심 노드 (Core Nodes) 전체](https://docs.n8n.io/integrations/builtin/core-nodes/)
- [트리거 노드 (Trigger Nodes)](https://docs.n8n.io/integrations/builtin/trigger-nodes/)
- [앱 노드 (App Nodes) — 500+ 통합](https://docs.n8n.io/integrations/builtin/app-nodes/)
- [클러스터 노드 (Cluster Nodes — AI/LangChain)](https://docs.n8n.io/integrations/builtin/cluster-nodes/)
- [Credential 노드 전체](https://docs.n8n.io/integrations/builtin/credentials/)

### 자주 쓰는 핵심 노드
- [HTTP Request](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/)
- [Webhook](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.webhook/)
- [Code](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/)
- [If](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.if/)
- [Switch](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.switch/)
- [Merge](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.merge/)
- [Loop Over Items](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.splitinbatches/)
- [Set / Edit Fields](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.set/)
- [Schedule Trigger](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/)
- [Execute Sub-workflow](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.executeworkflow/)
- [Wait](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.wait/)

### AI 클러스터 노드
- [AI Agent](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.agent/)
- [Chat Trigger](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-langchain.chattrigger/)
- [Basic LLM Chain](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainllm/)
- [Q&A Chain](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.chainretrievalqa/)
- [OpenAI](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.openai/)
- [Anthropic Chat Model](https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatanthropic/)
- [Google Gemini](https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatgooglegemini/)
- [Vector Store (모음)](https://docs.n8n.io/integrations/builtin/cluster-nodes/sub-nodes/)

### 인기 앱 노드
- [Gmail](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.gmail/)
- [Google Sheets](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/)
- [Google Drive](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/)
- [Slack](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.slack/)
- [Discord](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.discord/)
- [Notion](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.notion/)
- [Airtable](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.airtable/)
- [HubSpot](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/)
- [Telegram](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.telegram/)
- [GitHub](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.github/)

---

## 🔑 자격증명 (Credentials)

- [자격증명 개요](https://docs.n8n.io/credentials/)
- [자격증명 추가/편집](https://docs.n8n.io/credentials/add-edit-credentials/)
- [API key vs OAuth](https://docs.n8n.io/credentials/credential-types/)
- [공유 (Sharing)](https://docs.n8n.io/credentials/sharing-credentials/)

---

## 🌐 API

- [공개 API 개요](https://docs.n8n.io/api/)
- [API 인증](https://docs.n8n.io/api/authentication/)
- [페이지네이션](https://docs.n8n.io/api/pagination/)
- [API 참조 (Swagger)](https://docs.n8n.io/api/api-reference/)
- [Curl로 사용](https://docs.n8n.io/api/using-api-playground/)

---

## 🧩 임베드 (Embed)

- [임베드 개요](https://docs.n8n.io/embed/)
- [n8n 임베드 준비](https://docs.n8n.io/embed/prerequisites/)
- [구성](https://docs.n8n.io/embed/configuration/)
- [디플로이먼트](https://docs.n8n.io/embed/deployment/)
- [화이트라벨링](https://docs.n8n.io/embed/white-labelling/)

---

## 👥 협업 (Collaboration)

- [팀 작업](https://docs.n8n.io/user-management/)
- [팀 역할](https://docs.n8n.io/user-management/roles-and-permissions/)
- [SAML SSO](https://docs.n8n.io/user-management/saml/)
- [LDAP](https://docs.n8n.io/user-management/ldap/)

---

## 🔧 커스텀 노드 개발 (Node Building)

- [노드 빌딩 개요](https://docs.n8n.io/integrations/creating-nodes/overview/)
- [노드 만들기 가이드](https://docs.n8n.io/integrations/creating-nodes/build/)
- [선언적 노드 (Declarative)](https://docs.n8n.io/integrations/creating-nodes/build/declarative-style-node/)
- [프로그래밍 방식 노드](https://docs.n8n.io/integrations/creating-nodes/build/programmatic-style-node/)
- [트리거 노드 만들기](https://docs.n8n.io/integrations/creating-nodes/build/trigger-node/)
- [노드 테스트](https://docs.n8n.io/integrations/creating-nodes/test/)
- [노드 발행](https://docs.n8n.io/integrations/creating-nodes/deploy/submit-community-nodes/)
- [노드 UI 디자인 가이드](https://docs.n8n.io/integrations/creating-nodes/plan/node-ui-design/)

---

## 📚 추가 리소스

- [n8n 커뮤니티 포럼](https://community.n8n.io/)
- [n8n 블로그](https://blog.n8n.io/)
- [n8n YouTube](https://www.youtube.com/@n8n-io)
- [n8n 워크플로우 템플릿](https://n8n.io/workflows/)
- [n8n GitHub](https://github.com/n8n-io/n8n)
- [n8n 노드 발행 (npm)](https://www.npmjs.com/search?q=keywords:n8n-community-node-package)

---

## 🤝 기여 (Contributing)

이 모음집에 빠진 링크나 깨진 링크 발견하면 PR로 보내주세요.

---

> 🏛️ **만든 이유**: n8n 공식 문서는 방대해서 카테고리별 빠른 진입점이 필요. 자주 쓰는 페이지만 한 곳에 모아 북마크 대용으로 사용.
