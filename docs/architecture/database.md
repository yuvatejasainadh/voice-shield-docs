# Database Design

## Backend database (voice-shield-api)
Only one persisted table is currently defined in code:

```mermaid
erDiagram
    ANALYSIS_RECORDS {
        string id PK
        string filename
        string stored_audio_path
        string status
        string classification
        int risk_score
        float confidence
        float ai_probability
        float duration_seconds
        int segments_analyzed
        int processing_time_ms
        string detector_version
        json reasons
        datetime created_at
    }
```

## Android local database (voice-shield-app)
```mermaid
erDiagram
    CALL_SESSIONS {
        string sessionId PK
        long startTimestamp
        long endTimestamp
        int durationSeconds
        string direction
        string state
        bool processed
        string resultReportId
    }
    ANALYSIS_HISTORY {
        string id PK
        int riskScore
        string riskLevel
        string classification
        long timestamp
    }
```

## Call/chunk/result model status
- `Call` and `Analysis` exist in Android local model.
- Backend chunk-level entities are **not yet implemented**.
