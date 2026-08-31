# ML / Detection Pipeline

## Production pipeline in current backend
Current backend uses external providers, not an in-repo local inference model:
- STT orchestration: Sarvam -> AssemblyAI -> Groq
- Voice manipulation detection: Reality Defender

Risk mapping in backend service:
- `LIKELY_GENUINE`
- `SUSPICIOUS`
- `LIKELY_AI_GENERATED`

## WavLM in project context
WavLM appears in benchmark research artifacts under `backend/benchmark_results`, not as the active production inference path in current backend routes.
