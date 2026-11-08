# Database Patterns

## Schema and access
Use migrations under version control. Define constraints and indexes from real query patterns. Parameterize queries and use least-privilege database credentials.

## Transactions
Use transactions for invariants that must be atomic. Keep them short and avoid external network calls inside transactions. Understand isolation level and retry behavior.

## Performance
Use pagination, bounded result sets, connection pooling, and query plans. Watch for N+1 queries and unbounded scans.

## Reliability
Configure backups, restore tests, replication monitoring, and migration rollback strategy. Never treat a successful backup job as proof that recovery works.
