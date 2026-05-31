<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f2937&height=160&section=header&text=Heewon%20Lee&fontSize=48&fontColor=ffffff&fontAlignY=42&desc=Backend%20Developer&descAlignY=62&descSize=16&descColor=9ca3af&animation=fadeIn" width="100%"/>

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-111827?style=flat-square&logo=googlechrome&logoColor=white)](https://heewonn09.github.io/portfolio/)
[![Notion](https://img.shields.io/badge/Notion-111827?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/35eed7ed6e4480099195c22cf179891a?source=copy_link)
[![Velog](https://img.shields.io/badge/Velog-111827?style=flat-square&logo=velog&logoColor=20C997)](https://velog.io/@heewonn09)
[![Tistory](https://img.shields.io/badge/Tistory-111827?style=flat-square&logo=tistory&logoColor=white)](https://heewonn09.tistory.com)
[![GitHub](https://img.shields.io/badge/GitHub-111827?style=flat-square&logo=github&logoColor=white)](https://github.com/heewonn09)
[![Email](https://img.shields.io/badge/heewonn09@naver.com-111827?style=flat-square&logo=naver&logoColor=03C75A)](mailto:heewonn09@naver.com)

</div>

<br/>

서비스 병목을 분석하고, **성능과 비용을 개선하는 구조를 설계하는 백엔드 개발자**입니다.
Spring Boot 기반 REST API 개발부터 RAG 챗봇 시스템, IoT 디바이스 연동, Vibe Coding까지 — 기능 구현을 넘어 구조적인 의사결정을 추구합니다.

<br/>

---

## About Me

- Spring Boot 기반 REST API 설계 · 구현 · 운영까지 고려한 백엔드 개발
- RAG + LLM 구조 설계로 AI 챗봇 응답속도 **4~5초 → 0.3~0.8초** 단축, 비용 **80% 절감**
- MQTT 기반 IoT 디바이스 제어 + 자연어 → 디바이스 명령 변환 시스템 구현
- OpenAI Codex · Claude Code 기반 **Vibe Coding** — 설계 주도 AI 협업 개발 경험
- filesystem · GitHub · Notion · Pinecone **MCP 서버 연동** 경험
- Docker Compose 컨테이너화 + GitHub Actions CI/CD 파이프라인 구성

<br/>

---

## Key Achievements

| 지표 | Before | After | 결과 |
|:--|:--:|:--:|:--:|
| 챗봇 평균 응답시간 | 4 ~ 5초 | 0.3 ~ 0.8초 | **90% 개선** |
| LLM 토큰 사용량 | — | 60 ~ 80% 절감 | **비용 80% ↓** |
| 특정 API 응답속도 | — | 쿼리 + 인덱스 최적화 | **유의미하게 개선** |
| 컨테이너 환경 재현성 | 수동 설정 | `docker compose up` 단일 명령 | **100% 재현** |

<br/>

---

## Projects

<details>
<summary>&nbsp;<b>NOVA &nbsp;—&nbsp; 스마트 아파트 통합관리 플랫폼</b>&nbsp; <code>Main Project</code></summary>

<br/>

LLM 호출 구조를 Rule 기반으로 재설계해 **비용 80% 절감, 응답속도 90% 개선**을 달성한 IoT + AI 통합 플랫폼.

**Tech**
`Spring Boot` `JPA` `MySQL` `MariaDB` `MQTT` `RAG` `Pinecone` `Gemini API` `React Native` `React` `Docker` `GitHub Actions` `Swagger`

**핵심 역할**

- Rule 기반 Dispatcher 설계 — 단순 명령은 DB/API, 복잡 질의만 LLM + RAG 처리
- RAG 챗봇 파이프라인 구현 (Embedding → Pinecone → 검색 → 응답)
- 자연어 → MQTT 제어 명령 변환 로직 구현
- Controller → Service → Repository 계층 구조 REST API 설계
- 쿼리 구조 개선 + 인덱스 적용으로 API 응답속도 유의미하게 개선

**성과**

| 항목 | 결과 |
|:--|:--|
| LLM 토큰 사용량 | 60 ~ 80% 절감 |
| 챗봇 응답시간 | 4 ~ 5초 → 0.3 ~ 0.8초 |
| IoT 제어 | 자연어 기반 디바이스 제어 구현 |

</details>

---

<details>
<summary>&nbsp;<b>Mindflow &nbsp;—&nbsp; AI 행동 코칭 챗봇</b>&nbsp; <code>Vibe Coding</code></summary>

<br/>

행동 로그 × 감정 패턴 분석 × AI 피드백 코칭을 연결한 풀스택 서비스.
**설계와 조사는 직접**, 구현은 OpenAI Codex + Claude Code **Vibe Coding** 방식으로 진행.

**Tech**
`FastAPI` `SQLAlchemy` `MySQL` `Redis` `Gemini API` `React` `Vite` `Recharts` `Docker Compose` `GitHub Actions`

---

**Vibe Coding 적용 방식**

| 단계 | 방식 | 도구 |
|:--|:--|:--:|
| 아키텍처 설계 · 기술 조사 | 직접 설계 | — |
| 전체 모듈 초기 생성 | 프롬프트 기반 코드 생성 | OpenAI Codex |
| 기존 코드 리팩토링 | 구조 개선 지시 | Claude Code |
| 버그 수정 · 디버깅 | AI 보조 디버깅 | Claude Code |
| 아키텍처 검토 · 개선 | 설계 리뷰 | Claude Code |

---

**MCP 연동 경험**

```
Filesystem MCP   —  로컬 파일 읽기/쓰기 자동화, 코드 파일 직접 수정
GitHub MCP       —  레포 연동, 코드 push · PR 생성 자동화
Notion MCP       —  개발 일지 · 스펙 문서 자동 동기화
Pinecone MCP     —  Vector DB 데이터 삽입 · 조회 자동화 연동
```

---

**리팩토링 — Claude Code 적용 전후**

Before
```python
# 모든 분석 로직이 단일 함수에 집중
def analyze(data):
    # 500줄짜리 God Function
    ...
```

After
```python
# 계층 분리 — PatternAnalysisService
class PatternAnalysisService:
    def analyze_frequency(self) -> FrequencyResult: ...
    def analyze_intensity(self) -> IntensityResult: ...
    def analyze_trend(self)    -> TrendResult:     ...

# /api/ui ViewModel 계층 — 프론트 데이터 조립 비용 최소화
class UIViewModel:
    def build_dashboard_response(self) -> DashboardDTO: ...
```

---

**Architecture**

```
User → React (Vite) → FastAPI Backend
                           ├── JWT Auth (HS256)
                           ├── PatternAnalysisService
                           ├── MySQL / Redis  (캐시 · Rate Limit)
                           └── Gemini API ──▶ fallback 분석 텍스트 (미연동 시 자동 전환)
```

---

**성과 및 개선점**

| 구분 | 항목 | 내용 |
|:--:|:--|:--|
| ✓ | 환경 재현성 | Docker Compose로 3서비스 컨테이너화, 재현성 100% 확보 |
| ✓ | CI/CD | GitHub Actions lint + build 자동화, PR 머지 시 자동 검증 |
| ✓ | AI 안정성 | Gemini fallback 구조 — 네트워크 장애 시에도 전체 흐름 유지 |
| ✓ | 캐시 최적화 | Redis 적용으로 분석 API 반복 호출 비용 절감 |
| △ | 코드 구조 | God Function → Claude Code로 계층 분리 리팩토링 |
| △ | 테스트 커버리지 | 바이브 코딩 특성상 초기 부족 → 핵심 로직 단위 테스트 보완 필요 |
| △ | 코드 일관성 | AI 생성 코드 컨벤션 통일을 위한 문서화 필요성 인식 |

---

**Vibe Coding 인사이트**

AI가 코드를 생성해도 설계 의도와 구조적 판단은 개발자의 몫임을 체감했습니다.
프롬프트 품질이 곧 코드 품질로 이어졌고, MCP 연동으로 반복 작업(파일 수정, PR, 문서화)을 자동화하면서 개발 흐름 자체에 집중할 수 있었습니다.

</details>

---

<details>
<summary>&nbsp;<b>스마트 주차장 &nbsp;—&nbsp; 모빌리티 허브</b></summary>

<br/>

RC카와 IoT 센서를 활용한 스마트 주차 시스템.
OCR 자동 승인의 인식 한계를 빠르게 판단해 **관리자 확인 기반 반자동 구조로 전환**, 실제 동작 가능한 시스템으로 완성.

**Tech**
`Spring Boot` `JPA` `MySQL` `MQTT` `Raspberry Pi` `Python` `React`

**핵심 역할**
- 입차 승인 로직 설계 및 구현
- 라인트레이서 기반 차량 감지 처리
- 관리자 승인 → MQTT 기반 서보모터 제어 연결
- OCR 한계를 판단하고 서비스 동작 중심으로 구조 재설계

</details>

<br/>

---

## Tech Stack

**Backend**
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Framework](https://img.shields.io/badge/Spring_Framework-6DB33F?style=flat-square&logo=spring&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

**Database**
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-3C3C3C?style=flat-square)

**AI / ML**
![RAG](https://img.shields.io/badge/RAG-FF6F00?style=flat-square)
![Gemini API](https://img.shields.io/badge/Gemini_API-4285F4?style=flat-square&logo=googlegemini&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-111827?style=flat-square)
![Text Embedding](https://img.shields.io/badge/Text_Embedding-7B61FF?style=flat-square)

**Vibe Coding / AI Tools**
![Claude Code](https://img.shields.io/badge/Claude_Code-CC785C?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI Codex](https://img.shields.io/badge/OpenAI_Codex-412991?style=flat-square&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_Server-111827?style=flat-square)

**IoT**
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878A?style=flat-square&logo=arduino&logoColor=white)
![Mosquitto](https://img.shields.io/badge/Mosquitto-3C5280?style=flat-square&logo=eclipsemosquitto&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22B5BF?style=flat-square)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)
![Android](https://img.shields.io/badge/Android-34A853?style=flat-square&logo=android&logoColor=white)

**Languages**
![Java](https://img.shields.io/badge/Java-F89820?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000000)

**Infra / DevOps**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![MSA](https://img.shields.io/badge/MSA-FF6F00?style=flat-square)

**Tools**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![IntelliJ](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=000000)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![DBeaver](https://img.shields.io/badge/DBeaver-382923?style=flat-square)
![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white)

<br/>

---



<sub>heewonn09@naver.com &nbsp;·&nbsp; 010-5129-8600</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1f2937,100:0d1117&height=80&section=footer&animation=fadeIn" width="100%"/>

</div>
