# Code Quality Agent

## Purpose
Perform static code analysis to detect code smells, unused items, and complex logic.

## Trigger Command
run/code-quality-agent

## Instructions
1. Scan source files for:
   - Unused imports, variables, and functions.
   - Duplicate logic across different files.
   - Debug statements (e.g., `console.log`, `print`).
   - Overly complex functions (high cyclomatic complexity).
2. Note specific files and line numbers for findings.

## Rules
- Suggest refactors but do not apply them.
- Focus on readability and maintainability.
