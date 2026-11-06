## Park Young Hyun (박영현)
**Cloud & AI Solutions Engineer** — *Google Cloud · Generative AI Agents · RAG & Data Pipelines*

![Metrics](/github-metrics-yhp2205.svg)

## 📫 Contacts
- **Email** : yhp2205@gmail.com
- **Role** : Cloud & AI Solutions Engineer (2024.09 ~ Present)

<br/>

## ⌨️ Skills & Tech Stack
**Core Stack** : 프로덕션 설계 · 구축 · 운영 기술

<p>
  <img alt="Google Cloud" src="https://img.shields.io/badge/Google_Cloud-4285F4.svg?&style=flat-square&logo=googlecloud&logoColor=white"/>
  <img alt="Vertex AI" src="https://img.shields.io/badge/Vertex_AI_&_ADK-4285F4.svg?&style=flat-square&logo=googlecloud&logoColor=white"/>
  <img alt="Google Gemini" src="https://img.shields.io/badge/Google_Gemini-8E75B2.svg?&style=flat-square&logo=googlegemini&logoColor=white"/>
  <img alt="BigQuery" src="https://img.shields.io/badge/BigQuery-669DF6.svg?&style=flat-square&logo=googlebigquery&logoColor=white"/>
  <img alt="PostgreSQL" src="https://img.shields.io/badge/Cloud_SQL_(pgvector)-4169E1.svg?&style=flat-square&logo=postgresql&logoColor=white"/>
  <img alt="Cloud Run" src="https://img.shields.io/badge/Cloud_Run-4285F4.svg?&style=flat-square&logo=googlecloud&logoColor=white"/>
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED.svg?&style=flat-square&logo=docker&logoColor=white"/>
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB.svg?&style=flat-square&logo=python&logoColor=white"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6.svg?&style=flat-square&logo=typescript&logoColor=white"/>
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB.svg?&style=flat-square&logo=react&logoColor=black"/>
</p>

- **Generative AI & Multi-Agent** : `Google ADK` · `Gemini Enterprise` · `Gemini API (Multimodal · Structured Output)` 기반 도메인 특화 멀티 에이전트 설계 및 배포
- **RAG & Document Intelligence** : `Vertex AI RAG Engine` · `Document AI` · 합본 PDF 3단계 하이브리드 분할기 및 비정형 표 파서 직접 구현
- **Search & Vector DB** : `Vertex AI Search` 개인화 추천 시스템 엔드투엔드 단독 구축 및 `Cloud SQL(PostgreSQL + pgvector)` 임베딩(`HNSW`) 검색 구현
- **Data Engineering** : `BigQuery(DTS · Scheduled Queries)` 기반 대규모 데이터 마트(560만~700만 행) 운영, `live/history` 이중 테이블 + `data_hash` 증분 파이프라인 설계
- **Cloud Native & FinOps** : `Cloud Run` · `Cloud Functions` · `Pub/Sub` · `Docker` 서버리스 컨테이너 배포, `Log Sink → GCS` 아키텍처 비용 최적화 및 무중단 인프라 운영

<br/>

## 🚀 Key Engineering Highlights
- **멀티 에이전트 추론 지연 90% 단축 및 환각 제어**
  - BigQuery 6종 사전 병렬 조회 및 LLM 근거 확인 병렬 호출(`concurrency=6`)로 응답 시간을 **45~104초 → 6~8초**로 단축하고, 툴 타임아웃 시 허위 보고서 생성을 차단하는 **4겹 결정론적 출력 가드(`output_guard.py`)** 구현
- **비정형 PDF 파싱 고도화 및 고정밀 법령·규정 RAG 구축**
  - 규칙 기반 헤더 Gate(단일 문서 LLM 비용 0원) + Flash 경계 분할 + 연속성 검증 가드/정규식 Fallback을 결합한 **3단계 하이브리드 분할기(`bundle_splitter.py`)** 설계 및 스니펫 길이 정규화(`matched / sqrt(length)`)로 장문 인용 편향 해결
- **증분형 개인화 추천 파이프라인 단독 구축 (~20,000건 규모)**
  - BigQuery `live`/`history` 분리 아키텍처와 `data_hash` 변경 감지로 기존 LLM 추출 메타데이터를 보존(재추출 비용 0원화)하고, `Vertex AI Search` 색인 및 `Cloud Run` 추천 API 서빙 전 구간 구축
- **엔터프라이즈 클라우드 무중단 운영 (MSP) 및 FinOps**
  - 멀티 프로젝트(GCP 프로젝트 4개 · 운영기 VM 16대) 환경에서 데이터 마트 적재 중단 RCA 규명 및 **20개월 치 무결성 백필**, `Cloud SQL` EoS 무중단 스위치오버, `CIS 496건 / CVE 296건` 야간 패치, **Cloud Logging 비용 약 90% 절감** 수행

<br/>

## 🏆 Certifications
- **Google Cloud Certified — Professional Cloud Architect (PCA)** (2024.11)
- **Google Cloud Certified — Professional Data Engineer (PDE)** (2026.01)
- **Google Cloud Certified — Associate Cloud Engineer (ACE)** (2026)
- **Gemini Enterprise Certified Partner Specialist** (2026)
- **SQLD (국가공인 SQL 개발자)** (2025) · **ADsP (국가공인 데이터분석 준전문가)** (2024)

<br/>

## 📖 Education & Activities
- **Technical Speaker & Enablement** (2026)
  - Google Workspace Discovery Day 기업 고객 50인 단독 발표 (*「Gemini Enterprise × GWS 부서별 실무 적용」*)
  - 7개 주요 병원·기업 약 490인 규모(누적 339인 완료 · 150인 예정) 생성형 AI 핸즈온 실습 환경 단독 프로비저닝 및 현장 기술지원
- **GoogleCloud 기반 인공지능 개발자 과정 (SeSAC, 752시간)** (2023.10.04 ~ 2024.02.11)
  - Vertex AI Workbench Multi-GPU 기반 고속도로 CCTV 차량 인식 `YOLOv8` 모델 파인튜닝 (`mAP50-95: 0.743 → 0.823`)
- **연세대학교 미래캠퍼스** (2024.08 졸업)
  - 정보통계학과 · 인지과학 연계전공 학사
  - Google Developer Student Clubs (GDSC, 2020 ~ 2021)
