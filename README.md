<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:0f3460&height=180&section=header&text=Heewon%20Lee&fontSize=56&fontColor=58a6ff&fontAlignY=40&desc=Backend%20Developer%20%7C%20AI%20%2B%20IoT%20%7C%20Vibe%20Coder&descAlignY=62&descSize=18&descColor=8b949e&animation=fadeIn" width="100%"/>

</div>

<div align="center">

[![Portfolio](https://img.shields.io/badge/웹_포트폴리오-0f3460?style=flat-square&logo=googlechrome&logoColor=white)](https://heewonn09.github.io/portfolio/)
[![Notion](https://img.shields.io/badge/노션_포트폴리오-000000?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/35eed7ed6e4480099195c22cf179891a?source=copy_link)
[![Velog](https://img.shields.io/badge/Velog-20C997?style=flat-square&logo=velog&logoColor=white)](https://velog.io/@heewonn09)
[![Tistory](https://img.shields.io/badge/Tistory-FF5722?style=flat-square&logo=tistory&logoColor=white)](https://heewonn09.tistory.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/heewonn09)
[![Email](https://img.shields.io/badge/heewonn09@naver.com-03C75A?style=flat-square&logo=naver&logoColor=white)](mailto:heewonn09@naver.com)

</div>

---

## 🙋 About Me

> **서비스 병목을 분석하고, 성능과 비용을 개선하는 구조를 설계하는 백엔드 개발자**

- 🖥️ **Spring Boot** 기반 REST API 설계 · 구현 · 운영까지 고려한 백엔드 개발
- 🧠 **RAG + LLM** 구조 설계로 AI 챗봇 응답속도 **4 ~ 5초 → 0.3 ~ 0.8초** 단축, 비용 **80% 절감**
- 📡 **MQTT 기반 IoT** 디바이스 제어 + 자연어 → 디바이스 명령 변환 시스템 구현
- 🤖 **Vibe Coding** — OpenAI Codex · Claude Code로 설계 기반 AI 협업 개발 경험
- 🔌 **MCP 연동** — filesystem · GitHub · Notion · Pinecone MCP 서버 활용 경험
- 🐳 **Docker Compose** 컨테이너화 + **GitHub Actions** CI/CD 파이프라인 구성

---

## ⚡ Key Achievements

| 지표 | Before | After | 개선율 |
|:---:|:---:|:---:|:---:|
| 챗봇 평균 응답시간 | 4~5초 | 0.3~0.8초 | **↑ 90%** |
| LLM 토큰 사용량 | 기준치 | 60~80% 절감 | **↓ 80%** |
| 특정 API 응답속도 | 기준치 | 쿼리 + 인덱스 최적화 | **유의미하게 개선** |
| 컨테이너 환경 재현성 | 수동 설정 | docker compose up | **100%** |

---

## 🤖 Vibe Coding — Mindflow 바이브 코딩 경험
<details>
<summary><b>🧠 Mindflow — AI 행동 코칭 챗봇 (클릭해서 펼치기)</b></summary>

<br/>

### 📌 프로젝트 개요
행동 로그 × 감정 패턴 분석 × AI 피드백 코칭을 연결한 풀스택 서비스.  
**설계와 조사는 직접**, 구현은 **OpenAI Codex + Claude Code로 바이브 코딩** 방식으로 진행.

---

### 🎯 바이브 코딩 적용 방식

| 단계 | 담당 | 도구 |
|:---|:---|:---:|
| 아키텍처 설계 · 기술 조사 | 직접 설계 | - |
| 전체 모듈 초기 생성 | 프롬프트 기반 코드 생성 | OpenAI Codex |
| 기존 코드 리팩토링 | 구조 개선 지시 | Claude Code |
| 버그 수정 · 디버깅 | AI 보조 디버깅 | Claude Code |
| 아키텍처 검토 · 개선 | 설계 리뷰 | Claude Code |

---

### 🔌 MCP 연동 경험

```
📁 Filesystem MCP     — 로컬 파일 읽기/쓰기 자동화, 코드 파일 직접 수정
🐙 GitHub MCP         — 레포 연동, 코드 push · PR 생성 자동화
📋 Notion MCP         — 개발 일지 · 스펙 문서 자동 동기화
🌲 Pinecone MCP       — Vector DB 데이터 삽입 · 조회 자동화 연동
```

---

### 🛠️ 리팩토링 포인트 (Claude Code 활용)

**Before (바이브 코딩 초기)**
```python
# 모든 분석 로직이 단일 함수에 집중
def analyze(data):
    # 500줄짜리 God Function
    ...
```

**After (Claude Code 리팩토링)**
```python
# 계층 분리: PatternAnalysisService
class PatternAnalysisService:
    def analyze_frequency(self) -> FrequencyResult: ...
    def analyze_intensity(self) -> IntensityResult: ...
    def analyze_trend(self)    -> TrendResult:     ...

# /api/ui ViewModel 계층 — 프론트 데이터 조립 비용 최소화
class UIViewModel:
    def build_dashboard_response(self) -> DashboardDTO: ...
```

---

### 🏗️ 아키텍처

```
User → React(Vite) → FastAPI Backend
                          ├── JWT Auth (HS256)
                          ├── PatternAnalysisService
                          ├── MySQL / Redis (캐시 · Rate Limit)
                          └── Gemini API ──► fallback 분석 텍스트 (API 미연동 시 자동 전환)
```

---

### 📈 성과 및 개선점

| 항목 | 내용 |
|:---|:---|
|  **환경 재현성** | Docker Compose로 MySQL + Redis + Backend 3서비스 컨테이너화, 재현성 100% |
|  **CI/CD** | GitHub Actions — lint + build 자동화, PR 머지 시 자동 검증 |
|  **AI 안정성** | Gemini fallback 구조 — 네트워크 장애 시에도 서비스 전체 흐름 유지 |
|  **캐시 최적화** | Redis 적용으로 분석 API 반복 호출 비용 절감 |
| 🔧 **개선점** | Codex 생성 초기 코드의 God Function 문제 → Claude Code로 계층 분리 리팩토링 |
| 🔧 **개선점** | 바이브 코딩 특성상 초기 테스트 커버리지 부족 → 핵심 로직 단위 테스트 보완 필요 |
| 🔧 **개선점** | AI 생성 코드의 일관성 유지를 위해 코드 컨벤션 문서화 필요성 인식 |

---

### 💡 바이브 코딩을 통해 얻은 인사이트

> AI가 코드를 생성해도 **설계 의도와 구조적 판단은 개발자의 몫**임을 체감.  
> 프롬프트의 품질이 곧 코드 품질로 이어졌고, 리팩토링 지시 시 **명확한 맥락 제공**이 핵심이었음.  
> MCP 연동으로 반복 작업(파일 수정, PR, 문서화)을 자동화하면서 **개발 흐름에 집중**할 수 있었음.

</details>

---

## 🏠 Projects

<details>
<summary><b>🏠 NOVA — 스마트 아파트 통합관리 플랫폼 (클릭해서 펼치기)</b></summary>

<br/>

> **LLM 호출 구조 개선으로 비용 80% 절감 / 응답속도 90% 개선**  
> [📎 GitHub](https://github.com/heewonn09)

**기술 스택**  
`Spring Boot` `JPA` `MySQL` `MariaDB` `MQTT` `RAG` `Pinecone` `Gemini API` `React Native` `React` `Docker` `GitHub Actions` `Swagger`

**핵심 역할**
- Rule 기반 Dispatcher 설계 — 단순 명령은 DB/API, 복잡 질의만 LLM+RAG 처리
- RAG 챗봇 파이프라인 구현 (Embedding → Pinecone → 검색 → 응답)
- 자연어 → MQTT 제어 명령 변환 로직 구현
- Controller → Service → Repository 계층 구조로 REST API 설계
- 쿼리 구조 개선 + 인덱스 적용으로 API 응답속도 유의미하게 개선

**성과**

| 항목 | 수치 |
|:---|:---:|
| LLM 토큰 사용량 | **60~80% 절감** |
| 챗봇 응답시간 | **4~5초 → 0.3~0.8초** |
| IoT 제어 | 자연어 기반 디바이스 제어 구현 |

</details>

<details>
<summary><b>🚗 스마트 주차장 — 모빌리티 허브 (클릭해서 펼치기)</b></summary>

<br/>

> **OCR 자동 승인 → 관리자 확인 기반 반자동 구조로 전환**  
> [📎 GitHub](https://github.com/heewonn09)

**기술 스택**  
`Spring Boot` `JPA` `MySQL` `MQTT` `Raspberry Pi` `Python` `React`

**핵심 역할**
- 입차 승인 로직 설계 및 구현
- 라인트레이서 기반 차량 감지 처리
- 관리자 승인 버튼 → MQTT 기반 서보모터 제어 연결
- OCR 한계를 빠르게 판단하고 서비스 동작 중심으로 구조 재설계

**성과**  
OCR 인식 실패로 멈출 수 있었던 프로젝트를 대체 로직으로 완성, MQTT 실시간 제어로 응답 지연 최소화

</details>

<details>
<summary><b>📱 헬스케어 관리 앱 — 스마트프로그래밍 대외경진대회 수상 (클릭해서 펼치기)</b></summary>

<br/>

> **2023년 백석대학교 컴퓨터공학부 스마트프로그래밍 대외경진대회**

**기술 스택**  
`Android` `Java` `SQLite` `공공데이터 API` `XML`

**핵심 역할**
- BMI 계산 및 상태 분류, SQLite 기반 회원가입/로그인 구현
- 공공데이터 API 연동으로 음식 검색 시 열량·영양 정보 조회
- XML 파싱 기반 비동기 데이터 처리 구현
- 날짜별 식단 다이어리 기능 설계 및 구현

</details>

---

## 🛠️ Tech Stack

### 🖥️ Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Framework](https://img.shields.io/badge/Spring_Framework-6DB33F?style=flat-square&logo=spring&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-005571?style=flat-square)

### 🗄️ Database
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone_VectorDB-3C3C3C?style=flat-square)

### 🧠 AI / ML
![RAG](https://img.shields.io/badge/RAG-FF6F00?style=flat-square)
![Gemini API](https://img.shields.io/badge/Gemini_API-4285F4?style=flat-square&logo=googlegemini&logoColor=white)
![LLM](https://img.shields.io/badge/LLM_Integration-000000?style=flat-square)
![Text Embedding](https://img.shields.io/badge/Text_Embedding-7B61FF?style=flat-square)

### 🤖 AI Dev Tools (Vibe Coding)
![Claude Code](https://img.shields.io/badge/Claude_Code-CC785C?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI Codex](https://img.shields.io/badge/OpenAI_Codex-412991?style=flat-square&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_Server-000000?style=flat-square&logo=anthropic&logoColor=white)

### 📡 IoT / Embedded
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878A?style=flat-square&logo=arduino&logoColor=white)
![Mosquitto](https://img.shields.io/badge/Mosquitto-3C5280?style=flat-square&logo=eclipsemosquitto&logoColor=white)

### 🔗 Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22B5BF?style=flat-square)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)
![Android](https://img.shields.io/badge/Android-34A853?style=flat-square&logo=android&logoColor=white)

### 💻 Languages
![Java](https://img.shields.io/badge/Java-F89820?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000000)

### 🐳 Infra / DevOps
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![MSA](https://img.shields.io/badge/MSA-FF6F00?style=flat-square)

### 🔧 Tools
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![IntelliJ](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=000000)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![DBeaver](https://img.shields.io/badge/DBeaver-382923?style=flat-square)
![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white)



<div align="center">

📧 **heewonn09@naver.com** &nbsp;|&nbsp; 📱 **010-5129-8600**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,50:161b22,100:0d1117&height=100&section=footer&animation=fadeIn" width="100%"/>

</div>
