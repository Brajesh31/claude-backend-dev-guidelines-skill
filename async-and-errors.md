# Async Work and Error Handling

Use asynchronous execution for I/O-bound work when supported by the runtime. Bound concurrency and define timeouts.

## Error handling
- Distinguish expected domain failures from unexpected infrastructure failures.
- Retry only transient and safe-to-retry operations.
- Use exponential backoff with limits and jitter.
- Propagate cancellation and enforce deadlines.
- Make background jobs idempotent and observable.

Do not swallow exceptions or return success-shaped responses after partial failure. Use correlation IDs to connect logs across asynchronous work.
