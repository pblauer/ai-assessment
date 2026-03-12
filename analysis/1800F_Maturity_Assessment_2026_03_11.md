# AI Maturity Assessment: 1800F

---

## 1. Project Context
- **Project Name:** 1800F 
- **Project Goal (What/Why):** The team is building a multibranding-capable React Native mobile application for the "1800 Flowers" umbrella. The project aims to provide a skinnable platform that can easily extend to other sub-brands. Technically complex with over 15 backend integrations (CMS, Firebase, Auth0, etc.).
- **AI Toolset & Agreements:** Tech Lead uses personal **ChatGPT Pro** ($200 tier). Team uses **Codex** (VS Code integration and standalone client). Client is supportive and uses Codex internally, but there is no commercial agreement for the client to cover Forte's licenses.
- **Transcript Date:** 2026-03-11

---

## 2. Executive Summary
### Summary
Project 1800F is driven by a Technical Lead, Humberto, who operates at an "Augmented" level of expertise, successfully treating AI as a high-velocity junior developer while maintaining absolute architectural sovereignty. He has established a sophisticated workflow using local MD files as context rules and a Figma-to-code pipeline. However, the team culture is currently bifurcated; while the lead is highly optimized, other members (e.g., Nico) show adoption hesitancy, keeping the collective maturity in the "Enabled" phase.

### Key Highlights
- **Maturity Level:** L2 - Enabled
- **Average Total Score:** 2.73 / 5.0
- **Adoption Lead:** Humberto Bringas (Individual Maturity: L5 - Augmented)

---

## 3. AI Team Adoption Level
| Role | Adoption Level | Description |
| :--- | :---: | :--- |
| **Team Lead** | **High** | Humberto uses ChatGPT Pro and Codex for foundation, maquetation, and architectural auditing. |
| **Team Overall** | **Partial** | Freddy (QA) uses the free version of Codex for automation; Nico (Dev) is currently hesitant with no adoption. |

---

## 4. AI Workflow & Usage Patterns
### Workflow Pattern
**AI as a Junior Developer / Maquetator**
The Tech Lead uses AI as a high-speed Junior Developer specifically for layout/maquetation work and boilerplate scaffolding. Humberto acts as the Senior Reviewer/Architect, auditing AI outputs against design links and architectural quality gates. He describes himself as "a reviewer of what the guy does."

### Categorized Usages
- **Skill Gap Compensation:** Humberto uses AI specifically to bridge gaps in React Native layout/maquetation expertise (Timestamp 00:18:29).
- **Accelerating Boilerplate:** Scaffolding all foundation elements (DTOs, Mappers, API controllers) from Figma links and descriptions.
- **Architectural Auditing:** Feeding local architectural MD files to AI agents as "Rules" to ensure generated code aligns with project standards (Timestamp 00:19:18).
- **Automation Scaffolding:** QA (Freddy) uses AI to accelerate the creation and extension of automation frameworks (Timestamp 00:22:18).

---

## 5. Scoring per Section
| Section | Average Score | Status |
| :--- | :---: | :--- |
| **Product (Discovery & Strategy)** | 2.0 | Low |
| **Engineering (Development)** | 4.0 | High |
| **QA (Validation & Quality)** | 2.0 | Low |
| **Risks (Governance & Ethics)** | 3.5 | Med |
| **Team & Tracking (Knowledge)** | 2.0 | Low |

---

## 6. Scoring Breakdown (The 15 Questions) - Score: 1: Lowest - 5 Highest
| Phase | Question | Score | Evidence / Rationale |
| :--- | :--- | :---: | :--- |
| **Product** | 1. Requirements Expansion | 3 | AI used for initial roadmap/stories from Figma, but manual refinement by Nelson (PO) is still required. |
| | 2. Edge Case Analysis | 2 | Used ad-hoc to "force definitions" rather than a systematic grooming phase. |
| | 3. Backlog Prioritization | 1 | No evidence of AI-assisted prioritization frameworks. |
| **Engineering** | 4. Tool Integration | 4 | Humberto uses Codex/VS Code integration; Freddy uses Codex; Nico is currently "hesitant" and non-using. |
| | 5. Boilerplate & Scaffolding | 5 | Primary method for foundation, shared components, and Figma-to-code (Timestamp 00:16:30). |
| | 6. Code Review Quality | 3 | Human-AI "ping-pong" occurs for review, but no automated first-pass agents. |
| | 7. Refactoring & Tech Debt | 4 | Actively used for refactor patterns based on documented architectural patterns in local MD files. |
| **QA** | 8. Test Case Design | 2 | Primary focus is on script generation; scenario design remains largely manual. |
| | 9. Automation Acceleration | 4 | Freddy is explicitly using Codex to extend the automation framework (Timestamp 00:22:18). |
| | 10. Defect Clarity | 1 | No evidence of AI-augmented bug reporting. |
| | 11. Synthetic Data Gen | 1 | No evidence of synthetic data usage. |
| **Risks** | 12. Data Privacy & Security | 2 | Use of personal accounts and "caution" rather than formal security protocols. (Capped at L3) |
| | 13. Human Sovereignty | 5 | Strict policy: "I am a reviewer of what the guy does." 100% human oversight. |
| **Team/Tracking**| 14. Prompt Library Usage | 2 | Uses MD files for context, but lacks a shared, versioned team prompt library. |
| | 15. Impact Tracking | 2 | Subjective reporting ("10x time saved") without formal V×E×Q tracking. |

---

## 7. Strengths
- **Individual Augmented Capacity:** Lead (Humberto) uses AI for high-speed scaffolding and architectural auditing.
- **Figma-to-Code Pipeline:** Seamless generation of React Native components directly from Figma links using the Codex standalone client.
- **Context-Aware Architecture Rules:** Use of local `.md` files as a "rules engine" for AI agents (Timestamp 00:19:18).
- **Strong Human Sovereignty:** A culture of "Verify, Don't Just Trust," where all AI output is peer-reviewed.

---

## 8. Path to Next Level (Moving to L3 - Integrated)
To reach the next maturity level, the team must achieve the following:
a. **Governance & Tool Alignment:** Transition from personal Pro accounts to enterprise-sanctioned licenses (Copilot/ChatGPT Enterprise) and establish formal data-privacy protocols (Score 12 must reach 4+).
b. **Institutionalize Knowledge:** Formalize the architectural context currently in MD files into a **Shared Prompt Library** and establish a standard onboarding path for new devs (e.g., Nico).
c. **Expand QA Lifecycle:** Train the QA team to use AI for generating **Test Scenarios** (negative, boundary analysis) from stories, moving beyond script-only automation.

---

## 9. Prioritized Recommendations (Top 10)
1. **Secure Enterprise Governance** - Criticality: **Critical**. Move from personal Pro accounts to enterprise licenses to eliminate security risks (Q12).
2. **Standardize the Prompt Library** - Criticality: **High**. Convert architectural MD files into shared team patterns (Q14).
3. **Augment QA Scenario Design** - Criticality: **High**. Train Freddy to use AI for boundary and negative test scenario generation (Q8).
4. **Institutionalize Discovery Refinement** - Criticality: **Med**. Introduce Persona-based prompts for the PO to extract Edge Cases and NFRs (Q2).
5. **Onboard Laggards** - Criticality: **Med**. Pair Nico with an AI Champion to overcome adoption hesitancy and tool-access friction (Q4).
6. **Establish Multiplier Metrics** - Criticality: **Low/Opportunity**. Implement tracking for time saved to quantify ROI for the client (Q15).
7. **Automate Quality Gates** - Criticality: **Low**. Use AI-assisted PR checklists to perform a "first pass" on security and style (Q6).
8. **Synthetic Data Strategy** - Criticality: **Low**. Explore AI for generating realistic, anonymized test data for complex e-commerce flows (Q11).
9. **Backlog Prioritization Frameworks** - Criticality: **Low**. Use AI-assisted RICE scoring to justify backlog ranking (Q3).
10. **Defect Clarity Enhancement** - Criticality: **Low**. Use AI to augment bug reports with reproduction steps and root-cause suggestions (Q10).

---

## 10. The "Show Me" Protocol (Evidence)
- **Artifact/Demo 1:** Codex Integration (00:16:30) - Humberto demonstrated the Codex client chatting with Figma links to generate React Native components.
- **Artifact/Demo 2:** Architectural Context Files (00:19:18) - Showed documentation in `.md` files that act as "Quality Gates," fed to AI to ensure alignment with project standards.
- **Artifact/Demo 3:** QA Automation Extension (00:22:18) - Evidence of Freddy using Codex to extend the automation framework.
