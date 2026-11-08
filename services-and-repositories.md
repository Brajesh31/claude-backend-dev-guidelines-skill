# Services and Repositories

## Services
Services coordinate use cases, enforce workflow rules, and call domain logic or adapters. Keep them independent of HTTP request/response objects. Prefer explicit dependencies and avoid giant service classes.

## Repositories
Repositories encapsulate persistence queries and mapping. Expose operations that express application needs rather than leaking ORM details everywhere.

## Transactions
Define transaction boundaries around business operations. Avoid holding database transactions open while waiting on slow external APIs. Use idempotency and an outbox or compensation strategy when a workflow spans systems.

## Testing
Unit-test service behavior with repository fakes. Integration-test repository queries against the actual database engine.
