# Introduction

## What is Voice Shield?
Voice Shield is an AI-assisted voice-security system designed to reduce fraud from AI-cloned voices and deepfake audio impersonation.

### Practical scenario
An attacker can synthesize a trusted person's voice and pressure a victim during a call. Voice Shield analyzes audio and returns risk signals so users can verify before acting.

## Why this project exists
- Human listeners are often unable to reliably detect high-quality synthetic speech.
- Caller ID and contact names are insufficient against social-engineering attacks.
- Risk can evolve over a call; one static check is often insufficient.

## Current implementation snapshot
- Android app supports manual audio analysis and post-call recording analysis workflow.
- Backend validates audio, runs transcription provider orchestration, and optional Reality Defender analysis.
- Web app provides project/demo pages, but parts of the API contract in UI are still placeholder.
