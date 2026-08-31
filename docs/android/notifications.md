# Notification Strategy

## Implemented logic
In `CallAnalysisWorker`:
- `riskScore >= 61`: high-priority alert notification
- else: completion notification

## Anti-spam status
- Duplicate prevention for repeated recording analysis is implemented via `SettingsRepository.markRecordingProcessed()`.
- Transition-based per-chunk dedup notifications (`LOW->LOW ignore`, etc.) are **Planned**, not currently implemented end-to-end.
