# Data Flow

## Current implemented flow
```mermaid
sequenceDiagram
    participant Android
    participant API as FastAPI
    participant STT as STT Providers
    participant RD as Reality Defender
    participant DB as SQLite

    Android->>API: POST /api/v1/analyze (multipart audio)
    API->>API: Validate extension, size, decode, duration
    API->>STT: Transcription orchestration
    API->>RD: Voice manipulation detection (optional)
    API->>DB: Save analysis_records row (if voice analysis available)
    API-->>Android: CombinedAnalysisResponse
```

## Real-time chunk pipeline status
Chunk-based continuous call analysis with callback/webhook updates is **Planned**; current implementation is request/file based.
