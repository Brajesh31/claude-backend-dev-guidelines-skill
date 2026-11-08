# Input Validation Patterns

Validate all untrusted input at system boundaries.

## Rules
- Validate type, length, format, range, and allowed values.
- Reject unknown fields where the API contract requires strict schemas.
- Normalize only when normalization is part of the documented contract.
- Validate identifiers and ownership before reading or mutating resources.
- Keep business invariants in the domain/application layer, not only in request schemas.

Return field-level errors without leaking secrets or internal implementation details. Never rely on client-side validation as a security control.
