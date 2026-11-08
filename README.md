# claude-backend-dev-guidelines-skill

A Claude Code skill for consistent backend development with Node.js, Express, TypeScript, and modern service architecture patterns.

## Overview

This skill provides practical conventions for building and maintaining backend services. It focuses on layered architecture, route and controller design, service and repository responsibilities, validation, error handling, configuration, monitoring, and testing.

The guidance is intended for codebases using the technologies and patterns described in the skill. Adapt it to the actual project rather than applying conventions blindly.

## Main Capabilities

- Organize routes, controllers, services, and repositories.
- Implement consistent controller patterns.
- Validate inputs with Zod.
- Manage database access with Prisma.
- Handle errors and asynchronous operations.
- Configure middleware and dependency injection.
- Manage application configuration.
- Monitor performance and errors.
- Write unit and integration tests.
- Refactor legacy backend patterns.

## Architecture Layers

| Layer | Responsibility |
|---|---|
| Routes | Define endpoints and middleware order |
| Controllers | Translate HTTP requests and responses |
| Services | Implement business logic |
| Repositories | Encapsulate persistence operations |
| Middleware | Cross-cutting request behavior |
| Configuration | Centralize environment and runtime settings |

## Installation

```bash
git clone https://github.com/Brajesh31/claude-backend-dev-guidelines-skill.git ~/.claude/skills/backend-dev-guidelines
```

## Usage

Invoke the skill when creating or refactoring backend features:

```text
/backend-dev-guidelines
```

Provide the framework version, project structure, database layer, validation approach, monitoring setup, and expected behavior.

## Recommended Feature Workflow

1. Inspect existing routes and architecture.
2. Define the endpoint contract and validation schema.
3. Add or update the route.
4. Implement controller request and response handling.
5. Put business logic in a focused service.
6. Encapsulate database access in the repository layer.
7. Add consistent error handling.
8. Add logs and monitoring where appropriate.
9. Write unit and integration tests.
10. Verify behavior and compatibility.

## Reference Guide

The repository includes focused guides for:

- Architecture and project structure.
- Routing and controllers.
- Services and repositories.
- Input validation.
- Monitoring and error tracking.
- Middleware.
- Database access patterns.
- Configuration management.
- Asynchronous operations and error handling.
- Testing strategy.
- End-to-end implementation workflows.

## Quality Checklist

- Controllers remain thin.
- Business logic is not duplicated across routes.
- Input validation occurs at trust boundaries.
- Database access is predictable.
- Errors use consistent response structures.
- Async failures are handled.
- Secrets are not hard-coded.
- Logs avoid sensitive values.
- Tests cover success and failure paths.
- Configuration is validated at startup.

## Repository Contents

- `SKILL.md`: Main backend development instructions.
- `references/`: Detailed guides for architecture, implementation, and testing.
- `README.md`: Workflow and architecture overview.

## Practical Principle

A layered architecture is useful only when responsibilities are genuinely separated. Do not add unnecessary abstractions or repositories around trivial operations without a maintainability benefit.
