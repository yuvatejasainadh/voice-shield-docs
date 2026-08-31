# Troubleshooting

## Backend
- **422 INVALID_AUDIO**: verify file is decodable and non-empty
- **413 FILE_TOO_LARGE / AUDIO_TOO_LONG**: reduce size or duration
- **503 not ready**: check DB and provider env configuration
- **502 provider errors**: verify provider API keys/connectivity

## Android
- Missing analysis: verify recording access URI and permissions
- No notifications: check POST_NOTIFICATIONS permission and app settings
- API unreachable: verify base URL and network access

## Web
- Demo fails: ensure API base URL points to actual backend and route prefix is correct (`/api/v1/...`)

## Deployment
- Domain reachable but API failing: verify tunnel/backend target health and readiness endpoint
