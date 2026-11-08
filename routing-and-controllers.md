# Routing and Controllers

Keep routing declarative and controllers focused on HTTP concerns.

## Guidelines
- Group routes by resource or business capability.
- Apply authentication and authorization at the correct boundary.
- Validate path, query, and body inputs before invoking business logic.
- Use consistent status codes and response envelopes.
- Keep controllers thin; delegate workflows to services.
- Define versioning and deprecation policy for public APIs.

Never trust client-supplied identity or authorization claims without verifying them. Avoid exposing internal stack traces or database errors.
