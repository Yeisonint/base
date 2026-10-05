# Code quality and design

## Principles
- Apply **KISS (Keep It Simple, Stupid)**: use the simplest solution that correctly solves the problem.
- Apply **YAGNI (You Aren't Gonna Need It)**: do not implement features, extensibility or infrastructure that are not currently needed.
- Apply **SOLID** when appropriate, favoring clear responsibilities, low coupling, high cohesion and extensibility without over-architecture.
- Apply **Clean Code** principles: prioritize readability, cohesion, maintainability and testability.
- Avoid significant duplication (**DRY**), but do not create artificial abstractions just to remove small coincidences.
- Do not apply KISS, SOLID, DRY, Clean Code or design patterns dogmatically if they increase complexity.
- Avoid over-engineering. Do not introduce patterns, abstractions, layers or additional frameworks without technical justification.
- Prefer explicit, easy-to-understand code over clever, overly compact or complex solutions.

## Structure
- Keep a clear separation between presentation, business logic, persistence, infrastructure and configuration when the architecture requires it.
- Every function, class and module must have a clear responsibility.
- Keep functions cohesive. Split functions when their size or complexity makes them hard to understand, test or maintain.
- Avoid functions with too many parameters, unexpected side effects or multiple responsibilities.
- Prefer composition over inheritance when it reduces coupling and complexity.
- Design interfaces based on the real needs of their consumers. Avoid overly large or generic interfaces.
- Avoid global state and shared mutability when they can cause coupling or concurrency problems.
- Prefer deterministic, easily testable solutions when possible.

## Code
- Use strict, explicit typing. Avoid `any`, `void*` and other evasive generic types unless justified.
- Use descriptive and consistent names for variables, functions, classes and modules.
- Do not leave commented-out code, temporary files, `TODO`s, dead code, unused imports or debugging leftovers.

## Performance
- Avoid unnecessarily expensive operations and consider time complexity, memory, I/O and scalability when relevant.
- Do not optimize prematurely. Prioritize correctness, clarity and maintainability; optimize when there is a demonstrable need.
