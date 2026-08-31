# API Reference (Verified from route code)

Base prefix: `/api/v1`

## GET `/health`
Purpose: liveness check.

Response:
```json
{"status":"healthy","service":"voice-clone-detection-api","version":"0.1.0"}
```

## GET `/ready`
Purpose: readiness for database and provider configuration.
- Returns `200` when database connection is ready.
- Returns `503` when not ready.

## POST `/analyze`
Purpose: combined transcription + voice risk analysis.
- Content-Type: `multipart/form-data`
- Field: `audio` file
- Query params:
  - `language` (optional)
  - `include_voice_analysis` (default `true`)

Possible statuses: `200`, `400`, `413`, `415`, `422`, `502`.

## POST `/transcription`
Purpose: transcription-only endpoint.
- Fields: `audio`
- Query params: `language`, `include_segments`

Possible statuses: `200`, `400`, `413`, `415`, `422`, `502`.

## GET `/history`
Purpose: paginated analysis history.
- Query params: `page` (>=1), `limit` (1..100)

## Not implemented in backend (but referenced in Android client)
- `GET /api/v1/analysis/{analysisId}`

## Auth
- No API auth middleware is currently implemented in route stack.
