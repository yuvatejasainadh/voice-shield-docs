# Cloudflare and Domain Routing

Known public API domain used by app defaults:
- `voice-api.asteriontechnologies.tech`

Target architecture (documented intent):
```mermaid
flowchart TD
    I[Internet] --> CF[Cloudflare]
    CF --> D[voice-api.asteriontechnologies.tech]
    D --> T[Cloudflare Tunnel]
    T --> API[Voice Shield FastAPI backend]
```

Status: tunnel-level config files were not found in inspected repositories; treat operational details as pending verification.
