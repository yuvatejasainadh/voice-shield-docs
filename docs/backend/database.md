# Backend Database

- Engine: SQLAlchemy
- Default URL: `sqlite:///./voice_clone_detection.db`
- Table created at startup from model metadata
- Additive SQLite migration helper: `upgrade_sqlite_schema()`

Main model: `AnalysisRecord` (`backend/app/db/models.py`).
