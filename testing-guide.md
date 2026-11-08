# Backend Testing Guide

## Test layers
- Unit tests: business rules and pure functions.
- Integration tests: database, cache, queue, and external adapter behavior.
- API tests: routing, validation, auth, status codes, and response contracts.
- End-to-end tests: a small set of critical user journeys.

## Quality
Use deterministic fixtures, isolate test data, clean up resources, and avoid depending on production services. Test authorization failures, malformed input, concurrency, timeouts, and transaction rollback.

Run migrations in CI against a disposable database. Keep secrets out of test logs.
