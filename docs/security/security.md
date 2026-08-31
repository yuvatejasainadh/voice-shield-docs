# Security Architecture

## Implemented
- HTTPS client-server intent in app/web configuration
- Backend audio extension/size/duration/decode validation
- Server-side provider API key usage (not returned to clients)
- Structured error handling and limited response error exposure

## Not yet implemented / not found in route stack
- Request authentication/authorization for API endpoints
- Webhook signature verification endpoint
- Explicit rate limiting middleware

## Recommended hardening
- Add API auth (token/JWT/service key)
- Add rate-limit and abuse controls
- Add webhook HMAC signatures + replay protection
- Define retention/deletion policy controls
