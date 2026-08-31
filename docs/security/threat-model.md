# Threat Model

| Threat | Impact | Current Mitigation | Recommended Mitigation |
|---|---|---|---|
| AI voice cloning | Fraud/impersonation | Provider-based risk analysis | Ensemble + call context verification |
| Replay audio attacks | False trust decisions | None explicit | Replay-detection features |
| Malicious audio uploads | Service abuse/crashes | Format/size/decode validation | Rate limits, malware scanning, queue isolation |
| API abuse / DoS | Availability loss | Basic validation only | Auth + throttling + WAF rules |
| Webhook spoofing | Fake risk events | Not implemented | Signed webhook payloads |
| Backend compromise | Data exposure | Env var secrets | Secret manager, least privilege, audit logs |
| Model extraction/probing | Evasion risk | None explicit | Query limits, monitoring, adversarial testing |
