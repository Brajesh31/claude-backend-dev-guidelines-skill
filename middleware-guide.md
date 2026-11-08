# Middleware Guide

Middleware should implement cross-cutting transport concerns in a predictable order.

## Common middleware
- Request ID and structured access logging
- Security headers and CORS policy
- Authentication and authorization
- Rate limiting
- Body size limits and content-type checks
- Centralized error handling

## Ordering
Establish request context early, reject malformed or oversized input before expensive work, authenticate before protected handlers, and ensure error middleware can observe downstream failures.

Avoid putting business workflows or database-specific logic in middleware.
