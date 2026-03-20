---
description: Run an AI SDLC Maturity Assessment from a transcript file
---

This workflow automates the AI-Augmented SDLC Maturity Assessment process for a specific client and transcript.

### Usage
`/ai-sdlc-assessment "ProjectName" "path/to/script.srt"`

### Workflow Steps

1. **Ingest & Normalize:**
    - Move/Copy the source transcript from the provided path to `transcripts/`.
    - Rename it to `transcripts/[ProjectName]_Transcript_[YYYY_MM_DD].md` (convert to .md if it is .srt).
    - Use the current date for `[YYYY_MM_DD]`.

2. **Translation (If needed):**
    - Check if the transcript is in Spanish.
    - If it is, generate an English version with the `_EN` suffix at `transcripts/[ProjectName]_Transcript_[YYYY_MM_DD]_EN.md`.

3. **Analysis & Research:**
    - Adhere strictly to the **GEMINI.md** core mandates.
    - Use `docs/AI-Augmented SDLC _Template_.md` for the 15-question framework.
    - Infer the project goal (What/Why) from the transcript and any attached context. If the goal is unclear, explicitly mark it as assumed or unknown.
    - Focus on finding "Show Me" evidence for any score above 3.

4. **Scoring:**
    - Assign scores (1-5) for each of the 15 questions across the 5 phases:
        - Product (Q1-3)
        - Engineering (Q4-7)
        - QA (Q8-11)
        - Risks (Q12-13)
        - Team / Tracking (Q14-15)
    - Calculate averages per section.
    - Determine maturity level (L1-L5) based on the total average.
    - Ensure L4/L5 is only assigned if Q12 and Q13 are at 4 or 5.

5. **Recommendations:**
    - Provide 5-10 prioritized recommendations with criticality levels.
    - Identify the two lowest-scoring questions and turn them into actionable sprint goals.

6. **Final Report:**
    - Generate the final assessment report following the template in `docs/AI-Maturity-Assessment-Instruction.md`.
    - Save the report to `analysis/[ProjectName]_Maturity_Assessment_[YYYY_MM_DD].md`.
    - Present a summary of the assessment and a link to the final file. Summary should include Overall Maturity and any missing points, details or unkowns detected in the transcript. Recommend follow up questions to complete any incomplete section. 