# Voice Shield Documentation

Central technical documentation for **Voice Shield** (SIH 2026 Problem Statement **26104**): AI-powered detection and prevention of voice-cloning impersonation.

## Repositories
- [voice-shield-app](https://github.com/yuvatejasainadh/voice-shield-app) — Android client (Kotlin, Compose, Room, WorkManager)
- [voice-shield-api](https://github.com/yuvatejasainadh/voice-shield-api) — FastAPI backend for audio validation, STT orchestration, and voice-risk scoring
- [voice-shield-web](https://github.com/yuvatejasainadh/voice-shield-web) — Public web/demo/docs UI (React + Vite)
- [voice-shield-docs](https://github.com/yuvatejasainadh/voice-shield-docs) — This repository

## What Voice Shield does
Voice Shield helps users detect potential AI voice impersonation during voice interactions. It analyzes uploaded call/voice audio and returns a risk assessment (`LIKELY_GENUINE`, `SUSPICIOUS`, `LIKELY_AI_GENERATED`) with supporting metadata.

## Documentation Index
- Overview
  - [Introduction](docs/overview/introduction.md)
  - [Problem Statement](docs/overview/problem-statement.md)
  - [Features & Current Status](docs/overview/features.md)
  - [Roadmap](docs/overview/roadmap.md)
- Architecture
  - [System Architecture](docs/architecture/system-architecture.md)
  - [Repository Architecture](docs/architecture/repository-architecture.md)
  - [Data Flow](docs/architecture/data-flow.md)
  - [Sequence Diagrams](docs/architecture/sequence-diagrams.md)
  - [Database Design](docs/architecture/database.md)
- Backend
  - [FastAPI Architecture](docs/backend/architecture.md)
  - [API Reference](docs/backend/api.md)
  - [Audio Processing](docs/backend/audio-processing.md)
  - [Webhooks](docs/backend/webhooks.md)
  - [Backend Database](docs/backend/database.md)
- Android
  - [Architecture](docs/android/architecture.md)
  - [Real-time Analysis UX](docs/android/realtime-analysis.md)
  - [Notifications](docs/android/notifications.md)
  - [Permissions](docs/android/permissions.md)
- ML
  - [Pipeline](docs/ml/pipeline.md)
  - [Evaluation](docs/ml/evaluation.md)
  - [Limitations](docs/ml/limitations.md)
- Web
  - [Website Architecture](docs/web/architecture.md)
- Deployment
  - [Local Development](docs/deployment/local-development.md)
  - [Production](docs/deployment/production.md)
  - [Cloudflare & Domain](docs/deployment/cloudflare.md)
  - [Environment Variables](docs/deployment/environment.md)
- Security
  - [Security Architecture](docs/security/security.md)
  - [Privacy](docs/security/privacy.md)
  - [Threat Model](docs/security/threat-model.md)
- Testing
  - [Backend Testing](docs/testing/backend.md)
  - [Android Testing](docs/testing/android.md)
  - [Web Testing](docs/testing/web.md)
- Development
  - [Setup](docs/development/setup.md)
  - [Workflow](docs/development/workflow.md)
  - [Troubleshooting](docs/development/troubleshooting.md)
- Reference
  - [Glossary](docs/reference/glossary.md)
  - [FAQ](docs/reference/faq.md)

## Important implementation note
This documentation distinguishes:
- **Implemented**: Verified from current repositories
- **Planned / Future Enhancement**: Desired architecture not yet implemented in code

## Contribution
See [CONTRIBUTING.md](CONTRIBUTING.md).
