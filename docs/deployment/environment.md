# Environment Variables Reference

| Variable | Repository | Purpose | Required | Example |
|---|---|---|---|---|
| DATABASE_URL | voice-shield-api | SQLAlchemy DB URL | Yes | `sqlite:///./voice_clone_detection.db` |
| MAX_UPLOAD_SIZE_MB | voice-shield-api | Upload file-size cap | Yes | `25` |
| MAX_AUDIO_DURATION_SECONDS | voice-shield-api | Duration cap | Yes | `600` |
| CORS_ORIGINS | voice-shield-api | Allowed origins | Yes | `http://localhost:3000` |
| SARVAM_API_KEY | voice-shield-api | Primary STT provider key | If used | `<sarvam-key>` |
| ASSEMBLYAI_API_KEY | voice-shield-api | Fallback STT key | If used | `<assemblyai-key>` |
| GROQ_API_KEY | voice-shield-api | Fallback STT key | If used | `<groq-key>` |
| REALITY_DEFENDER_API_KEY | voice-shield-api | Voice-risk provider key | If voice analysis enabled | `<rd-key>` |
| STORAGE_PATH | voice-shield-api | Temp/storage path | Yes | `./storage` |
| GEMINI_API_KEY | voice-shield-app/.web | Placeholder AI Studio secret usage | Optional | `<gemini-key>` |
| APP_URL | voice-shield-web | App hosted URL in AI Studio setup | Optional | `https://example.app` |

Never commit real secrets.
