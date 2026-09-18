# System Architecture

```text
JavaFX UI
   |
ChatController
   |--------------------|
   v                    v
AIService           ChatRepository
   |                    |
OpenAI-compatible      SQLite
REST API
```

## Non-functional requirements
- Performance: avoid blocking the JavaFX UI with unnecessary work.
- Security: API keys are read from environment variables and are not stored in source code.
- Usability: simple chat interface with model selector and history.
- Reliability: validation and exception handling prevent common failures.
- Maintainability: MVC-style separation and service/repository abstractions.
- Resource efficiency: SQLite provides lightweight local persistence.
