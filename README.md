# Paul Kapuku Software Portfolio
# 👋 Hi, I’m Paul N. KAPUKU

> 💻 Backend Engineer | Python • Javascript • Kafka • Spark • FastAPI • NodeJS/Nestjs • Nginx • Docker • SQL • NoSql • AWS • LLM • AI Enginering • ML and AI fundamentals

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
- [Tech Stack](#tech-stack)  
- [GitHub Stats](#github-stats)  
- [Contact](#contact)

---

## 📝 About Me

I’m a backend engineer with 5 years of experience building real-time data pipelines, microservices, and AI-powered APIs. I’ve led projects at midsize startups and enjoy mentoring juniors on best practices in observability, testing, and cloud architecture.

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

- 📝 [Consumer Repo](https://recommender.example.com) •
- 📖 [Producer Repo](https://github.com/you/content-analysis)

---

## 🛠 Tech Stack

| Language           | Frameworks       | Data & Messaging         | DevOps & Cloud             | AI/LLM/ML    
|--------------------|------------------|--------------------------|----------------------------|--------------------------------------------------
| Python             | FastAPI, Flask   | Kafka, Spark, PostgreSQL | Docker, AWS, Tencent Cloud |Deep learning and ML concepts, Transformers, fine-tuning, RAG pipelines, LangChain, HuggingFace
| Node.js, Typescript| NestJS, Express  | Redis, RabbitMQ          | GitHub Actions             |
| Rails              | Ruby on Rails    | Celey                    |                            |



---

## 📊 GitHub Stats

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=hpkn&show_icons=true)](https://github.com/hpkn)

---

## 📫 Contact

- 📧 hassangpaul@gmail.com  
- 💼 [LinkedIn](https://www.linkedin.com/in/hassangpaul/)  

---

> “Simplicity is the ultimate sophistication.” – Leonardo da Vinci
