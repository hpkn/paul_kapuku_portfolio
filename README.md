# Paul Kapuku — Software Portfolio / 소프트웨어 포트폴리오

<div align="center">

**Backend & Platform Engineering · LLM Systems · AWS**

[🇬🇧 English](#-english) · [🇰🇷 한국어](#-한국어)

</div>

---

<a name="english"></a>

## 🇬🇧 English

# Paul N. Kapuku

**Senior LLM & AI Engineer** at RS-TEAM · Daejeon, South Korea
Backend architecture · Distributed systems · AWS · LLM & RAG infrastructure

I build backend platforms that carry AI workloads in production — not demos. Six years of
engineering across Korea and the DRC, currently leading the team behind an AI-powered
procurement intelligence platform, and co-founder/CTO of a software company in Kinshasa.

Working languages: **Korean · English · French**. In Korea since 2015.

📫 hassangpaul@gmail.com · [LinkedIn](https://www.linkedin.com/in/hassangpaul/)

---

## Contents

- [What I do](#what-i-do)
- [Selected work](#selected-work)
- [Open-source & demos](#open-source--demos)
- [Tech stack](#tech-stack)
- [How I work with AI tooling](#how-i-work-with-ai-tooling)
- [Contact](#contact)

---

## What I do

I sit between backend architecture and applied AI. Most of my work looks like this: take a
messy real-world domain, build the ingestion and data layer that makes it queryable, put an
LLM where it genuinely adds signal, and keep the whole thing running on infrastructure that
someone else can operate.

**Engineering leadership** — I lead development on BidSight at RS-TEAM: setting technical
direction, reviewing code, and reporting architecture to the executive team. I'm also
co-founder and CTO of Intel'city Kinshasa, where I've hired and led a small engineering team
since founding.

**Backend & platform** — Python/FastAPI and TypeScript/NestJS services, PostgreSQL, event
pipelines on Kafka and Celery/RabbitMQ, deployed on AWS with Docker and GitHub Actions.

**LLM infrastructure** — RAG pipelines over Korean-language corpora, pgvector semantic search,
self-hosted inference with Ollama and vLLM alongside AWS Bedrock, embedding pipelines, and the
GPU operations that keep them alive.

---

## Selected work

### BidRaon ([https://bidraon.ai](https://bidraon.ai/)) — AI procurement intelligence platform
*RS-TEAM · Lead engineer · proprietary*

A platform that turns Korean government procurement data into decisions: which tenders to bid
on, against whom, and at what price.

- **Ingestion & integrations** — pipelines against the KONEPS / 나라장터 public procurement
  ecosystem, plus Aligo and Dream Security PASS for notifications and identity
- **Semantic search** — pgvector over procurement documents and rubrics, with a section
  grounding validator to keep generated answers tied to source text
- **Bid intelligence** — recommendation logic, competitor analysis, and KDE-based
  distribution charts with named classification cases for bidding patterns
- **Document automation** — an automated policy-document (약관) download and extraction
  pipeline, plus Korean-language PDF report generation with ReportLab/WeasyPrint
- **Stack** — NestJS, FastAPI, PostgreSQL + pgvector, Ollama, AWS

### Skin and Hair analysis platforms (https://www.choicetech.kr) — distributed image inference

A multi-region microservices platform for image-based skin analysis, built around an
asynchronous inference pipeline.

- Decoupled services for image ingestion, ML inference and result delivery (NestJS), so each
  scales and fails independently
- Python Celery workers handling preprocessing and model inference, queued through RabbitMQ
  with Redis for coordination and retry semantics
- Idempotent message handling with deduplication, so retries under load don't double-process
- Deployed across EU and US AWS regions with Route 53 DNS failover and Nginx load balancing
- PostgreSQL for transactional storage, Prometheus/Grafana for metrics and alerting
- CI/CD via GitHub Actions with end-to-end test coverage

### Wapi Car — fleet telematics for the DRC
*Intel'city Kinshasa · Co-founder & CTO · proprietary*

GPS geolocation and logistics platform serving fleet operators in Kinshasa: animated route
history over an interactive map, minute-by-minute movement timelines, and stop/parking
reports. Built and operated by a team I hired and lead.

---

## Open-source & demos

| Project | What it is | Stack |
|---|---|---|
| [korean_multi_rag_chabot](https://github.com/hpkn/korean_multi_rag_chabot) | Korean-optimised RAG chatbot over multiple sources — Notion, Jira, Obsidian, local documents — with HWP/HWPX extraction for Korean office formats and local inference via Ollama | Python · RAG · Ollama · Korean NLP |
| [career-document-matching-demo](https://github.com/hpkn/career-document-matching-demo) · [live](https://ai-test.rs-team.com) | Semantic matching between career documents and job descriptions, with a rules engine and semantic normaliser layered over retrieval. Deployed as a systemd service | Python · Streamlit · RAG · NLP |
| [BE-SKIN-Analysis-sample-v2](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2) | Reference implementation of the async inference platform above — service structure, migrations, Swagger docs, e2e tests | TypeScript · NestJS · PostgreSQL |
| [local-image-generation-ollama](https://github.com/hpkn/local-image-generation-ollama) | Fully local image generation through Ollama — no cloud APIs, for privacy-constrained and offline environments | Python · Ollama |

Additional work at RS-TEAM and Intel'city is proprietary and not published.

---

## Tech stack

| | |
|---|---|
| **Languages** | Python · TypeScript · JavaScript · SQL |
| **Backend** | FastAPI · NestJS · Express · Flask · Django |
| **Data** | PostgreSQL · pgvector · Redis · Kafka · Spark · Celery · RabbitMQ |
| **Cloud & ops** | AWS · Docker · Nginx · GitHub Actions · Prometheus · Grafana |
| **AI / LLM** | RAG pipelines · embeddings · Ollama · vLLM · AWS Bedrock · LangChain · HuggingFace · Transformers · fine-tuning |

---

## How I work with AI tooling

I run LLM tooling as part of the engineering process, not beside it — agentic coding tools in
daily development, LLM-assisted review and documentation, and shared inference environments so
a team gets consistent results rather than each engineer improvising.

That extends to operating the infrastructure. I run self-hosted inference on GPU hardware
(RTX 4090 serving a chat model alongside bge-m3 embeddings) and on cloud GPU instances, which
means debugging things like NaN embedding output traced to a misconfigured FlashAttention
environment variable, or driver-level GPU faults under sustained load. Useful experience, in
that it's the part most teams discover only after they've committed to self-hosting.

---

## Contact

- 📧 **hassangpaul@gmail.com**
- 💼 [linkedin.com/in/hassangpaul](https://www.linkedin.com/in/hassangpaul/)
- 🌏 Daejeon, South Korea · open to roles in Seoul and remote

---
---

<a name="한국어"></a>

## 🇰🇷 한국어

# Paul N. Kapuku (폴 카푸쿠)

**Senior LLM & AI Engineer**, RS-TEAM · 대전
백엔드 아키텍처 · 분산 시스템 · AWS · LLM/RAG 인프라

데모가 아닌 **프로덕션 환경에서 AI 워크로드를 감당하는 백엔드 플랫폼**을 만듭니다.
한국과 콩고민주공화국에서 6년간 엔지니어링을 해왔고, 현재 AI 기반 조달 인텔리전스
플랫폼 개발을 리드하고 있으며, 킨샤사 소재 소프트웨어 회사의 공동창업자 겸 CTO입니다.

업무 언어: **한국어 · 영어 · 프랑스어** · 2015년부터 한국 거주

📫 hassangpaul@gmail.com · [LinkedIn](https://www.linkedin.com/in/hassangpaul/)

---

## 목차

- [주요 업무 영역](#주요-업무-영역)
- [주요 프로젝트](#주요-프로젝트)
- [오픈소스 및 데모](#오픈소스-및-데모)
- [기술 스택](#기술-스택-1)
- [AI 도구 활용 방식](#ai-도구-활용-방식)
- [연락처](#연락처)

---

## 주요 업무 영역

백엔드 아키텍처와 응용 AI의 접점에서 일합니다. 복잡한 실제 도메인을 다루고, 질의 가능한
형태로 만드는 수집·데이터 계층을 구축하고, LLM이 실질적인 가치를 더하는 지점에 배치한 뒤,
다른 사람이 운영할 수 있는 인프라 위에서 안정적으로 돌아가게 만드는 일입니다.

**엔지니어링 리더십** — RS-TEAM에서 BidSight 개발을 리드하며 기술 방향 설정, 코드 리뷰,
경영진 대상 아키텍처 보고를 담당합니다. Intel'city Kinshasa의 공동창업자 겸 CTO로서
창업 이래 소규모 엔지니어링 팀을 채용하고 이끌어 왔습니다.

**백엔드 및 플랫폼** — Python/FastAPI, TypeScript/NestJS 서비스, PostgreSQL,
Kafka 및 Celery/RabbitMQ 기반 이벤트 파이프라인, Docker와 GitHub Actions를 활용한 AWS 배포.

**LLM 인프라** — 한국어 코퍼스 기반 RAG 파이프라인, pgvector 시맨틱 검색,
Ollama·vLLM 자체 호스팅 추론 및 AWS Bedrock 연동, 임베딩 파이프라인, GPU 운영.

---

## 주요 프로젝트

### BidSight — AI 조달 인텔리전스 플랫폼
*RS-TEAM · 리드 엔지니어 · 비공개*

한국 공공조달 데이터를 의사결정으로 전환하는 플랫폼입니다. 어떤 입찰에, 누구와 경쟁하며,
어떤 가격으로 참여할지를 판단할 수 있게 합니다.

- **수집 및 연동** — KONEPS/나라장터 공공조달 생태계 연동 파이프라인, 알림 및 본인인증을
  위한 Aligo·드림시큐리티 PASS 연동
- **시맨틱 검색** — 조달 문서 및 평가 루브릭에 대한 pgvector 검색, 생성 답변을 원문에
  근거시키는 섹션 그라운딩 검증기
- **입찰 인텔리전스** — 추천 로직, 경쟁사 분석, 입찰 패턴 분류 케이스를 적용한
  KDE 기반 분포 차트
- **문서 자동화** — 보험 약관 자동 다운로드·추출 파이프라인,
  ReportLab/WeasyPrint 기반 한국어 PDF 리포트 생성
- **기술 스택** — NestJS, FastAPI, PostgreSQL + pgvector, Ollama, AWS

### 피부 분석 플랫폼 — 분산 이미지 추론
*컨슈머 저장소: [BE-SKIN-Analysis-sample-v2](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2)*

비동기 추론 파이프라인을 중심으로 설계한 멀티 리전 마이크로서비스 플랫폼입니다.

- 이미지 수집, ML 추론, 결과 전달을 분리한 서비스 구조(NestJS)로 개별 확장 및 장애 격리
- 전처리와 모델 추론을 담당하는 Python Celery 워커, RabbitMQ 큐잉 및 Redis 기반
  조율·재시도 처리
- 중복 제거를 포함한 멱등적 메시지 처리로 부하 상황의 재시도에도 중복 처리 방지
- EU·US AWS 리전 배포, Route 53 DNS 페일오버 및 Nginx 로드 밸런싱
- 트랜잭션 저장을 위한 PostgreSQL, Prometheus/Grafana 기반 메트릭 및 알림
- GitHub Actions CI/CD 및 E2E 테스트

### Wapi Car — 콩고민주공화국 차량 관제 플랫폼
*Intel'city Kinshasa · 공동창업자 겸 CTO · 비공개*

킨샤사 지역 차량 운영사를 위한 GPS 위치 기반 물류 플랫폼입니다. 인터랙티브 지도 상의
경로 이력 애니메이션, 분 단위 이동 타임라인, 정차·주차 리포트를 제공합니다.
직접 채용하고 이끄는 팀이 개발·운영하고 있습니다.

---

## 오픈소스 및 데모

| 프로젝트 | 설명 | 기술 스택 |
|---|---|---|
| [korean_multi_rag_chabot](https://github.com/hpkn/korean_multi_rag_chabot) | Notion·Jira·Obsidian·로컬 문서 등 다중 소스를 대상으로 하는 한국어 최적화 RAG 챗봇. HWP/HWPX 추출 지원 및 Ollama 로컬 추론 | Python · RAG · Ollama · 한국어 NLP |
| [career-document-matching-demo](https://github.com/hpkn/career-document-matching-demo) · [데모](https://ai-test.rs-team.com) | 경력 문서와 채용 공고 간 시맨틱 매칭. 검색 위에 룰 엔진과 의미 정규화 계층을 결합. systemd 서비스로 배포 | Python · Streamlit · RAG · NLP |
| [BE-SKIN-Analysis-sample-v2](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2) | 위 비동기 추론 플랫폼의 레퍼런스 구현 — 서비스 구조, 마이그레이션, Swagger 문서, E2E 테스트 | TypeScript · NestJS · PostgreSQL |
| [local-image-generation-ollama](https://github.com/hpkn/local-image-generation-ollama) | Ollama 기반 완전 로컬 이미지 생성. 클라우드 API 없이 프라이버시 제약·오프라인 환경 대응 | Python · Ollama |

RS-TEAM 및 Intel'city의 그 외 업무는 비공개입니다.

---

## 기술 스택

| | |
|---|---|
| **언어** | Python · TypeScript · JavaScript · SQL |
| **백엔드** | FastAPI · NestJS · Express · Flask · Django |
| **데이터** | PostgreSQL · pgvector · Redis · Kafka · Spark · Celery · RabbitMQ |
| **클라우드·운영** | AWS (EC2, S3, Route 53) · Docker · Nginx · GitHub Actions · Prometheus · Grafana |
| **AI / LLM** | RAG 파이프라인 · 임베딩(bge-m3) · Ollama · vLLM · AWS Bedrock · LangChain · HuggingFace · Transformers · 파인튜닝 |

---

## AI 도구 활용 방식

LLM 도구를 엔지니어링 프로세스의 일부로 운영합니다. 일상 개발에서의 에이전틱 코딩 도구
활용, LLM 기반 리뷰 및 문서화, 그리고 개인별 편차 없이 일관된 결과를 얻기 위한 팀 공용
추론 환경 구성까지 포함합니다.

인프라 운영도 직접 합니다. GPU 하드웨어(RTX 4090에서 챗 모델과 bge-m3 임베딩 동시 서빙)와
클라우드 GPU 인스턴스에서 자체 호스팅 추론을 운영하며, FlashAttention 환경 변수 오설정으로
인한 NaN 임베딩 문제나 지속 부하 상황의 드라이버 레벨 GPU 오류 같은 이슈를 직접
디버깅해 왔습니다. 자체 호스팅을 결정한 뒤에야 마주치게 되는 영역입니다.

---

## 연락처

- 📧 **hassangpaul@gmail.com**
- 💼 [linkedin.com/in/hassangpaul](https://www.linkedin.com/in/hassangpaul/)
- 🌏 대전 · 서울 및 원격 근무 가능

---

<div align="center">
<sub>Backend · Distributed systems · LLM infrastructure — 한국어 · English · Français</sub>
</div>
