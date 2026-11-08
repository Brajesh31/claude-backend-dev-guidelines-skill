# Error Tracking and Monitoring

Instrument the service so operators can detect and diagnose failures.

## Error tracking
Capture unexpected exceptions with request correlation IDs, release/version, environment, and safe context. Redact credentials, tokens, personal data, and request bodies by default.

## Metrics
Track request rate, latency percentiles, error rate, saturation, database pool health, queue depth, and dependency failures.

## Logs and traces
Use structured logs and distributed trace context across service boundaries. Avoid high-cardinality metric labels and never log secrets.

## Operations
Define alert thresholds, ownership, escalation, retention, and incident runbooks. Test alerts and recovery procedures.
