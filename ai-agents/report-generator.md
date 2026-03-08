# Report Generator Agent

## Purpose
Synthesize all agent findings into a master technical blueprint and a high-data-density visual dashboard.

## Trigger Command
run/report-generator

## Output Files
- **Technical Report**: `reports/repository_analysis_report.md`
- **Visual Dashboard**: `reports/dashboard.html`

## Technical Report & Dashboard Sections
1. **EXECUTIVE SUMMARY**: Modernization Gauge (0-100 score) & Risk Scorecard.
2. **BUSINESS IMPACT & ROI**: Detailed labor savings, Architect equivalence, and Cost mitigation.
3. **TECHNICAL IMPROVEMENT BLUEPRINT**:
   - **Architecture**: Blueprint for hook-based refactoring (e.g., `useBleManager`).
   - **Modernization**: Migration path for critical packages (e.g., `Vision Camera`).
4. **DATA DEEP DIVE**:
   - **Tech Debt Heatmap**: High-complexity directory identification.
   - **Dependency Graph Analysis**: Linking risks to specific native modules.
5. **INTERACTIVE CHECKLIST**: Developer to-do list for priority-1 refactors.

## Dashboard Template (HTML/CSS)
- **Architecture**: 3-Tab View (Overview, Deep Dive, ROI).
- **Visuals**: SVG Circular Gauges for Modernization, Bar Charts for Risk Distribution.
- **Rules**: Must be fully self-contained (Single HTML file).
