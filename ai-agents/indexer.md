# Indexer Agent

## Purpose
Index all files in the repository to provide a complete list of assets for analysis.

## Trigger Command
run/indexer

## Instructions
1. Scan the `PROJECT_PATH` recursively.
2. Ignore `node_modules`, `.git`, `dist`, `build`, and other temporary folders.
3. Generate a list of all source files, configuration files, and documentation.
4. Store the list of files in a temporary memory for subsequent agents.

## Rules
- Include hidden files if they are configuration files (e.g., `.env`, `.eslintrc`).
- Provide count of total files.
