# ML Evaluation (Research vs Production)

## Research artifacts found
`voice-shield-api/backend/benchmark_results` includes:
- dataset audit reports (including ~1000 genuine / 1000 spoof balanced set mention)
- WavLM diagnostic report
- sliding-window experiment report
- model comparison summaries

## Important interpretation
- Small-sample benchmark files (e.g., 20-sample experiments) are exploratory.
- Do **not** interpret those as production guarantees.
- Current production API path relies on external provider outputs.
