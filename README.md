# Spring Boot + AI 4-Week Learning Workbook

This repository is a workbook for a fast, practical 4-week learning track from Java/Spring Boot fundamentals into a minimal Spring Boot + AI project.

## Goals
- Learn Java + Spring Boot basics
- Build an API with CRUD flow
- Connect a backend to an AI service
- Add a minimal RAG flow with embeddings/vector retrieval
- Track progress in a structured, verifiable way

## Repository structure
- `docs/learning-plan.md` — weekly plan and daily checklist
- `src/main/java/...` — Spring Boot skeleton
- `src/test/java/...` — smoke tests
- `docker-compose.yml` — optional local container setup
- `.env.example` — environment variables

## Quick start

```bash
cp .env.example .env
source .env
mvn spring-boot:run
```

Health check:

```bash
curl http://localhost:8080/api/health
```

Chat example:

```bash
curl -X POST http://localhost:8080/api/chat \
  -H "Content-Type: application/json" \
  -d '{"message":"请给我一个管线拓扑检查建议"}'
```

## 4-week plan
See `docs/learning-plan.md`.

## Notes
- Keep secrets in environment variables.
- Use AI as a coding assistant, not as a blind replacement for understanding.
- Focus on testing, validation, and production-oriented engineering.
