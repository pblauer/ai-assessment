# AI-Augmented SDLC Assessment Workspace

This workspace is dedicated to assessing the AI Maturity of software delivery engagements based on the **AI-Augmented SDLC Framework**. It provides a standardized methodology for analyzing interview transcripts with Team Leads and Delivery Managers.

## Core Mandates for AI Agents
1. **Framework Adherence:** All assessments must strictly follow the 5-level maturity model and 15-question framework defined in `docs/AI-Augmented SDLC _Template_.md`.
2. **Evidence-Based Scoring:** Every score above 3 must be supported by "Show Me" evidence from the transcript.
3. **Sovereignty & Security:** Projects cannot exceed Level 3 if they score below 4 on Data Privacy (Q12) or Human Sovereignty (Q13).
4. **Translation Requirement:** If a transcript is provided in Spanish, a translated English version must be generated and stored in the `transcripts/` folder before assessment.
5. **Standardized Output:** All assessments must be saved to the `analysis/` folder using the naming convention below.

## File Naming Conventions
- **Transcripts:** `transcripts/[ProjectName]_Transcript_[YYYY_MM_DD].md`
- **Translations:** `transcripts/[ProjectName]_Transcript_[YYYY_MM_DD]_EN.md`
- **Assessments:** `analysis/[ProjectName]_Maturity_Assessment_[YYYY_MM_DD].md`

## Workflow Process
1. **Ingest:** Locate the newest transcript in `transcripts/`.
2. **Translate:** If the source is Spanish, generate an English version with the `_EN` suffix.
3. **Analyze:** Research the project goal (What/Why) and the 15-question evidence.
4. **Score:** Calculate averages per section (Product, Engineering, QA, Risks, Team/Tracking).
5. **Recommend:** Provide 5 prioritized recommendations with criticality levels.
6. **Save:** Write the final report to `analysis/`.
