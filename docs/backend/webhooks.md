# Webhook Architecture

## Current state
A dedicated webhook callback endpoint for per-chunk push responses is **not implemented** in current `voice-shield-api` routes.

## What is implemented instead
- Synchronous API response model: client uploads audio and receives JSON response in the same request.

## Planned webhook model
- Chunk-level processing response callbacks
- Session/chunk identifiers for idempotent updates
- Retry and signature verification

These are architecture goals and should be treated as **Future Enhancement** until code is added.
