# Audio Processing and Validation

## Supported extensions
`wav`, `mp3`, `m4a`, `aac`, `ogg`, `flac`, `webm`

## Validation steps
1. Extension allow-list check
2. File existence/non-empty
3. Upload size <= `MAX_UPLOAD_SIZE_MB` (default 25 MB)
4. Decoding via `soundfile`, fallback to `PyAV`
5. Duration > 0 and <= `MAX_AUDIO_DURATION_SECONDS` (default 600s)

## Decoder metadata extracted
- sample rate
- channels
- total samples
- duration seconds

## Preprocessing
Current backend validates and may normalize unsupported provider formats to WAV before provider upload in service layer.
