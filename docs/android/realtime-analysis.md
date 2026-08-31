# Android Real-Time Detection UX

## Before call
- Requests runtime permissions (audio, phone state, notifications, media/storage).
- Initializes DB, repositories, and notification helper.

## During call
- Tracks telephony state transitions.
- Maintains local call session metadata.
- Current code does **not** stream live chunks to backend continuously.

## After call
- WorkManager searches for matching recording.
- Validates discovered audio.
- Uploads to `/api/v1/analyze`.
- Stores report and sends notification.
