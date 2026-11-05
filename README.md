# Real-Time Collaborative Code Editor

A learning-by-building project exploring Go, WebSockets, and real-time communication. Multiple users open the same document and see each other's changes live.

**Stack:** Go, React/Next.js, PostgreSQL, WebSockets, Redis, Docker

## Status

Work in progress. Currently: project setup and a running Go API.

## Roadmap

- [x] Project setup, Go API with health check
- [ ] Users and documents (basic auth, PostgreSQL)
- [ ] Editor page, saving to the database
- [ ] WebSockets: broadcast changes to connected users
- [ ] Multiple users in one document, basic presence
- [ ] Redis for shared presence/messages, reconnect handling
- [ ] Error/loading states, tests, Docker, architecture notes

## Structure

```
backend/    Go API
frontend/   React client
```

## Run the backend

```
cd backend
go run .
```

Then open http://localhost:8080/health. It should return `{"status":"ok"}`.
