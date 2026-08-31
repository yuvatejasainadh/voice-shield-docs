# FastAPI Backend Architecture

## Folder structure
```text
backend/app/
├── api/routes/
│   ├── analyze.py
│   ├── health.py
│   ├── history.py
│   ├── ready.py
│   └── transcription.py
├── audio/
├── core/
├── db/
├── ml/
├── schemas/
├── services/
├── utils/
└── main.py
```

## Responsibilities
- `api/routes`: HTTP route definitions
- `audio`: file/audio validation
- `services`: provider integrations + orchestration
- `schemas`: pydantic request/response contracts
- `db`: SQLAlchemy engine/models/session
- `core`: settings and logging

## Runtime behaviors
- CORS origins from `CORS_ORIGINS`
- startup creates DB tables and runs additive SQLite upgrade
- exception handlers normalize validation and internal errors
