# Domain-specific considerations

- **Web applications:** consider input validation, authentication, authorization, sessions, CORS, CSRF, XSS, injection, secret management and exposure of sensitive information where applicable.
- **Desktop applications:** consider error states, empty states, loading, user interaction, basic accessibility and behavior on failure.
- **Network applications:** consider timeouts, reconnection, connection loss, invalid responses, concurrency and resource limits.
- **Systems with persistence:** consider transactions, consistency, migrations, concurrency, integrity and error recovery.
- **Embedded or low-level code:** consider memory limits, execution timing, concurrency, interrupts, hardware access and behavior on failure.
