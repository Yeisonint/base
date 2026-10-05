# Safety, security and compatibility

## Errors and input
- Handle errors following the idiomatic conventions of the language and project. Errors must be propagated, recovered from or logged correctly; never silently ignored.
- Validate input coming from users, files, network, databases, external APIs and any other untrusted source.

## Security
- Never expose secrets, passwords, tokens, private keys, credentials or sensitive information in code, logs, error messages or commits.
- Do not hardcode credentials, machine-specific paths or sensitive settings when they should be configurable.
- Apply security principles appropriate to the context: least privilege, input validation, safe error handling, injection protection, and authentication and authorization where applicable.

## Runtime
- Consider concurrency, race conditions, deadlocks, memory safety and synchronization when the language or architecture requires it.
- Properly release resources such as memory, files, sockets, connections, locks, processes, threads and devices.
- Maintain cross-platform compatibility when the project requires it. Do not assume an operating system or architecture without verifying it.
- Do not assume a tool is installed. Verify required tools and follow the project's conventions.

## Changes and dependencies
- Do not change existing APIs, contracts, protocols or data formats without identifying affected consumers and considering backward compatibility.
- Before deleting code, verify that no references, imports, dependencies, endpoints, configurations or consumers still use it.
- Do not change existing behavior unrelated to the task. If you detect an additional problem, report it instead of silently fixing it.
- Prioritize existing tools, libraries and dependencies. Do not add new dependencies if a viable native solution exists.
- Do not run destructive, irreversible or deep-cleanup commands without explicit confirmation, including deleting directories or databases, deployments, or commands with force options.
