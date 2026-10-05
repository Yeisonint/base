# Testing and verification

## Tests
- Add or modify tests when a change introduces or modifies verifiable behavior.
- Tests must check real behavior, edge cases, invalid input and relevant failure conditions.
- Do not disable tests, linters, warnings, validations or security rules to make a build pass.
- Do not hide errors by suppressing warnings, exceptions or compiler messages without technical justification.

## Definition of done
- A task is done only when the project builds successfully without relevant warnings and passes the available linter, static analysis and tests.
- Verify changes in the target environment when it differs from the development environment.
- Never declare a task complete based only on the code looking correct. Distinguish between implemented, built, tested and verified in the target environment.
- If a validation cannot run due to an environment limitation, state it explicitly and do not claim the task is fully validated.

## Failure limits
- If the compiler, linter or tests fail 2 consecutive times due to your changes, stop automatic attempts, diagnose the problem and report the exact error and your hypothesis.
- If you try to fix the same bug or failure 3 consecutive times without success, stop immediately and ask for human assistance.
