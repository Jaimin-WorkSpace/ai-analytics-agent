# Manager Agent (Orchestrator)

## Purpose
The single entry point for the Repository Analysis System. Orchestrates 8 specialized agents to deliver a master technical blueprint and dashboard.

## Trigger Command
run/manager [REPOSITORY_PATH]

**Examples:**
- `run/manager /Users/yashcomputers/Desktop/Projects/MyApp`
- `run/manager https://github.com/username/repo.git`
- `run/manager /path/to/any/project`

**IMPORTANT:** Always use the provided repository path from the command. Never use hardcoded paths.

## Execution Rules
1. **Intake**: 
   - If a Git URL is provided: `git clone --depth 1 [URL] /tmp/analysis_target`.
   - If a local path is provided: Set as analysis target.
2. **Data Integrity**: `rm -rf reports/*` before starting to ensure a fresh single source of truth.
3. **Pipeline**: 
   - Trigger `run/indexer` → `run/project-analyzer` → `run/dependency-auditor` → `run/security-risk-analyzer` → `run/code-quality-agent` → `run/performance-analyzer` → `run/large-file-detector` → `run/report-generator`.

## Rules
- **Deliverables**: Must produce both a technical `repository_analysis_report.md` and a premium `dashboard.html`.
- **No Side Effects**: System must only perform analysis; no code modification or refactoring is allowed.
- **Complete Autonomy**: Once triggered, no further user input should be required.
