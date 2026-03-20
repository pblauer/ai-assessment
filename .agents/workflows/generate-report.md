---
description: Generates or updates a project's HTML report based on its markdown assessment
---

This workflow automates the generation of a project-specific HTML report and updates the portfolio dashboard.

### Usage
`/generate-report "ProjectName"`

### Workflow Steps

1. **Read Assessment:**
    - Locate the latest markdown assessment in `analysis/` for the provided project name.
    - Example: `analysis/[ProjectName]_Maturity_Assessment_[YYYY_MM_DD].md`.

2. **Extract Data:**
    - Parse the executive summary, scores, tools, and recommendations.
    - Calculate the radar chart coordinates based on the scores.

3. **Generate HTML Report:**
    - Use the established premium HTML structure (as seen in `reports/1800F.html` and `reports/Lender.html`).
    - Create/Update `reports/[ProjectName].html` with the extracted data.

4. **Update Portfolio Header:**
    - If this is a new project, add a row to the "Maturity Comparison" table in `reports/index.html`.
    - If it's an update, ensure the stats and link are current.
    - Recalculate portfolio-wide stats (Avg. Maturity, Total Assessments).

5. **Completion:**
    - Provide a link to the generated report and the updated portfolio.
