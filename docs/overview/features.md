# Features and Current Status

## Implemented
- Multi-format audio validation (`wav`, `mp3`, `m4a`, `aac`, `ogg`, `flac`, `webm`)
- FastAPI endpoints for health/readiness, analysis, history, transcription
- STT orchestrator with provider fallback order: Sarvam -> AssemblyAI -> Groq
- Optional Reality Defender deepfake risk analysis
- SQLite persistence for analysis records (backend)
- Android Room persistence for call sessions and analysis history
- Android WorkManager-based post-call recording discovery and analysis

## Partially implemented / In progress
- Web app API integration shape differs from backend response schema in some pages
- Android client defines `GET /api/v1/analysis/{id}` consumption path, backend route currently absent

## Planned / Future enhancement
- True live chunk-by-chunk call streaming loop
- Dedicated webhook callback channel for chunk result push
- Call-level temporal risk aggregation and anti-duplicate transition engine
