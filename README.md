# Paul Kapuku Software Portfolio / 소프트웨어 포트폴리오

<div align="center">

[🇬🇧 English](#english) | [🇰🇷 한국어](#korean)

</div>

---

<a name="english"></a>
# 🇬🇧 English Version

# 👋 Hi, I'm Paul N. KAPUKU

> 💻 Backend Engineer | Python • Javascript • Typescript • Kafka • Spark • FastAPI • NodeJS/Nestjs • Nginx • Docker • SQL • NoSql • AWS • LLM • AI Engineering • ML and AI fundamentals

---

##

> 🔭 Currently building a marketing-recommendation engine with LLM-driven insights  
> 🌱 Always learning about data-driven architectures & distributed systems  
> 📫 Reach me at hassangpaul@gmail.com   |  [LinkedIn](https://linkedin.com/in/hassangpaul)

---

## 📋 Table of Contents

- [About Me](#about-me)  
- [Featured Projects](#featured-projects)  
  - [Marketing Recommender](#marketing-recommender)  
  - [Event-Driven Pipeline](#event-driven-pipeline)  
  - [Content Analysis Service](#content-analysis-service)  
  - [Skin Analysis Service](#skin-analysis-service)
  - [Customer CRM Backend API](#customer-crm-backend-api)
- [Tech Stack](#tech-stack)  
- [GitHub Stats](#github-stats)  
- [Contact](#contact)

---

## 📝 About Me

I'm a backend engineer with 5 years of experience building real-time data pipelines, microservices, and AI-powered APIs. I've led projects at midsize startups and enjoy mentoring juniors on best practices in observability, testing, and cloud architecture.

---

## 🚀 Featured Projects

### Marketing Recommender  
![marketing-recommender demo](./assets/recommender.gif)  
**Stack:** Python • Playwright • BeautifulSoup • Kafka • Spark • Celery • Redis • Ollama LLM • FastAPI • PostgreSQL • Docker • GPU Server • Ubuntu

**Highlights:**  
- Ingests clickstream via Kafka, aggregates hourly/daily metrics with Spark 
- Runs sentiment & keyword extraction through an on-prem LLM (Ollama)  
- Exposes a FastAPI dashboard that shows real-time KPIs, trends, and alerts  

#### Event-Driven Pipeline  
**Highlights:**  
- Designed a microservices architecture for processing millions of user events/day  
- Implemented Celery-like worker queues, back-pressure handling, and idempotency  
- Achieved 99.99% uptime.  

#### Content Analysis Service   
- Crawls web & social media, stores raw data in Postgres, cleans & tags with LLM  
- Aggregates brand-mention stats: sentiment, top keywords, source distribution  
- Provides a JSON API & web hook for downstream analytics platforms 

- 📝 [Live Demo](https://recommender.example.com) • 📖 [Repo](https://github.com/rstful/data-tips)


### Skin Analysis Service  
**Stack:** Node.js • NestJS • Python • RabbitMQ • Celery • Redis • PostgreSQL • AWS EC2 • AWS Route 53 • Nginx

**Highlights:**
- Microservices Architecture: Architected and deployed decoupled services for image ingestion, analysis, and results delivery—enabling horizontal scaling and fault isolation. (Nodejs, Nestjs)
- High-Performance Worker Pipeline: Built a Python-based Celery worker (producer) that performs advanced image preprocessing and ML inference, orchestrated via RabbitMQ and Redis for reliable task queuing and retry semantics.
- Resilience & Idempotency: Engineered end-to-end message retry and deduplication logic to guarantee exactly-once processing, even under spikes and failures.
- Global High Availability: Deployed across EU and US AWS regions with automated DNS failover (Route 53) and Nginx load balancing, achieving 99.99% service uptime.
- Data Integrity & Monitoring: Leveraged PostgreSQL for transactional storage of user analyses, supplemented with Prometheus/Grafana dashboards and alerting for real-time performance and error tracking.
- Deployment with github action
- End to End test.

- 📝 [Consumer Repo](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2)
- 📖 [Producer Repo](https://github.com/you/content-analysis)


### Customer CRM Backend API 
🚀 **Features**
- Core Functionality
  - Consultant Management - Complete CRUD operations with business rules
  - Customer Management - Customer profiles, preferences, and history
  - Authentication & Authorization - JWT-based auth with role-based access
  - Multi-Database Support - Primary, secondary, and analysis databases
  - File Storage - AWS S3 integration for document/image storage
  - Email Services - Templated email notifications
  - Internationalization - Multi-language support
  - API Documentation - Swagger/OpenAPI integration
- Architecture Features
  - Domain-Driven Design - Rich domain models with business logic
  - Repository Pattern - Abstracted data access layer
  - Use Case Pattern - Clear application business rules
  - Value Objects - Type-safe data validation (Email, Phone, etc.)
  - Unit of Work - Transaction management
  - Result Pattern - Explicit error handling without exceptions
  - Event Sourcing Ready - Domain events for audit trails

🛠️ **Technology Stack**
- Core Technologies
  - Runtime: Node.js 18+
  - Framework: NestJS 9+
  - Language: TypeScript 4.7+
  - Database: PostgreSQL 14+
  - ORM: TypeORM 0.3+
- Infrastructure
  - Authentication: JWT with RS256/HS256
  - File Storage: AWS S3
  - Email: NodeMailer with Handlebars templates
  - Logging: Winston with structured logging
  - Validation: class-validator with DTOs
  - Documentation: Swagger/OpenAPI 3.0
  - Testing: Jest with Supertest
- Development Tools
  - Code Quality: ESLint, Prettier
  - API Testing: Thunder Client, Postman
  - Database: pgAdmin, DBeaver
  - Containerization: Docker & Docker Compose

📋 **Prerequisites**
- Node.js 18+ and npm 8+
- PostgreSQL 14+
- Redis 6+ (for caching)
- Docker (optional, for containerization)
- AWS Account (for S3 storage in production)

[Repo](https://github.com/hpkn/Login_user_management)

### Additional Featured Projects

#### Career Document Matching Demo
**Stack:** Python • Streamlit • LLM • NLP • RAG

**Description:** 
An intelligent document matching system that uses LLM and NLP techniques to analyze and match career documents with job opportunities. The system leverages Retrieval Augmented Generation (RAG) for semantic understanding of career documents, achieving accurate skill-to-job mapping.

**Key Features:**
- Streamlit-based web interface for real-time document analysis
- - RAG pipeline for context-aware document processing
  - - Semantic similarity matching between career profiles and job descriptions
    - - Support for multiple document formats (PDF, DOCX)
      - - Deployed as system service on cloud infrastructure
        - - Live demo: https://ai-test.rs-team.com
         
          - 📖 [Repository](https://github.com/hpkn/career-document-matching-demo)
         
          - ---

          #### Login User Management System
          **Stack:** TypeScript • NestJS • PostgreSQL • JWT • TypeORM

          **Description:**
          A comprehensive user authentication and management system built with NestJS and TypeScript. The system provides role-based access control, JWT-based authentication, and secure user lifecycle management.

          **Key Features:**
          - JWT-based authentication with RS256/HS256 support
          - - Role-based access control (RBAC)
            - - User profile management and preferences
              - - Secure password hashing and validation
                - - Database transaction management with TypeORM
                  - - Comprehensive error handling
                    - - API documentation with Swagger
                     
                      - 📖 [Repository](https://github.com/hpkn/Login_user_management)
                     
                      - ---

                      #### BE-SKIN Analysis Sample v2
                      **Stack:** TypeScript • NestJS • Python • ML/AI • Image Processing

                      **Description:**
                      An advanced skin analysis service demonstrating machine learning integration with backend services. The project showcases best practices in building scalable microservices with async task processing.

                      **Key Features:**
                      - Image preprocessing and ML model inference
                      - - Celery-based async task processing
                        - - Results caching with Redis
                          - - Database transaction management
                            - - Error handling and data validation
                             
                              - 📖 [Repository](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2)
                             
                              - ---

                              #### LLM Pipeline Sample
                              **Stack:** Python • LLM • RAG • Transformers • Prompt Engineering

                              **Description:**
                              A production-ready template for building LLM-powered applications with the three main patterns: RAG (Retrieval Augmented Generation), fine-tuning, and prompt engineering. This sample demonstrates best practices for deploying LLM applications.

                              **Key Features:**
                              - RAG pipeline implementation with vector databases
                              - - Multi-model comparison and evaluation
                                - - Prompt optimization techniques
                                  - - Error handling and fallback strategies
                                    - - Production deployment configuration
                                     
                                      - 📖 [Repository](https://github.com/hpkn/llm-pipeline-sample)
                                     
                                      - ---

                                      #### Korean Multi-RAG Chatbot
                                      **Stack:** Python • RAG • LLM • FastAPI • Korean NLP

                                      **Description:**
                                      A specialized chatbot system optimized for Korean language processing using multi-source RAG. The system integrates multiple knowledge bases and uses advanced NLP techniques for context-aware responses.

                                      **Key Features:**
                                      - Multi-source RAG implementation
                                      - - Korean language-specific NLP processing
                                        - - FastAPI backend with async support
                                          - - Knowledge base management
                                            - - Context-aware response generation
                                             
                                              - 📖 [Repository](https://github.com/hpkn/korean_multi_rag_chabot)
                                             
                                              - ---

                                              #### File Data Extraction Template
                                              **Stack:** Python • Data Extraction • PDF Processing

                                              **Description:**
                                              A versatile Python template for extracting structured data from various file formats including Excel, PDF, HWPX (Korean Word Format), and Word documents. Useful for document processing pipelines and data consolidation.

                                              **Key Features:**
                                              - Support for multiple file formats (PDF, Excel, HWPX, DOCX)
                                              - - Structured data extraction
                                                - - Data validation and cleaning
                                                  - - Batch processing capability
                                                    - - Error handling for malformed files
                                                     
                                                      - 📖 [Repository](https://github.com/hpkn/file_data_extraction_template)
                                                     
                                                      - ---

                                                      #### TIPS Model Test (Jupyter Notebook)
                                                      **Stack:** Python • Jupyter • Machine Learning • Model Evaluation

                                                      **Description:**
                                                      A Jupyter notebook environment for testing and evaluating machine learning models. Includes utilities for model comparison, performance metrics, and visualization.

                                                      📖 [Repository](https://github.com/rstful/TIPS-Model-Test)

                                                      ---

                                                      #### Local LLM Test
                                                      **Stack:** Python • Ollama • LLM • Local Inference

                                                      **Description:**
                                                      Demonstrates running large language models locally using Ollama, enabling offline LLM inference and fine-tuning without cloud dependencies. Useful for privacy-sensitive applications and development.

                                                      📖 [Repository](https://github.com/rstful/local-llm-test)

                                                      ---

                                                      #### Coupon Generator
                                                      **Stack:** Python • Data Generation

                                                      **Description:**
                                                      A utility tool for generating coupon codes with validation. Implements coupon generation logic with uniqueness guarantees and configurable parameters.

                                                      📖 [Repository](https://github.com/rstful/coupon-generator)

                                                      ---

                                                      #### Africa Bid Management
                                                      **Stack:** Python • Django • Business Logic

                                                      **Description:**
                                                      A bidding management system for African business operations. Handles bid creation, evaluation, and award processing.

                                                      📖 [Repository](https://github.com/hpkn/africa_bid)

                                                      ---

                                                      #### Local Image Generation with Ollama
                                                      **Stack:** Python • Ollama • Image Generation • Local Inference

                                                      **Description:**
                                                      Demonstrates running image generation models locally using Ollama, enabling offline image synthesis without cloud services or external APIs.

                                                      📖 [Repository](https://github.com/hpkn/local-image-generation-ollama)

                                                      ---

---

## 🛠 Tech Stack

| Language           | Frameworks       | Data & Messaging         | DevOps & Cloud             | AI/LLM/ML    
|--------------------|------------------|--------------------------|----------------------------|--------------------------------------------------
| Python             | FastAPI, Flask   | Kafka, Spark, PostgreSQL | Docker, AWS, Tencent Cloud |Deep learning and ML concepts, Transformers, fine-tuning, RAG pipelines, LangChain, HuggingFace
| Node.js, Typescript| NestJS, Express  | Redis, RabbitMQ          | GitHub Actions             |
| Rails              | Ruby on Rails    | Celery                   |                            |

---

## 📊 GitHub Stats

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=hpkn&show_icons=true)](https://github.com/hpkn)

---

## 📫 Contact

- 📧 hassangpaul@gmail.com  
- 💼 [LinkedIn](https://www.linkedin.com/in/hassangpaul/)  

---

> "Simplicity is the ultimate sophistication." – Leonardo da Vinci

---
---

<a name="korean"></a>
# 🇰🇷 한국어 버전

# 👋 안녕하세요, Paul N. KAPUKU입니다

> 💻 백엔드 엔지니어 | Python • Javascript • Kafka • Spark • FastAPI • NodeJS/Nestjs • Nginx • Docker • SQL • NoSql • AWS • LLM • AI 엔지니어링 • ML 및 AI 기초

---

##

> 🔭 현재 LLM 기반 인사이트를 활용한 마케팅 추천 엔진을 개발 중입니다  
> 🌱 데이터 중심 아키텍처와 분산 시스템에 대해 꾸준히 학습하고 있습니다  
> 📫 연락처: hassangpaul@gmail.com   |  [LinkedIn](https://linkedin.com/in/hassangpaul)

---

## 📋 목차

- [자기소개](#자기소개)  
- [주요 프로젝트](#주요-프로젝트)  
  - [마케팅 추천 시스템](#마케팅-추천-시스템)  
  - [이벤트 기반 파이프라인](#이벤트-기반-파이프라인)  
  - [콘텐츠 분석 서비스](#콘텐츠-분석-서비스)  
  - [피부 분석 서비스](#피부-분석-서비스)
  - [고객 CRM 백엔드 API](#고객-crm-백엔드-api)
- [기술 스택](#기술-스택)  
- [GitHub 통계](#github-통계)  
- [연락처](#연락처-정보)

---

## 📝 자기소개

저는 5년간의 경험을 보유한 백엔드 엔지니어로, 실시간 데이터 파이프라인, 마이크로서비스, AI 기반 API를 구축해왔습니다. 중견 스타트업에서 프로젝트를 이끌었으며, 관찰 가능성, 테스팅, 클라우드 아키텍처 모범 사례에 대해 주니어 개발자들을 멘토링하는 것을 즐깁니다.

---

## 🚀 주요 프로젝트

### 마케팅 추천 시스템  
![marketing-recommender demo](./assets/recommender.gif)  
**기술 스택:** Python • Playwright • BeautifulSoup • Kafka • Spark • Celery • Redis • Ollama LLM • FastAPI • PostgreSQL • Docker • GPU Server • Ubuntu

**주요 특징:**  
- Kafka를 통한 클릭스트림 수집, Spark로 시간별/일별 메트릭 집계
- 온프레미스 LLM(Ollama)을 통한 감정 분석 및 키워드 추출 실행
- 실시간 KPI, 트렌드, 알림을 보여주는 FastAPI 대시보드 제공

#### 이벤트 기반 파이프라인  
**주요 특징:**  
- 일일 수백만 건의 사용자 이벤트를 처리하는 마이크로서비스 아키텍처 설계
- Celery 유사 워커 큐, 백프레셔 처리 및 멱등성 구현
- 99.99% 가동 시간 달성

#### 콘텐츠 분석 서비스   
- 웹 및 소셜 미디어 크롤링, Postgres에 원시 데이터 저장, LLM으로 정제 및 태깅
- 브랜드 언급 통계 집계: 감정, 주요 키워드, 소스 분포
- 다운스트림 분석 플랫폼을 위한 JSON API 및 웹훅 제공

- 📝 [라이브 데모](https://recommender.example.com) • 📖 [저장소](https://github.com/rstful/data-tips)


### 피부 분석 서비스  
**기술 스택:** Node.js • NestJS • Python • RabbitMQ • Celery • Redis • PostgreSQL • AWS EC2 • AWS Route 53 • Nginx

**주요 특징:**
- 마이크로서비스 아키텍처: 이미지 수집, 분석, 결과 전달을 위한 분리된 서비스를 설계 및 배포하여 수평적 확장과 장애 격리 가능 (Nodejs, Nestjs)
- 고성능 워커 파이프라인: 고급 이미지 전처리 및 ML 추론을 수행하는 Python 기반 Celery 워커(생산자) 구축, RabbitMQ와 Redis를 통한 신뢰성 있는 작업 큐잉 및 재시도 처리
- 복원력 및 멱등성: 스파이크 및 장애 상황에서도 정확히 한 번 처리를 보장하는 엔드투엔드 메시지 재시도 및 중복 제거 로직 구현
- 글로벌 고가용성: EU 및 미국 AWS 리전에 배포, 자동 DNS 페일오버(Route 53) 및 Nginx 로드 밸런싱으로 99.99% 서비스 가동 시간 달성
- 데이터 무결성 및 모니터링: 사용자 분석의 트랜잭션 저장을 위한 PostgreSQL 활용, Prometheus/Grafana 대시보드 및 실시간 성능 및 오류 추적을 위한 알림 시스템 구축
- GitHub Actions를 통한 배포
- 엔드투엔드 테스트

- 📝 [Consumer 저장소](https://github.com/hpkn/BE-SKIN-Analysis-sample-v2)
- 📖 [Producer 저장소](https://github.com/you/content-analysis)


### 고객 CRM 백엔드 API 
🚀 **기능**
- 핵심 기능
  - 컨설턴트 관리 - 비즈니스 규칙이 포함된 완벽한 CRUD 작업
  - 고객 관리 - 고객 프로필, 선호도 및 이력
  - 인증 및 권한 부여 - 역할 기반 접근 제어를 포함한 JWT 기반 인증
  - 다중 데이터베이스 지원 - 기본, 보조 및 분석 데이터베이스
  - 파일 저장소 - 문서/이미지 저장을 위한 AWS S3 통합
  - 이메일 서비스 - 템플릿 기반 이메일 알림
  - 국제화 - 다국어 지원
  - API 문서화 - Swagger/OpenAPI 통합
- 아키텍처 기능
  - 도메인 주도 설계 - 비즈니스 로직이 포함된 풍부한 도메인 모델
  - 리포지토리 패턴 - 추상화된 데이터 접근 계층
  - 유스케이스 패턴 - 명확한 애플리케이션 비즈니스 규칙
  - 값 객체 - 타입 안전 데이터 검증 (이메일, 전화번호 등)
  - 작업 단위 - 트랜잭션 관리
  - 결과 패턴 - 예외 없는 명시적 오류 처리
  - 이벤트 소싱 준비 - 감사 추적을 위한 도메인 이벤트

🛠️ **기술 스택**
- 핵심 기술
  - 런타임: Node.js 18+
  - 프레임워크: NestJS 9+
  - 언어: TypeScript 4.7+
  - 데이터베이스: PostgreSQL 14+
  - ORM: TypeORM 0.3+
- 인프라
  - 인증: RS256/HS256을 사용한 JWT
  - 파일 저장소: AWS S3
  - 이메일: Handlebars 템플릿을 사용한 NodeMailer
  - 로깅: 구조화된 로깅을 위한 Winston
  - 검증: DTO를 사용한 class-validator
  - 문서화: Swagger/OpenAPI 3.0
  - 테스팅: Supertest를 사용한 Jest
- 개발 도구
  - 코드 품질: ESLint, Prettier
  - API 테스팅: Thunder Client, Postman
  - 데이터베이스: pgAdmin, DBeaver
  - 컨테이너화: Docker & Docker Compose

📋 **필수 요구사항**
- Node.js 18+ 및 npm 8+
- PostgreSQL 14+
- Redis 6+ (캐싱용)
- Docker (선택사항, 컨테이너화용)
- AWS 계정 (프로덕션 S3 저장소용)

[저장소](https://github.com/hpkn/Login_user_management)

---

## 🛠 기술 스택

| 언어               | 프레임워크       | 데이터 및 메시징         | DevOps 및 클라우드         | AI/LLM/ML    
|--------------------|------------------|--------------------------|----------------------------|--------------------------------------------------
| Python             | FastAPI, Flask   | Kafka, Spark, PostgreSQL | Docker, AWS, Tencent Cloud |딥러닝 및 ML 개념, Transformers, 파인튜닝, RAG 파이프라인, LangChain, HuggingFace
| Node.js, Typescript| NestJS, Express  | Redis, RabbitMQ          | GitHub Actions             |
| Rails              | Ruby on Rails    | Celery                   |                            |

---

## 📊 GitHub 통계

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=hpkn&show_icons=true)](https://github.com/hpkn)

---

## 📫 연락처 정보

- 📧 hassangpaul@gmail.com  
- 💼 [LinkedIn](https://www.linkedin.com/in/hassangpaul/)  

---

> "단순함은 궁극의 정교함이다." – 레오나르도 다 빈치
