# Backend Architecture Overview

Organize the backend around clear responsibilities and business capabilities.

## Typical request flow
HTTP route -> authentication/authorization -> validation -> controller/handler -> application service/use case -> repository or external adapter -> response mapping.

## Boundaries
- Routes define transport paths and middleware.
- Controllers translate HTTP input/output and should remain thin.
- Services implement application workflows and business orchestration.
- Repositories isolate persistence operations.
- Domain modules own business invariants.
- Configuration and infrastructure wiring belong at startup/composition boundaries.

Avoid circular dependencies and direct database access from route handlers. Document module ownership, data ownership, and external dependencies.
