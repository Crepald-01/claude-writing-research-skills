---
name: code-review
description: Review code changes or a file for bugs, security issues, edge cases, performance problems, and readability, and report findings ranked by severity with suggested fixes. Use when the user asks for a code review, a second opinion on a diff, or a check before merging.
---

# Code review

## Process
1. Understand intent: what the code is meant to do. If unclear, ask before judging design choices.
2. Read the change in full, including the surrounding code it touches.
3. Check each category:
   - **Correctness**: logic errors, off-by-one, null or undefined handling, wrong return values, race conditions.
   - **Security**: unvalidated input, injection (SQL, shell, HTML), secrets in code, unsafe deserialization, missing authorization checks.
   - **Edge cases**: empty input, very large input, concurrency, failure paths, timeouts.
   - **Performance**: needless loops over large data, repeated I/O inside loops, unbounded queries.
   - **Maintainability**: naming, duplication, unclear control flow, missing tests for new behaviour.
4. Check whether tests exist and cover the changed behaviour.

## Output
Findings grouped by severity:
- **Blocker**: will cause a bug, security hole, or data loss.
- **Should fix**: likely problem or significant maintainability issue.
- **Nit**: style or minor clarity.

For each finding: file and line, the problem in one sentence, and a suggested fix as a short code snippet.

End with a one-line verdict: approve, approve with changes, or request changes.

## Rules
- Cite specific lines. Do not give generic advice.
- Do not rewrite the whole file unless asked.
- Say when you could not run the code or tests, and do not claim they pass.
- Do not treat a style preference as a defect unless the project's guide requires it.
