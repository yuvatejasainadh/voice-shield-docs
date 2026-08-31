# Privacy

Voice/audio data is sensitive.

## Observed behavior
- Audio files are uploaded to backend for processing.
- Backend may store a server-side audio copy path in `analysis_records`.
- Third-party providers are used for transcription and deepfake scoring.

## Policy status
Formal retention windows, deletion guarantees, and legal/privacy policy wording were not fully defined in inspected repositories. Final policy should be reviewed with legal/compliance before production launch.
