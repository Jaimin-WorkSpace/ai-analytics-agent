# Large File Detector Agent

## Purpose
Identify files containing more than 1000 lines of code to improve modularity and maintainability.

## Trigger Command
run/large-file-detector

## Instructions
1. For each file in the indexed list:
   - Count total lines of code.
   - If count > 1000, report the file name and total lines.
   - Determine the risk level (MEDIUM/HIGH) based on size.
2. Suggest a modular structure to break down large files.

## Reporting Requirements
For each large file:
- File Name:
- Total Lines:
- Risk Level:
- Suggested Modular Structure:
