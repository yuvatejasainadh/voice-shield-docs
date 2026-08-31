# Repository Architecture

## voice-shield-app
- Kotlin + Jetpack Compose
- Room DB (`analysis_history`, `call_sessions`)
- WorkManager `CallAnalysisWorker` for post-call processing
- Telephony hooks via `TelephonyCallback` and `BroadcastReceiver`
- Retrofit API client for backend (`/api/v1/*`)

## voice-shield-api
- FastAPI app (`backend/app/main.py`)
- Route modules: `analyze.py`, `transcription.py`, `history.py`, `health.py`, `ready.py`
- Audio validator (`app/audio/validator.py`)
- Services: transcription orchestration and Reality Defender integration
- SQLAlchemy + SQLite persistence

## voice-shield-web
- React 19 + Vite + TypeScript
- Public pages for home/demo/download/docs/security
- Config-driven links in `src/config/project.ts` (contains placeholders in current code)

## voice-shield-docs
- Source-of-truth technical docs for architecture, API, security, deployment, and contribution workflow
