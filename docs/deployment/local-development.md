# Local Development Setup

## Backend (`voice-shield-api/backend`)
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
python run.py
# or: uvicorn app.main:app --reload
```

## Android (`voice-shield-app`)
- Open in Android Studio
- JDK 11 (source/target compatibility in Gradle)
- Sync Gradle and run app module

## Web (`voice-shield-web`)
```bash
npm install
npm run dev
npm run build
npm run lint
```
(Equivalent package-manager commands can be used if your environment uses Bun.)
