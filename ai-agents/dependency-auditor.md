# Dependency Auditor Agent

## Purpose
Audit project dependencies for deprecations, security risks, and version mismatches.

## Trigger Command
run/dependency-auditor

## Instructions
1. Locate dependency files: `package.json`, `yarn.lock`, `Pipfile`, etc.
2. Cross-reference libraries with current unmaintained lists (e.g., `react-native-camera` -> `react-native-vision-camera`).
3. For each deprecated library, identify the exact recommended migration path.

## Reporting Requirements
For each dependency:
- Library Name:
- Current Version:
- Recommended Version:
- Risk Level: (LOW / MEDIUM / HIGH)
- **Impact of Upgrade**: Detail what improves after the upgrade (e.g., "Fixes iOS 17 layout issues", "Reduces bundle size by 50kb").
- Suggested Replacement: (if applicable)
