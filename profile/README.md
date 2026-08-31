<div align="center">

<img src="../docs/assets/demo.gif" alt="EduFlow demo" width="720" />

# EduFlow

</div>

<br/>

AI를 쓰는 학생은 늘었지만, **제대로 읽고·검증하며 쓰는 법**을 배우기 어렵습니다.  
환각·편향·프롬프트 인젝션 같은 리스크는 교과서만으로는 체감되지 않고,  
교사는 출제·채점·학급 현황을 한곳에서 보기 힘듭니다.

**EduFlow**에서는 이렇게 연습합니다.

- **RAG 체험** — 학습 자료를 근거로 AI와 대화하고, 서술형 답안을 키포인트로 부분 채점
- **Hallucination 탐지** — AI 답변의 오류를 찾고 유형을 분류
- **AI 토론** — 찬반 에이전트 토론을 평가자로 검증
- **보안 실습** — 프롬프트 인젝션에 대응하는 방어 연습

<br/>

## &nbsp;&nbsp;Tech stack

| Repo | Role | Stack |
|------|------|-------|
| [`frontend`](https://github.com/eduflow-team/frontend) | 학생·교사 웹 | [![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=white&labelColor=222222)](https://react.dev/) [![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=flat-square&logo=vite&logoColor=white&labelColor=222222)](https://vite.dev/) [![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white&labelColor=222222)](https://www.typescriptlang.org/) [![React Router](https://img.shields.io/badge/React_Router-7-CA4245?style=flat-square&logo=reactrouter&logoColor=white&labelColor=222222)](https://reactrouter.com/) |
| [`backend`](https://github.com/eduflow-team/backend) | API · DB · 채점 | [![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white&labelColor=222222)](https://www.python.org/) [![FastAPI](https://img.shields.io/badge/FastAPI-0.115-009688?style=flat-square&logo=fastapi&logoColor=white&labelColor=222222)](https://fastapi.tiangolo.com/) [![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql&logoColor=white&labelColor=222222)](https://www.postgresql.org/) [![pgvector](https://img.shields.io/badge/pgvector-vector-222222?style=flat-square&labelColor=222222)](https://github.com/pgvector/pgvector) |
| [`ai`](https://github.com/eduflow-team/ai) | Langflow · 프롬프트 | [![Langflow](https://img.shields.io/badge/Langflow-1.10.0-000000?style=flat-square&labelColor=222222)](https://www.langflow.org/) [![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white&labelColor=222222)](https://www.docker.com/) |

<br/>

## &nbsp;&nbsp;Quick start

### &nbsp;&nbsp;Frontend

```bash
git clone https://github.com/eduflow-team/frontend.git
cd frontend
cp .env.example .env
npm install && npm run dev
```

### &nbsp;&nbsp;Backend

```bash
git clone https://github.com/eduflow-team/backend.git
cd backend
cp .env.example .env
docker compose up -d --build
docker compose exec backend alembic upgrade head
```

### &nbsp;&nbsp;AI

```bash
git clone https://github.com/eduflow-team/ai.git
cd ai
cp .env.example .env
docker compose up -d
```

<br/>

## &nbsp;&nbsp;Team

<div align="center">

| <a href="https://github.com/ucaeon"><img src="https://github.com/ucaeon.png" width="80" height="80" style="border-radius:50%"/><br/><b>유채원</b></a> | <a href="https://github.com/CHeeRiNG-CHiCKeN"><img src="https://github.com/CHeeRiNG-CHiCKeN.png" width="80" height="80" style="border-radius:50%"/><br/><b>손주희</b></a> | <a href="https://github.com/garden0324"><img src="https://github.com/garden0324.png" width="80" height="80" style="border-radius:50%"/><br/><b>임정원</b></a> | <a href="https://github.com/lyudongwon"><img src="https://github.com/lyudongwon.png" width="80" height="80" style="border-radius:50%"/><br/><b>류동원</b></a> |
|:---:|:---:|:---:|:---:|
| [@ucaeon](https://github.com/ucaeon) | [@CHeeRiNG-CHiCKeN](https://github.com/CHeeRiNG-CHiCKeN) | [@garden0324](https://github.com/garden0324) | [@lyudongwon](https://github.com/lyudongwon) |

</div>
