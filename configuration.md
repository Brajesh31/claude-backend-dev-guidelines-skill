# Configuration Management

Load configuration from environment or a managed secret/configuration service. Validate required values at startup and fail fast with safe error messages.

## Rules
- Separate public configuration from secrets.
- Never commit credentials or production environment files.
- Use distinct settings per environment.
- Define safe defaults only for non-sensitive optional settings.
- Rotate secrets and document ownership.
- Avoid logging configuration values wholesale.

Keep configuration parsing centralized and typed where the language supports it.
