# What is it?

The document outlines a structured framework for implementing an AI-Augmented Software Development Lifecycle (SDLC) across an organization. Its purpose is to provide a practical, execution-ready template for introducing AI into Discovery, Development, and Validation workflows in a governed, measurable, and scalable way. Rather than serving as a technical “how-to,” it defines the business case, personas, governance model, prompt library strategy, training approach, pilot rollout plan, metrics framework (including the AI Multiplier: Velocity × Efficiency × Quality), risk mitigation, and phased implementation roadmap. The document is designed to guide leadership and delivery teams through institutionalizing AI adoption—moving from ad-hoc experimentation to standardized, policy-driven, ROI-measured AI-enabled delivery

# AI Augmented Delivery: Service

# AI-Augmented SDLC

Companies are under increasing pressure to deliver more, faster (often with the same or smaller teams) while maintaining quality and client trust. Traditional delivery models are reaching their limits. AI-augmented development is the next major productivity shift since Agile. Organizations that deliberately embed AI into their software delivery lifecycle reduce cycle time, catch quality issues earlier, and free skilled teams to focus on higher-value work creating a durable competitive advantage rather than isolated efficiency gains

## The Challenge

Current state across the organization:

* Practitioners spend 50–85% of time on repetitive, low-value tasks (boilerplate code, manual test creation, documentation)  
* AI usage is ad-hoc and ungoverned, creating consistency issues and security risk  
* No standardized approach to AI integration across teams  
* Client policies on AI usage vary widely with no systematic guidance  
* Competitors are institutionalizing AI-enabled delivery, creating market pressure

## The Solution

Implement a structured AI-Augmented SDLC program that transforms practitioners’ workflows while maintaining governance and client trust. The approach focuses on three personas:

* Discovery (Product Owners, Business Analysts) – Requirements refinement, backlog prioritization, stakeholder communication  
* Development (Engineers) – Code generation, code review, unit testing, documentation  
* Validation (QA Engineers) – Test case design, test automation, defect documentation, test data generation

By completing this exercise, the organization will achieve:

* Structured Enablement: Practitioners clearly understand where to access AI training, role-specific prompt libraries, and ongoing support resources.  
* Curated Prompt Libraries: Approved, client-safe prompts organized by persona (e.g., Discovery, Development, Validation) and aligned to SDLC phases.  
* Governed AI Usage: Clear, enforceable policies defining what can and cannot be shared with AI tools, with client-specific guardrails where required.  
* Intentional Adoption: AI is used purposefully within client engagements as part of day-to-day delivery, not limited to ad-hoc or side experimentation.  
* Defined Ownership: Explicit roles and responsibilities established for prompt curation, usage monitoring, governance, and continuous enablement

## SDLC Opportunities/ROI

| Phase | Activity | Current State (No AI) | Desired State (With AI) | Time Saved | Key Benefits |
| ----- | ----- | ----- | ----- | ----- | ----- |
| **Discovery** | **Requirements Gathering** | Manually draft user stories from stakeholder conversations. Often miss edge cases or have unclear acceptance criteria.  *Time: 2-3 hrs/feature* | AI expands notes into structured stories with comprehensive acceptance criteria, automatically suggesting edge cases and error handling. *Time: 45-60 min/feature* | **50-60%** | More thorough coverage, standardized format, faster stakeholder iteration |
|   | **Backlog Prioritization** | Manually score items across dimensions (value, risk, effort, dependencies) using spreadsheets or intuition. *Time: 1-2 hrs/20 items* | AI applies prioritization framework (RICE, weighted scoring) and provides ranked recommendations with justification. *Time: 20-30 min/20 items* | **60-75%** | Consistent methodology, transparent reasoning, easy re-scoring |
|   | **Stakeholder Communication** | Manually summarize sprint progress, compile release notes, draft status updates for executives. *Time: 30-45 min/update* | AI generates tailored summaries and release notes based on sprint data and stakeholder profile (technical level, priorities). *Time: 10-15 min/update* | **65-70%** | Consistent formatting, appropriate detail for audience, more time for strategic thinking |
| **Development** | **Boilerplate Code Generation** | Manually write repetitive code (API endpoints, models, DTOs, mappers) by copying from similar files and modifying. *Time: 45-90 min/CRUD endpoint* | AI generates complete boilerplate (controller, service, repository, DTOs, mappers) from schema definition, following team conventions. *Time: 15-20 min/CRUD endpoint* | **70-80%** | Consistent patterns, fewer typo bugs, engineers focus on complex business logic |
|   | **Code Review** | Manually review each PR line-by-line for bugs, security issues, performance problems, and style violations. *Time: 20-40 min/medium PR* | AI performs initial scan for common issues (null checks, error handling, security, performance), human focuses on business logic. *Time: 10-15 min/medium PR* | **50-60%** | More thorough edge case coverage, faster turnaround, better design feedback |
|   | **Unit Test Creation** | Manually write unit tests, thinking through edge cases, mocking dependencies, setting up test data. *Time: 30-60 min/function* | AI generates comprehensive test suite covering happy path, boundaries, errors, and edge scenarios with appropriate mocks. *Time: 10-15 min/function* | **70-75%** | Higher coverage, more edge cases, consistent with team patterns |
|   | **Technical Documentation** | Manually write inline comments, API docs, and README files, often postponing or skipping. *Time: 30-45 min/component* | AI generates inline comments, README, API docs with examples, and ADRs following team templates from code. *Time: 10-15 min/component* | **65-70%** | Documentation stays current, faster onboarding, improved knowledge transfer |
| **Validation** | **Test Case Design** | Manually derive test cases from acceptance criteria, brainstorming positive, negative, and boundary scenarios.   *Time: 2-3 hrs/feature* | AI generates detailed test cases with preconditions, steps, expected results, test data covering all scenario types. *Time: 45-60 min/feature* | **60-70%** | More thorough coverage, consistent format, QA focuses on exploratory testing |
|   | **Test Automation Scripts** | Manually write Selenium/Playwright/Cypress scripts, identifying locators, handling waits, debugging flaky tests. *Time: 45-90 min/test scenario* | AI generates automation script with robust locators, appropriate waits, error handling, and parameterized data. *Time: 15-25 min/test scenario* | **65-75%** | Faster automation coverage, consistent patterns, QA focuses on complex orchestration |
|   | **Defect Documentation** | Manually document defects with reproduction steps, environment details, screenshots, and severity assessment. *Time: 15-25 min/defect* | AI generates structured defect report with clear steps, environment details, severity justification, potential root causes. *Time: 5-10 min/defect* | **60-65%** | Faster developer triage, fewer questions, consistent defect quality |
|   | **Test Data Generation** | Manually create test data (users, products, transactions) using spreadsheets, SQL scripts, or repetitive UI actions. *Time: 1-2 hrs/dataset* | AI generates realistic test data including edge cases, boundary values, and varied realistic patterns from schema. *Time: 15-30 min/dataset* | **75-85%** | More realistic data, better edge case coverage, easy regeneration |

# Project Personas

# AI-Augmented SDLC: Program Roles & Responsibilities

## AI Program Lead (Technical Program Owner) 

A senior leader responsible for overall program ownership, strategic alignment, and cross-functional coordination. This person drives the initiative from vision to implementation and reports progress to executive leadership.

Responsibilities:

* Overall program ownership and accountability for success metrics  
* Facilitate governance working group meetings and decision-making  
* Manage program budget, resource allocation, and timeline  
* Executive reporting on adoption rates, ROI, and strategic outcomes  
* Remove organizational blockers and escalate critical issues  
* Coordinate with Product, Engineering, QA leadership for alignment

## Executive Sponsor

 A C-level or VP-level executive who provides strategic direction, secures funding, and champions the initiative across the organization. This person ensures the program has necessary resources and organizational priority.

Responsibilities:

* Approve program funding and resource commitments  
* Provide air cover for organizational change and adoption challenges  
* Communicate strategic importance to leadership team and practitioners  
* Make final decisions on policy conflicts or major governance issues  
* Celebrate wins and reinforce culture of AI adoption

## Governance & Oversight

Cross-functional leaders from Product, Engineering, QA, Legal/Compliance, and Security who define policies, approve prompts (initially), and ensure responsible AI usage. This group balances innovation with risk management.

Responsibilities:

* Define and maintain AI usage policy (what can/cannot be shared)  
* Review and approve prompts for initial library (first 1-2 months)  
* Resolve escalations and ambiguous situations  
* Quarterly policy refresh based on evolving needs and tools  
* Monitor compliance incidents and recommend corrective actions  
* Approve client-specific AI guidance and exceptions

## Security & Compliance Lead 

A security or compliance professional who ensures AI usage meets data protection, privacy, and regulatory requirements. This person provides oversight on data handling, tool security, and client confidentiality.

Responsibilities:

* Review AI tools for security posture and data handling practices  
* Define data classification guidelines for AI usage  
* Assess compliance with client contracts and regulatory requirements (HIPAA, GDPR, etc.)  
* Investigate and remediate any security or privacy incidents  
* Provide guidance on client-specific compliance constraints  
* Approve prompts that involve sensitive operations or data

## Discipline-Specific Roles

### Discovery Lead/Group (Product/BA Discipline Owner) 

A senior Product Owner or Business Analyst who validates and curates Discovery-specific prompts. This person ensures prompts align with product management best practices and deliver value for requirements, prioritization, and stakeholder communication.

Responsibilities:

* Review and validate Discovery persona prompts (requirements, backlog prioritization, stakeholder communication)  
* Contribute prompts based on real product management scenarios  
* Test prompts with product teams and gather feedback  
* Ensure prompts follow team conventions and methodologies  
* Provide domain expertise for governance decisions on Discovery use cases  
* Mentor other Product Owners/BAs on effective AI usage

### Development Lead/Group (Engineering Discipline Owner) 

A senior engineer who validates and curates Development-specific prompts. This person ensures prompts produce high-quality code that follows team standards and architectural patterns.

Responsibilities:

* Review and validate Development persona prompts (code generation, code review, unit testing, documentation)  
* Test prompts against real codebase and architecture patterns  
* Ensure generated code meets team standards (style, security, performance)  
* Identify gaps in prompt library for common engineering tasks  
* Provide technical expertise for governance decisions on Development use cases  
* Mentor other engineers on prompt engineering and AI pair programming

### Validation Group/Group (QA Discipline Owner) 

A senior QA Engineer who validates and curates Validation-specific prompts. This person ensures prompts produce comprehensive test coverage and align with quality engineering best practices.perona, na

Responsibilities:

* Review and validate Validation persona prompts (test case design, test automation, defect documentation, test data)  
* Test prompts against real features and acceptance criteria  
* Ensure generated test cases meet coverage and quality standards  
* Identify opportunities for AI in exploratory testing and quality analysis  
* Provide domain expertise for governance decisions on Validation use cases  
* Mentor other QA engineers on AI-augmented testing techniques

## Client Delivery & Adoption

### Delivery Managers (Client-facing Oversight) 

Delivery Managers or Engagement Leads responsible for ensuring AI usage complies with client policies and drives results on active engagements. These people bridge organizational AI capabilities with client-specific constraints.

Responsibilities:

* Document client-specific AI policies and constraints in central repository  
* Ensure practitioners on their engagements follow client AI guidance  
* Communicate AI capabilities and governance to client stakeholders  
* Monitor AI usage and outcomes on client projects (velocity, quality impact)  
* Escalate client concerns or policy violations to governance team  
* Identify opportunities to showcase AI-enabled delivery to clients

### Product Owners / Business Analysts (Discovery Persona) 

Practitioners who use AI to accelerate requirements gathering, backlog prioritization, and stakeholder communication. These are the primary beneficiaries of Discovery-focused prompts.

Responsibilities:

* Adopt AI for user story refinement, acceptance criteria generation, backlog prioritization  
* Contribute prompts based on real project needs  
* Provide feedback on prompt effectiveness and gaps  
* Follow AI usage policy and client-specific guidance  
* Report time saved and quality improvements

### Engineers (Development Persona) 

Practitioners who use AI to accelerate code generation, code review, unit testing, and documentation. These are the primary beneficiaries of Development-focused prompts.

Responsibilities:

* Adopt AI for boilerplate code generation, code review, unit testing, documentation  
* Maintain human oversight \- review all AI outputs before committing  
* Contribute prompts based on real coding scenarios  
* Follow team standards and architectural patterns when using AI  
* Report time saved and quality improvements

### QA Engineers (Validation Persona)

 Practitioners who use AI to accelerate test case design, test automation, defect documentation, and test data generation. These are the primary beneficiaries of Validation-focused prompts.

Responsibilities:

* Adopt AI for test case generation, automation scripts, defect documentation, test data  
* Maintain critical thinking \- AI augments, does not replace, exploratory testing  
* Contribute prompts based on real testing scenarios  
* Follow quality standards and ensure comprehensive coverage  
* Report time saved and quality improvements

# High Level Approach

# Approach

## 1\. Establish Ownership & Governance (Foundation)

Goal: Ensure AI usage is intentional, consistent, and safe from the start.

Key Activities:

* Appoint an AI Program Lead with end-to-end accountability for the initiative  
* Assign discipline-specific AI Leads:  
  * Development Lead (engineers)  
  * Discovery Lead (Product Owners, Business Analysts)  
  * Validation Lead (QA Engineers)  
* Document AI usage policy defining what can and cannot be shared with AI tools  
* Specify tasks that require mandatory human review (e.g., final approval of requirements, production deployments, client communications)  
* Create escalation paths for ambiguous situations (practitioner → AI Lead → Governance Working Group)

## 2\. Define AI-Augmented Ways of Working (Target State)

Goal: Specify exactly how and when AI should be used in each role's daily work.

Key Activities:

* Document 3-5 high-value AI use cases per persona:  
  * Developers: Boilerplate code generation, unit test creation, code review checklists, inline documentation  
  * Discovery: User story drafting, acceptance criteria refinement, backlog prioritization, stakeholder summaries  
  * Validation: Test case generation, automation script creation, defect documentation, test data generation  
* Map AI touchpoints to SDLC phases showing when AI should be used (e.g., "Use AI to generate test cases from acceptance criteria after story refinement")  
* Provide concrete examples of quality AI outputs (e.g., "A good AI-generated user story includes...")  
* List explicit exclusions (e.g., "Do not use AI for: client-specific business logic, PII-containing code, architectural decisions")

## 3\. Create a Shared Prompt & Pattern Library

Goal: Provide practitioners with proven, reusable prompts to reduce variation and accelerate adoption.

Key Activities:

* Build 30-50 initial prompts organized by persona and SDLC phase:  
  * Development: Code generation, refactoring guidance, test scaffolding  
  * Discovery: Story templates, NFR extraction, competitive analysis  
  * Validation: Test scenario expansion, edge case identification, defect reproduction  
* Structure each prompt with:  
  * Input requirements (what information the practitioner must provide)  
  * Output format (what the AI should generate)  
  * Validation checklist (how to verify the AI output is correct)  
* Store prompts in an accessible, searchable repository (e.g., Confluence, GitHub, dedicated tool)  
* Establish a quarterly review process to update prompts based on usage feedback

## 4\. Training & Enablement (Practical, Not Theoretical)

Goal: Equip practitioners with hands-on skills to use AI effectively in their specific roles.

Key Activities:

* Deliver 3-hour persona-specific training sessions with:  
  * Real project examples (not generic AI demos)  
  * Hands-on practice with the prompt library  
  * Live troubleshooting of common issues  
* Cover essential skills:  
  * Writing effective prompts (context, constraints, examples)  
  * Validating AI outputs (sanity checks, edge case testing)  
  * Recognizing AI failure modes (hallucinations, outdated information, security vulnerabilities)  
* Share annotated examples showing effective vs. ineffective AI usage from actual projects  
* Avoid broad "Introduction to AI" sessions; focus exclusively on job-relevant scenario

## 5\. Onboarding & Day-1 Experience

Goal: Integrate AI guidance into standard onboarding so new team members adopt best practices immediately.

Key Activities:

* Create persona-specific onboarding checklists that include:  
  * Links to approved AI tools and how to access them  
  * The prompt library relevant to their role  
  * AI usage policy summary and examples  
  * Contact information for their discipline's AI Lead  
* Embed AI guidance directly into:  
  * New hire onboarding materials  
  * Project kickoff templates (include "AI Usage Plan" section)  
  * SDLC phase checklists (e.g., "Before code review: run AI-assisted checklist")  
* Assign new practitioners a peer mentor (AI Champion) who models good AI usage

## 6\. Pilot, Learn, and Refine (Controlled Rollout)

Goal: Validate the AI-augmented approach with a small group before organization-wide rollout.

Key Activities:

* Select 1-2 pilot teams (30 practitioners total, 10 per persona) based on:  
  * Volunteer interest  
  * Representative client environments  
  * Bandwidth to provide feedback  
* Require pilot teams to use the AI-augmented approach for all applicable work over 6-8 weeks  
* Collect structured feedback weekly:  
  * Which prompts saved the most time?  
  * Where did AI outputs require significant rework?  
  * What barriers prevented adoption (tools, policies, skills)?  
* Refine prompt library, training materials, and policies based on pilot learnings before scaling

## 7\. Metrics, Feedback, and Continuous Improvement

Goal: Measure impact and use data to drive ongoing improvements.

Key Activities:

* Establish baseline measurements before pilot begins:  
  * Average story cycle time  
  * Defect escape rate  
  * Code review duration  
  * Test coverage percentage  
* Track persona-specific metrics during and after pilot:  
  * Efficiency: Self-reported time saved per week, stories completed per sprint  
  * Quality: Defects per story, rework rate, test coverage trends  
  * Adoption: Weekly active users, prompts used per practitioner  
* Conduct monthly retrospectives to review metrics and identify improvement opportunities  
* Iterate on prompts, policies, and training based on feedback and results

## 8\. Scale & Institutionalize

Goal: Transition from pilot program to standard operating procedure across the organization.

Key Activities:

* Roll out the refined AI-augmented approach to all 500 practitioners in cohorts over 6 months  
* Embed AI practices into permanent team processes:  
  * Update SDLC templates to reference prompt library at each phase  
  * Add AI usage policy to code review and testing checklists  
  * Include AI metrics in standard project health dashboards  
* Transition governance from centralized oversight to distributed ownership:  
  * AI Leads approve new prompts for their discipline  
  * Governance Working Group meets quarterly (not weekly)  
  * AI Champions handle day-to-day practitioner support  
* Establish annual review of AI tools, prompts, and policies to incorporate new capabilities and address evolving needs  
  

# Epics \+ Stories (template)

# Dcxza	AI-Augmented SDLC Program \- User Story Backlog

This backlog contains all user stories for implementing the AI-Augmented SDLC program internally. Stories are organized by epic area and prioritized for iterative delivery across three waves (Foundation, Scale, Optimize). 

Epic Summary

| Epic 1: Governance & Policy | 8 stories \- AI usage policies, working groups, compliance |
| :---- | :---- |
| Epic 2: Tooling & Infrastructure | 6 stories \- Tool selection, licenses, platforms, tracking |
| Epic 3: Prompt Library \- Discovery | 10 stories \- Requirements, backlog, stakeholder communication |
| Epic 4: Prompt Library \- Development | 18 stories \- Code gen, review, testing, documentation |
| Epic 5: Prompt Library \- Validation | 14 stories \- Test design, automation, defects, test data |
| Epic 6: Client-Specific Guidance | 12 stories \- Client policies, engagement workflows, templates |
| Epic 7: Training & Enablement | 12 stories \- Curriculum, delivery, champions, onboarding |
| Epic 8: Metrics, Adoption & Continuous Improvement | 12 stories \- KPIs, dashboards, ROI, feedback loops |

## Epic 1: Governance & Policy (8 Stories)

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| GOV-001 | MUST HAVE | Wave 1 | As an AI Program Lead, I want to form a Governance Working Group with representatives from Product, Engineering, QA, Legal, and Security so that we have cross-functional oversight of AI usage policies |
| GOV-002 | MUST HAVE | Wave 1 | As a Governance Working Group member, I want to define what types of data can and cannot be shared with AI tools so that practitioners have clear guidelines on protecting client confidentiality |
| GOV-003 | MUST HAVE | Wave 1 | As a Security & Compliance Lead, I want to document AI tool security requirements (data encryption, access controls, audit logging) so that we only approve tools that meet our security standards |
| GOV-004 | MUST HAVE | Wave 1 | As a Governance Working Group, I want to create an AI Usage Policy document that defines approved use cases, prohibited activities, and escalation paths so that all practitioners have a reference for responsible AI usage |
| GOV-005 | SHOULD HAVE | Wave 1 | As a Governance Working Group, I want to establish a prompt approval process (submission, review criteria, approval workflow) so that we maintain quality and safety standards in our prompt library |
| GOV-006 | SHOULD HAVE | Wave 2 | As a Governance Working Group, I want to define a process for handling AI-related incidents (data leaks, policy violations, client complaints) so that we can respond quickly and improve our policies |
| GOV-007 | SHOULD HAVE | Wave 2 | As an AI Program Lead, I want to transition prompt approval from centralized governance to decentralized AI Champions for green-tagged prompts so that we can scale more efficiently |
| GOV-008 | NICE TO HAVE | Wave 3 | As a Governance Working Group, I want to conduct quarterly policy reviews based on new tools, client feedback, and industry trends so that our governance stays current and relevant |

## Epic 2: Tooling & Infrastructure (6 Stories)

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| TOOL-001 | MUST HAVE | Wave 1 | As an AI Program Lead, I want to evaluate AI tool options (GitHub Copilot, Cursor, ChatGPT Team) against criteria (cost, security, usage tracking, client acceptance) so that we select the best enterprise licenses |
| TOOL-002 | MUST HAVE | Wave 1 | As an AI Program Lead, I want to select and procure 1-2 enterprise AI tool licenses for internal/non-client work so that practitioners have approved tools to use |
| TOOL-003 | MUST HAVE | Wave 1 | As an AI Program Lead, I want to select a platform for prompt library management (Confluence, GitHub, dedicated tool) so that prompts are organized, searchable, and accessible to all practitioners |
| TOOL-004 | SHOULD HAVE | Wave 1 | As a Data Analyst/Metrics Lead, I want to set up a usage tracking dashboard (weekly active users, prompts used, time saved) so that we can monitor adoption and measure impact |
| TOOL-005 | SHOULD HAVE | Wave 2 | As an AI Program Lead, I want to document approved client-provided AI tools and how to use them so that practitioners can leverage client tools when available |
| TOOL-006 | NICE TO HAVE | Wave 2 | As an AI Program Lead, I want to integrate usage analytics from approved AI tools (API integrations, telemetry) so that we have automated tracking rather than relying on surveys |

## Epic 3: Prompt Library \- Discovery Persona (10 Stories)

*Focus: Requirements, Planning, Backlog Management, Stakeholder Communication*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| DISC-001 | MUST HAVE | Wave 1 | As a Discovery Lead, I want to create prompts for user story generation from rough requirements so that Product Owners can quickly draft well-structured stories |
| DISC-002 | MUST HAVE | Wave 1 | As a Discovery Lead, I want to create prompts for acceptance criteria refinement so that vague criteria can be expanded into testable Given/When/Then statements |
| DISC-003 | MUST HAVE | Wave 1 | As a Discovery Lead, I want to create prompts for backlog prioritization (RICE scoring, weighted frameworks) so that Product Owners can systematically rank items |
| DISC-004 | SHOULD HAVE | Wave 1 | As a Discovery Lead, I want to create prompts for stakeholder communication (sprint summaries, release notes) so that Product Owners can draft consistent status updates quickly |
| DISC-005 | SHOULD HAVE | Wave 2 | As a Discovery Lead, I want to create prompts for requirement clarification and edge case identification so that ambiguous requirements can be systematically explored |
| DISC-006 | SHOULD HAVE | Wave 2 | As a Discovery Lead, I want to create prompts for stakeholder interview guide generation so that Product Owners can prepare comprehensive discovery sessions |
| DISC-007 | SHOULD HAVE | Wave 2 | As a Discovery Lead, I want to create prompts for NFR (non-functional requirements) definition so that Product Owners can identify performance, security, and scalability needs |
| DISC-008 | NICE TO HAVE | Wave 2 | As a Discovery Lead, I want to create prompts for feature comparison matrices so that Product Owners can analyze competitive features systematically |
| DISC-009 | NICE TO HAVE | Wave 3 | As a Discovery Lead, I want to create advanced prompts for competitive analysis synthesis so that Product Owners can leverage AI for market research |
| DISC-010 | NICE TO HAVE | Wave 3 | As a Discovery Lead, I want to create advanced prompts for product roadmap scenario planning so that Product Owners can explore different strategic paths |

## Epic 4: Prompt Library \- Development Persona (18 Stories)

*Focus: Code Generation, Review, Testing, Documentation, Refactoring*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| DEV-001 | MUST HAVE | Wave 1 | As a Development Lead, I want to create prompts for boilerplate code generation (API endpoints, models, DTOs) so that engineers can quickly scaffold standard patterns |
| DEV-002 | MUST HAVE | Wave 1 | As a Development Lead, I want to create prompts for unit test generation so that engineers can create comprehensive test coverage faster |
| DEV-003 | MUST HAVE | Wave 1 | As a Development Lead, I want to create prompts for code review checklists so that engineers can systematically review PRs for common issues |
| DEV-004 | MUST HAVE | Wave 1 | As a Development Lead, I want to create prompts for inline code documentation so that engineers can generate clear comments and docstrings |
| DEV-005 | MUST HAVE | Wave 1 | As a Development Lead, I want to create prompts for README generation so that engineers can document components and services consistently |
| DEV-006 | SHOULD HAVE | Wave 1 | As a Development Lead, I want to create prompts for API design suggestions so that engineers can identify RESTful patterns and best practices |
| DEV-007 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for refactoring suggestions so that engineers can identify code smells and improvement opportunities |
| DEV-008 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for error handling pattern generation so that engineers can implement consistent exception management |
| DEV-009 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for SQL query optimization so that engineers can improve database performance |
| DEV-010 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for security vulnerability scanning guidance so that engineers can identify OWASP Top 10 issues |
| DEV-011 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for integration test generation so that engineers can create E2E test scenarios |
| DEV-012 | SHOULD HAVE | Wave 2 | As a Development Lead, I want to create prompts for mock data generation so that engineers can create realistic test fixtures |
| DEV-013 | NICE TO HAVE | Wave 2 | As a Development Lead, I want to create prompts for architectural decision record (ADR) generation so that engineers can document design decisions |
| DEV-014 | NICE TO HAVE | Wave 3 | As a Development Lead, I want to create prompts for PR description generation so that engineers can summarize changes comprehensively |
| DEV-015 | NICE TO HAVE | Wave 3 | As a Development Lead, I want to create prompts for performance profiling suggestions so that engineers can identify bottlenecks |
| DEV-016 | NICE TO HAVE | Wave 3 | As a Development Lead, I want to create prompts for migration path generation so that engineers can plan refactoring strategies |
| DEV-017 | NICE TO HAVE | Wave 3 | As a Development Lead, I want to create prompts for legacy code modernization so that engineers can update outdated patterns |
| DEV-018 | NICE TO HAVE | Wave 3 | As a Development Lead, I want to create prompts for accessibility audit guidance so that engineers can identify WCAG compliance issues |

## Epic 5: Prompt Library \- Validation Persona (14 Stories)

*Focus: Test Design, Automation, Defects, Test Data, Exploratory Testing*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| VAL-001 | MUST HAVE | Wave 1 | As a Validation Lead, I want to create prompts for test case generation from acceptance criteria so that QA can create comprehensive test scenarios |
| VAL-002 | MUST HAVE | Wave 1 | As a Validation Lead, I want to create prompts for test automation script generation (Selenium, Playwright, Cypress) so that QA can automate tests faster |
| VAL-003 | MUST HAVE | Wave 1 | As a Validation Lead, I want to create prompts for defect reproduction steps documentation so that QA can write clear bug reports |
| VAL-004 | MUST HAVE | Wave 1 | As a Validation Lead, I want to create prompts for test data generation so that QA can create realistic test fixtures |
| VAL-005 | SHOULD HAVE | Wave 1 | As a Validation Lead, I want to create prompts for exploratory testing scenario generation so that QA can plan unscripted testing sessions |
| VAL-006 | SHOULD HAVE | Wave 1 | As a Validation Lead, I want to create prompts for regression test prioritization so that QA can identify high-risk areas |
| VAL-007 | SHOULD HAVE | Wave 2 | As a Validation Lead, I want to create prompts for API test generation (Postman, REST Assured) so that QA can validate backend services |
| VAL-008 | SHOULD HAVE | Wave 2 | As a Validation Lead, I want to create prompts for test strategy documentation so that QA can define comprehensive test approaches |
| VAL-009 | SHOULD HAVE | Wave 2 | As a Validation Lead, I want to create prompts for boundary value analysis so that QA can identify edge cases systematically |
| VAL-010 | SHOULD HAVE | Wave 2 | As a Validation Lead, I want to create prompts for test coverage gap analysis so that QA can identify untested areas |
| VAL-011 | NICE TO HAVE | Wave 2 | As a Validation Lead, I want to create prompts for performance test scenario generation so that QA can design load tests |
| VAL-012 | NICE TO HAVE | Wave 3 | As a Validation Lead, I want to create prompts for test oracle generation so that QA can define expected outcomes for complex scenarios |
| VAL-013 | NICE TO HAVE | Wave 3 | As a Validation Lead, I want to create prompts for flaky test diagnosis so that QA can identify root causes of unstable tests |
| VAL-014 | NICE TO HAVE | Wave 3 | As a Validation Lead, I want to create prompts for visual regression test analysis so that QA can identify UI changes |

## Epic 6: Client-Specific Guidance (12 Stories)

*Focus: Client Policies, Engagement Workflows, Delivery Manager Support*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| CLIENT-001 | MUST HAVE | Wave 2 | As a Delivery Manager, I want a template for documenting client AI policies so that I can capture client constraints consistently |
| CLIENT-002 | MUST HAVE | Wave 2 | As a Delivery Manager, I want to document the top 10-15 client AI policies so that practitioners know which tools and prompts are allowed on each engagement |
| CLIENT-003 | MUST HAVE | Wave 2 | As a Delivery Manager, I want to create client-specific prompt libraries for sensitive industries (healthcare, financial) so that practitioners have pre-approved prompts for HIPAA/PCI environments |
| CLIENT-004 | MUST HAVE | Wave 2 | As a practitioner, I want a workflow for determining a new client's AI policy so that I know what's allowed before starting work |
| CLIENT-005 | SHOULD HAVE | Wave 2 | As a Delivery Manager, I want to tag prompts with client safety ratings (green/yellow/red per client) so that practitioners can quickly identify which prompts are approved |
| CLIENT-006 | SHOULD HAVE | Wave 2 | As a practitioner, I want a decision tree for escalating ambiguous AI usage questions so that I know when to ask my Delivery Manager vs. Governance team |
| CLIENT-007 | SHOULD HAVE | Wave 2 | As a Delivery Manager, I want to track AI usage by client engagement so that I can report adoption and value to clients |
| CLIENT-008 | SHOULD HAVE | Wave 2 | As a Sales/Delivery Lead, I want talking points for positioning AI capabilities with clients so that I can address security and compliance concerns |
| CLIENT-009 | NICE TO HAVE | Wave 3 | As a Delivery Manager, I want to create case studies showing AI-enabled delivery outcomes so that I can demonstrate value to current and prospective clients |
| CLIENT-010 | NICE TO HAVE | Wave 3 | As a Delivery Manager, I want a process for requesting client-specific AI tool approval so that we can use new tools when clients provide them |
| CLIENT-011 | NICE TO HAVE | Wave 3 | As a practitioner, I want examples of how to present AI-generated work to clients transparently so that I maintain trust and comply with client expectations |
| CLIENT-012 | NICE TO HAVE | Wave 3 | As a Delivery Manager, I want quarterly reviews of client AI policies to identify policy changes so that our guidance stays current |

## Epic 7: Training & Enablement (12 Stories) \- Not Needed Internally

*Focus: Curriculum, Delivery, Champions Network, Onboarding*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| TRAIN-001 | MUST HAVE | Wave 1 | As a Training Lead, I want to design a 4-module training curriculum (AI Fundamentals, Prompt Engineering, Role-Based Workshop, Governance) so that practitioners get comprehensive enablement |
| TRAIN-002 | MUST HAVE | Wave 1 | As a Training Lead, I want to create slide decks and hands-on exercises for each training module so that sessions are engaging and practical |
| TRAIN-003 | MUST HAVE | Wave 1 | As a Training Lead, I want to deliver training to a pilot cohort of 30 practitioners so that we can validate and refine the curriculum |
| TRAIN-004 | MUST HAVE | Wave 2 | As a Training Lead, I want to scale training delivery to 300+ practitioners in cohorts of 50 so that we achieve broad adoption |
| TRAIN-005 | MUST HAVE | Wave 2 | As an AI Program Lead, I want to recruit and train 15-20 AI Champions so that we have peer advocates supporting adoption |
| TRAIN-006 | SHOULD HAVE | Wave 1 | As a Training Lead, I want to create recorded training sessions for async viewing so that practitioners can learn at their own pace |
| TRAIN-007 | SHOULD HAVE | Wave 2 | As an AI Champion, I want office hours templates and facilitation guides so that I can effectively support my peers |
| TRAIN-008 | SHOULD HAVE | Wave 2 | As a Training Lead, I want to integrate AI training into new hire onboarding so that all new practitioners are enabled from day one |
| TRAIN-009 | SHOULD HAVE | Wave 2 | As an AI Champion, I want a prompt contribution guide so that I can help practitioners submit high-quality prompts |
| TRAIN-010 | NICE TO HAVE | Wave 2 | As a Training Lead, I want to create advanced training modules for complex use cases so that experienced practitioners can deepen their skills |
| TRAIN-011 | NICE TO HAVE | Wave 3 | As an AI Program Lead, I want to establish a rotation process for AI Champions so that we refresh the network annually |
| TRAIN-012 | NICE TO HAVE | Wave 3 | As a Training Lead, I want to measure training effectiveness (NPS, knowledge retention, usage correlation) so that we can continuously improve |

## Epic 8: Metrics, Adoption & Continuous Improvement (12 Stories)

*Focus: KPIs, Dashboards, ROI Analysis, Feedback Loops, Program Optimization*

| Story ID | Priority | Wave | User Story |
| ----- | :---: | :---: | ----- |
| METRICS-001 | MUST HAVE | Wave 1 | As a Data Analyst, I want to define adoption metrics (weekly active users, prompts used, training completion) so that we can track program uptake |
| METRICS-002 | MUST HAVE | Wave 1 | As a Data Analyst, I want to create a weekly usage tracking survey for the pilot cohort so that we can collect self-reported time savings |
| METRICS-003 | MUST HAVE | Wave 2 | As a Data Analyst, I want to measure velocity impact (story throughput for high-AI vs low-AI teams) so that we can quantify delivery improvements |
| METRICS-004 | MUST HAVE | Wave 2 | As a Data Analyst, I want to measure quality impact (defect rates, code review time, test coverage) so that we can demonstrate quality improvements |
| METRICS-005 | MUST HAVE | Wave 2 | As an AI Program Lead, I want monthly adoption reports (trends, success stories, barriers) so that I can report progress to leadership |
| METRICS-006 | SHOULD HAVE | Wave 2 | As a Data Analyst, I want to track prompt library health (total prompts, usage frequency, contribution rate) so that we can identify gaps and retire low-value prompts |
| METRICS-007 | SHOULD HAVE | Wave 2 | As an AI Program Lead, I want to calculate quarterly ROI (time saved × hourly rate) so that I can demonstrate program value |
| METRICS-008 | SHOULD HAVE | Wave 3 | As a Data Analyst, I want to create an executive dashboard showing adoption, velocity, quality, and ROI so that leadership has visibility |
| METRICS-009 | SHOULD HAVE | Wave 3 | As an AI Program Lead, I want to conduct quarterly practitioner surveys (satisfaction, barriers, suggestions) so that we gather continuous feedback |
| METRICS-010 | NICE TO HAVE | Wave 3 | As an AI Program Lead, I want to benchmark our AI adoption against industry peers so that we understand our competitive position |
| METRICS-011 | NICE TO HAVE | Wave 3 | As an AI Program Lead, I want to track governance incidents and policy violations so that we can identify and address compliance gaps |
| METRICS-012 | NICE TO HAVE | Wave 3 | As an AI Program Lead, I want to establish an annual AI strategy refresh process so that we continuously evaluate new tools and use cases |

# Potential Risks

# Risk Severity Definitions

Critical Impact: Program failure or major financial loss  |  High Impact: Significant delay or substantial cost  |  Medium Impact: Minor disruption or moderate cost

High Probability: \>50%  |  Medium Probability: 25-50%  |  Low Probability: \<25%

| ID | Category | Risk Description | Probability | Impact | Mitigation Strategy | Owner |
| :---: | :---: | ----- | :---: | :---: | ----- | :---: |
| T-01 | Technical | AI tool performance degradation or service outages causing work stoppage for practitioners across multiple client engagements | Medium | High | Multi-vendor strategy: Select 2 providers (GitHub Copilot \+ ChatGPT). Require 99.5% SLA in contracts. Maintain offline prompt library. Weekly tool health monitoring. | AI Program Lead |
| T-02 | Technical | AI-generated code contains security vulnerabilities (SQL injection, XSS, authentication bypass) that pass through code review undetected | Medium | Critical | Mandatory security scanning (SonarQube, Snyk) on all AI code before commit. Security-focused code review checklist. Quarterly penetration testing. AI prohibited from generating authentication/authorization code. | Security Lead |
| T-03 | Technical | AI tools incompatible with client technology stacks including legacy systems, air-gapped environments, or specific programming languages | High | Medium | Technology compatibility audit during client onboarding. Maintain offline-accessible prompt library. Train practitioners on manual prompt engineering. Set realistic 60% adoption targets (not 100%). | AI Program Lead |
| T-04 | Technical | Tool vendor changes pricing model mid-contract or discontinues product, forcing migration to alternative platform | Low | High | Negotiate 2-year price lock contracts with early renewal clauses. Evaluate 2 alternative vendors during selection phase with documented alternatives. Budget 10% contingency for tool migration. Maintain vendor-agnostic prompt library. | AI Program Lead |
| T-05 | Technical | AI tools leak proprietary code or client intellectual property through training data collection or logging mechanisms | Low | Critical | Enterprise contracts with zero data retention clauses. Tools must not use inputs for model training. Quarterly vendor audits for compliance. Deploy on-premises options where available. Document data handling in all client contracts. | Security Lead |
| T-06 | Technical | Prompt library becomes outdated as AI tools, programming frameworks, and best practices evolve, rendering prompts ineffective | Medium | Medium | Assign Prompt Librarian 0.1 FTE for ongoing maintenance. Quarterly prompt review cycles. Usage analytics identify low-performing prompts for retirement. AI Champions contribute updated prompts monthly. Version control tracks prompt evolution. | Prompt Librarian |
| P-01 | People | Low practitioner adoption despite training \- practitioners ignore AI tools and continue using manual methods for software delivery tasks | High | Critical | Make AI usage mandatory for new projects (not optional). Leadership communicates expectation in all-hands meetings. Track adoption by practitioner in performance reviews. AI Champions provide 1:1 coaching to laggards. Monthly adoption leaderboards with public recognition. | Exec Sponsor |
| P-02 | People | Practitioners over-rely on AI outputs, blindly accepting generated code/tests/documentation without proper validation and review | Medium | High | Training emphasizes AI limitations and hallucination risks. Mandatory human review policy for all AI outputs before production use. Code review checklist includes 'Validated AI-generated code' checkbox. Quarterly quality audits. Defect attribution tracking (AI vs. human). | QA Leadership |
| P-03 | People | Key program resources (AI Program Lead, Training Leads, AI Champions) leave organization mid-program due to turnover or reassignment | Medium | High | Document all processes, decisions, and learnings in shared repository (not tribal knowledge). Cross-train backup for AI Program Lead identified in Month 1\. Rotate AI Champions annually (prevents single points of failure). Tie program success to compensation/bonuses for retention. | AI Program Lead |
| P-04 | People | Practitioners fear AI will eliminate their jobs, leading to passive resistance, active sabotage, or voluntary turnover | Medium | Medium | Leadership messaging: 'AI augments work, does not replace people.' Frame AI adoption as career development opportunity. Show AI eliminates boring work, not jobs. Public commitment: No layoffs due to AI adoption. Highlight redeployment to higher-value strategic work. | Exec Sponsor |
| P-05 | People | Training completion but no workflow behavior change \- practitioners attend training sessions but continue working manually without integrating AI | High | Medium | Post-training assignments: Submit 3 AI-generated artifacts within first 2 weeks. Training Leads follow up individually with non-users. Integrate AI prompts directly into project templates (forces exposure). Share weekly success stories showing time saved. Make AI usage visible in sprint demos. | Training Leads |
| P-06 | People | Skill gaps widen between practitioners \- top performers adopt AI rapidly while average performers struggle, creating productivity and morale divide | Medium | Medium | AI Champions provide weekly office hours and 1:1 coaching for struggling practitioners. Celebrate learning progress (not just results) in communications. Create beginner-friendly prompts with detailed step-by-step instructions. Pair experienced AI users with novices on projects. Track monthly office hours attendance. | AI Champions |
| P-07 | People | Generational divide emerges \- senior practitioners resist AI adoption while junior practitioners over-rely on it without building fundamentals | Medium | Medium | Training emphasizes AI as tool that enhances (not replaces) human expertise. Recruit senior practitioners as AI Champions to leverage their credibility. Pair junior/senior practitioners on AI-assisted work. Publicly highlight senior practitioners' AI successes. Validate that AI assists but doesn't replace domain knowledge. | Training Leads |
| PR-01 | Process | Client explicitly prohibits AI tool usage on engagement due to security policies, competitive concerns, or regulatory constraints | High | High | Build client-specific AI policies during sales/onboarding process. Create offline prompt library for restricted environments. Negotiate AI usage allowance in statements of work. Document common client objections and develop counterpoints. Train Delivery Managers on positioning AI governance framework. | Delivery Mgrs |
| PR-02 | Process | Governance Working Group becomes decision bottleneck, creating delays in prompt approval and policy questions that slow practitioner adoption | Medium | Medium | Decentralize approval authority by Month 3: AI Champions approve green-tagged prompts without governance review. Governance only reviews yellow/red-tagged prompts. Set 5-business-day SLA for all approvals. Delegate tactical operational decisions to AI Program Lead. | Governance Group |
| PR-03 | Process | Prompt library grows excessively large (500+ prompts), becoming unsearchable and overwhelming for practitioners attempting to find relevant prompts | Medium | Medium | Implement comprehensive tagging system (persona, SDLC phase, domain, complexity level). Build search functionality with multi-select filters. Retire bottom 20% of prompts quarterly based on usage analytics. Create featured prompts section highlighting top 10 per persona. Maintain library cap of 150 active prompts. | Prompt Librarian |
| PR-04 | Process | Metrics collection remains manual and burdensome, leading to incomplete data and inability to accurately demonstrate program ROI to leadership | Medium | High | Automate metrics collection: Tool usage data via API integrations. Practitioner surveys sent automatically via workflow. Velocity metrics pulled from Jira/project management tools. Monthly dashboard auto-generated and distributed. Budget additional funding for analytics tooling if needed. Assign Data Analyst 0.2 FTE to metrics. | Data Analyst |
| PR-05 | Process | Practitioner inadvertently shares client PII, proprietary business logic, or confidential code with AI tools, violating usage policy and client contracts | Medium | Critical | Training curriculum includes real violation examples and specific consequences. Weekly governance policy reminders in practitioner newsletter. Prompt library examples use only anonymized/generic content. Quarterly audits of practitioner AI usage logs. Immediate incident response playbook with legal review process. | Security Lead |

 

# Next Steps

# Next Steps \- Program Kickoff

## 2-Week Assessment/Kickoff example

### Week 1: Team Formation & Setup

Leadership & Governance

* Identify and appoint AI Program Lead  
* Confirm Executive Sponsor  
* Form Governance Working Group (Product Lead, Engineering Lead, QA Lead, Legal/Compliance, Security Lead)  
* Schedule first governance meeting for Week 2

Discipline Leads

* Identify Discovery Lead (senior Product Owner or Business Analyst)  
* Identify Development Lead (senior engineer)  
* Identify Validation Lead (senior QA engineer)  
* Confirm each lead's time commitment and responsibilities

Training Team

* Identify 2-3 Training Leads  
* Confirm training resource availability  
* Assign backup for each critical role

Infrastructure Setup

* Select prompt library platform (Confluence, GitHub, dedicated tool)  
* Set up prompt library structure (organize by persona and SDLC phase)  
* Create shared repository for program documentation  
* Set up communication channels (Slack channel, email distribution list)

Communications (if appropriate)

* Executive Sponsor announces program launch to organization  
* AI Program Lead sends welcome email to governance team  
* Create program kickoff slide deck

### Week 2: Tool Selection & Policy Foundation

Governance Kickoff

* Conduct first Governance Working Group meeting  
* Review program charter and objectives  
* Establish weekly meeting cadence  
* Assign governance members to key workstreams (policy, prompts, client guidance)

Tool Evaluation & Selection

* Evaluate AI tools  
* Create Tool Catalogue  
* Select 1-2 tools for enterprise deployment  
* Initiate procurement process with selected vendors

Policy & Governance Framework

* Draft AI Usage Policy outline (what can/cannot be shared with AI tools)  
* Define prompt approval workflow (submission, review, approval, publication)  
* Establish safety tagging system (Green/Yellow/Red for prompts)  
* Create escalation path for ambiguous situations  
* Define incident response process for policy violations

Pilot Preparation

* Define pilot cohort selection criteria (volunteers, diverse client environments, bandwidth)  
* Target 30 practitioners (10 per persona: Discovery, Development, Validation)  
* Begin recruiting pilot participants  
* Schedule pilot kickoff for Month 3

Metrics & Tracking Setup

* Define baseline metrics to track (story cycle time, defect rates, code review duration, test coverage)  
* Set up usage tracking dashboard structure  
* Create weekly pilot feedback survey template  
* Establish success criteria for Wave 1 Phase Gate

Content Development Planning

* Training Leads begin curriculum design (4-module structure)  
* Discipline Leads identify first 10-15 prompts to create per persona  
* Assign prompt creation tasks to discipline leads  
* Set target: 30-50 prompts ready by end of Month 2

### Key Deliverables (End of Week 2\)

* Core team identified and committed (AI Program Lead, Exec Sponsor, 3 Discipline Leads, 2-3 Training Leads)  
* Governance Working Group operational with weekly meeting schedule  
* 1-2 AI tools selected and procurement initiated  
* Prompt library platform set up and accessible  
* AI Usage Policy outline drafted  
* Pilot cohort recruitment underway (target: 30 practitioners)  
* Baseline metrics identified and tracking framework established  
* Prompt creation and curriculum design work initiated

## Forte Specific Next Steps

| Category | Action | Primary Owner | Purpose / Outcome |
| ----- | ----- | ----- | ----- |
| **Ownership & Leadership** | Confirm Technical Program Owner (TPO) | Executive Sponsor | Single point of accountability for roadmap, outcomes, and tradeoffs |
|  | Form Governance Group (Product, Eng, QA, Security) | TPO | Own AI guardrails, policy decisions, and escalations |
|  | Assign AI PDLC Governor (if separate from TPO) | Executive Sponsor | Ensure consistency of AI-augmented delivery across all PDLC phases |
|  | Assign Prompt Owner(s) by discipline (Discover / Build / Validate) | TPO \+ Discipline Leads | Own prompt structure, quality, and evolution |
| **Guardrails & Standards** | Define initial AI usage policy | Governance Group | Clarify what data and use cases are allowed internally and with clients |
|  | Define prompt standards & structure | Prompt Owners | Ensure consistent, high-quality AI outputs |
|  | Define human decision gates | Governance Group | Make clear where humans retain final authority |
| **Tools & Enablement** | Identify initial AI toolset | TPO \+ Governance | Establish approved tools for early rollout |
|  | Confirm system of record (e.g., ADO / GitHub) | TPO | Centralize prompts, artifacts, and auditability |
|  | Enable access & security controls | Security Lead | Ensure safe and compliant AI usage |
| **Execution & Tracking** | Set program tracking cadence (weekly / bi-weekly) | TPO | Maintain momentum and surface blockers early |
|  | Agree on metrics & review cadence | TPO \+ Governance | Measure delivery impact, not just activity |
|  | Define MVP success criteria | TPO \+ Discipline Leads | Establish what “good” looks like for the pilot |
| Team Readiness | Provide role-specific baseline guidance | Discipline Leads | Enable teams to use AI effectively from day one |
|  | Define onboarding path for new members | TPO \+ Discipline Leads | Ensure scalability and consistency |
|  | Communicate expectations for AI usage | Delivery Leadership | Position AI as part of delivery, not optional |
| **Pilot Launch** | Select pilot project | TPO \+ Delivery Managers | Test AI-augmented delivery on real work |
|  | Confirm pilot participants | Delivery Managers | Ensure named Product, Dev, QA, Ops involvement |
|  | Establish baseline metrics | TPO/Delivery Manager | Enable before/after measurement |
|  | Launch MVP with feedback loop | TPO \+ Discipline Leads | Capture learnings and refine standards |

# Measuring Impact (example)

# How would clients know that things are changing

## AI Multiplier Framework: V × E × Q

Program ROI is measured via the AI Multiplier Framework (V × E × Q), which captures the compound effect of velocity gains, efficiency improvements, and quality enhancements ensuring AI adoption delivers measurable business value across all critical dimensions

| Dimension | Definition | Key Metrics |
| :---: | ----- | ----- |
| Velocity (V) | Delivery speed improvements | Story throughput, sprint velocity, release frequency |
| Efficiency (E) | Task-level productivity gains | Time saved per task, manual effort reduction |
| Quality (Q) | Deliverable excellence | Defect escape rate, test coverage, rework hours |

Multiplier Effect: 20% improvement in each dimension \= 1.2 × 1.2 × 1.2 \= 1.73x total impact (not additive)

## Observable changes

| PDLC Area | Before (Traditional Delivery) | After (AI-Augmented Delivery) | Business Value / Impact | Sample Metrics (How to Measure) |
| ----- | ----- | ----- | ----- | ----- |
| Discovery & Requirements | Requirements inconsistent; edge cases discovered late; frequent clarifications | AI-assisted refinement produces clearer, testable stories with risks surfaced early | Less rework, stronger alignment, better predictability | • % of stories needing clarification mid-sprint • Rework rate due to unclear requirements • Time from idea → sprint-ready |
| Backlog Readiness | Stories enter sprints partially defined | AI validates completeness before sprint start | More reliable sprint commitments | • Sprint commitment reliability • % of stories meeting “Definition of Ready” |
| Development & Coding | High time spent on boilerplate; inconsistent patterns | AI accelerates code generation and enforces standards | Higher throughput without quality loss | • Cycle time per story • Code churn rate • Dev hours per feature |
| Code Review | Manual, time-consuming reviews; reviewer fatigue | AI flags issues early, humans focus on judgment | Faster PR cycles, more consistent quality | • PR review cycle time • \# of review iterations • Post-merge defect rate |
| Testing Strategy | Test planning happens late | AI supports early, feature-level test strategy | Earlier risk coverage, fewer late surprises | • % of features with test strategy defined pre-build • Defects found pre-UAT vs post-UAT |
| Test Case Creation | Manual test creation; limited coverage | AI generates broader, earlier test coverage | Higher defect detection earlier | • Test coverage depth (happy vs negative paths) • Defect discovery phase distribution |
| Test Automation | Slow-growing, brittle automation | AI accelerates regression & integration automation | Faster regression cycles, scalable quality | • Regression execution time • % regression automated • Automation maintenance effort |
| Documentation | Manual, outdated documentation | AI keeps docs aligned with code and configs | Reduced onboarding and support effort | • Time to onboard new team members • Support tickets caused by unclear docs |
| Release Communication | Manual, inconsistent release notes | AI-generated, structured release summaries | Better stakeholder understanding, fewer questions | • Post-release clarification requests • Time spent preparing release notes |
| Operational Feedback | Reactive analysis of production issues | AI summarizes ops signals and feeds back insights | Faster learning, fewer repeat issues | • Mean time to insight after incident • Repeat incident rate |
| Compliance & Governance | Manual evidence gathering; late audits | AI assists with traceability and completeness | Lower audit overhead, reduced compliance risk | • Audit prep time • % artifacts traceable end-to-end |
| Overall Delivery Performance | Speed and quality depend on heroics | Systematic efficiency across PDLC | More value with same teams; margin improvement | • End-to-end cycle time • Defect leakage to prod • Predictability vs plan |

# Core Principles (TBD)

### **1\. Integrated Agency**

* **Concept**: AI must operate within the practitioner's existing workspace (IDE, terminal, PM tools) rather than in disconnected chat interfaces.  
* **Goal**: Enable seamless data flow and environmental awareness to reduce context switching.

### **2\. Maximum Machine Utilization**

* **Concept**: Automated agents should run continuously—during active work, breaks, and off-hours—to triage backlogs, conduct research, or run simulations.  
* **Goal**: Ensure humans always return to a "warm start" with pre-processed information or draft artifacts.

### **3\. Failure-Driven Evolution**

* **Concept**: Every instance of AI error or hallucination must trigger a permanent update to the system’s shared instructions, validation checklists, or security filters.  
* **Goal**: Build a self-improving "governance harness" that systematically prevents the recurrence of known failure modes.

### **4\. Human Sovereignty & Accountability**

* **Concept**: The machine generates candidates and proposals, but only the human retains the authority to approve, commit, or deploy work.  
* **Goal**: Maintain strict governance and client trust through mandatory human decision gates.

### **5\. Verified Competence**

* **Concept**: Practitioners must be able to perform a task manually before delegating it to the machine to ensure effective auditing of outputs.  
* **Goal**: Prevent skill atrophy and ensure humans can identify subtle errors that novices might overlook.

### **6\. Data-Centric Architecture**

* **Concept**: As AI accelerates software creation, the value of underlying data increases; this requires modern, governed architectures to remain effective.  
* **Goal**: Treat quality data as the essential fuel for AI scaling, ensuring it is secure, accessible, and structured for machine consumption.


# Week 1

## Goals

* Use AI to deliver more with less, consistently across various engagement types

## Challenges

* Internal AI adaption   
* AI usage, governance and oversight (internal \+ external)

## Immediate steps

* **Identify and appoint program participants**  
  * TPO \- Alina Navarko  
  * Delivery Oversight \- Egor  
* **Confirm Executive Sponsor**   
  * Steve  
* **Form Feedback Group (“aka Stakeholders”)**  
  * Lee, Alex, Lucas, Sergey, Pavel  
* **Form Delivery Group**  
  * PTOs \- Elena etc  
  * Delivery Managers \- Humberto?  
  * Prompt developers (hands on the keyboard)   
  * Subgroups/Acc  
    * Dev \- Pablo  
    * QA \- Vasyl  
    * POs \- Lucas  
* **Meeting schedule:**  
  * Governance \-  Bi-weekly(progress review/updates)  
  * Delivery (weekly)  
  * Library/process demos \- bi-weekly  
* **Project Artifacts**  
  * Jira Instance  
  * Project Backlog  
  * Set up communication channels  
  * Prompts Library  
    * Code locations  
    * Prompt inventory  
  * Approved “AI toolset” \- claude/other?  
    * Access  
    * Licenses  
    * Etc  
  * Target project(s) teams  
    * Inventory of items/project that currently use AI  
      * Project  
      * SDLC phase (QA, Dev, other)  
      * Tools/tech used  
      * Existing KPIs (if any)  
      * AI champions  
      * Etc  
    * Inventory of teams/projects to POC AI

## Mid/Long term steps

* AI policy”  
  * Approved tooling  
  * Developer access/reimbursements  
  * Training  
  * Security reviews  
  * Standardized KPIs  
  * “AI usage/principles” one pager

	  
	

# \-Draft- Team Assessment

# **AI-Augmented SDLC: Team Maturity Assessment**

This assessment is designed to identify the current maturity level of a delivery team regarding AI integration. It serves as a tool for Delivery Managers and AI Champions to trigger conversations, identify gaps, and move from ad-hoc usage to a governed, high-multiplier state.

## **1\. AI Maturity Model (5 Levels)**

To standardize our evaluation, we use the following maturity tiers:

| Level | Name | Description |
| :---- | :---- | :---- |
| **L1** | **Ad-Hoc** | Individual, uncoordinated AI use. No shared prompts or official tools. |
| **L2** | **Enabled** | Basic tool access provided. Team starts using AI for boilerplate and unit tests. |
| **L3** | **Integrated** | AI is part of the "Definition of Ready/Done." Shared prompt library usage. |
| **L4** | **Optimized** | Measurable impact on Velocity/Quality (V×E×Q). Automated agent utilization. |
| **L5** | **Augmented** | AI-First mindset. Governance is self-improving. Human-AI agency is seamless. |

## 

## 

## 

## 

## **2\. Assessment Questionnaire (15 Questions)**

Rate each question from 1 (Never/No) to 5 (Always/Institutionalized).

### **Phase 1: Discovery & Strategy (Product Persona)**

1. **Requirements Expansion:** Does the team use AI (e.g., Claude, ChatGPT) to expand rough notes into structured user stories with acceptance criteria?  
2. **Edge Case Analysis:** Is AI utilized to systematically identify edge cases, NFRs, or error-handling scenarios during the grooming phase?  
3. **Backlog Prioritization:** Does the team use an AI-assisted framework (like RICE scoring prompts) to help justify and rank backlog items?

### **Phase 2: Development & Engineering (Dev Persona)**

4. **Tool Integration:** Are developers using integrated AI agents (e.g., Cursor, GitHub Copilot) directly in their IDE rather than just web-chat?  
5. **Boilerplate & Scaffolding:** Is AI the primary method for generating repetitive code (DTOs, Mappers, API controllers)?  
6. **Code Review Quality:** Does the team use AI to perform a "first pass" on PRs for security vulnerabilities and style violations before human review?  
7. **Refactoring & Technical Debt:** Is AI used to suggest refactoring patterns or identify "code smells" in legacy modules?

### **Phase 3: Validation & Quality (QA Persona)**

8. **Test Case Design:** Does the team generate test scenarios (positive, negative, and boundary) from acceptance criteria using approved prompts?  
9. **Automation Acceleration:** Is AI used to generate boilerplate automation scripts (Selenium, Playwright, or Cypress) to increase coverage?  
10. **Defect Clarity:** Are bug reports AI-augmented to ensure clear reproduction steps, severity justification, and potential root causes?  
11. **Synthetic Data Generation:** Does the team use AI to generate anonymized, realistic test data for complex scenarios?

### **Phase 4: Governance & Ethics (Risk Persona)**

12. **Data Privacy & Security:** Does the team actively strip PII/sensitive data before interacting with AI, or use strictly approved "Safe" environments?  
13. **Human Sovereignty:** Does the team follow a "Verify, Don't Just Trust" policy where every AI output is manually peer-reviewed?

### **Phase 5: Knowledge & Metrics (Delivery Persona)**

14. **Prompt Library Usage:** Does the team contribute to or use a shared "Prompt Library" rather than writing prompts from scratch every time?  
15. **Impact Tracking:** Is the team measuring the "AI Multiplier" (e.g., tracking time saved per task or change in cycle time)?

## 

## 

## **3\. Scoring & Maturity Mapping**

To determine the final maturity level, calculate the **Average Score** (Total Sum / 15).

| Average Score | Maturity Level | Internal Designation |
| :---- | :---- | :---- |
| **1.0 – 1.9** | **Level 1** | **Ad-Hoc:** AI use is a "dark secret" or purely individual. No team-wide benefit. |
| **2.0 – 2.9** | **Level 2** | **Enabled:** Team has tools but uses them reactively. High variability in quality. |
| **3.0 – 3.9** | **Level 3** | **Integrated:** AI is a standard teammate. Prompts are shared and results are consistent. |
| **4.0 – 4.9** | **Level 4** | **Optimized:** AI usage is driven by data. The team proactively automates bottlenecks. |
| **5.0** | **Level 5** | **Augmented:** The team operates at a new baseline. Humans focus only on high-order logic. |

**Note:** A team cannot be Level 4 or 5 if they score below a **4** on Question 12 (Security) or Question 13 (Human Sovereignty), regardless of their average.

## 

## **4\. Assessment Approach: The "Evidence-Based Interview"**

Instead of a cold survey, the Delivery Manager (DM) should lead a 45-minute interactive session. The goal is to move from **opinion** to **evidence**.

### **Step 1: The "Show Me" Protocol**

For any score of **4 or 5**, the team must provide a brief demonstration.

* *Example:* "You rated Requirements Expansion as a 5\. Can you show us the prompt used and the resulting User Story in Jira from the last sprint?"  
* *Example:* "You rated Tool Integration as a 5\. Can you demonstrate a 2-minute refactor using Cursor/Copilot right now?"

### **Step 2: The "Hallucination" Check**

The DM should ask: *"Tell me about a time the AI gave you the wrong answer this month. How did the team catch it and what did you learn?"*

* If the team says "It never happens," their maturity is likely **L1/L2** because they aren't pushing the tool hard enough or aren't reviewing outputs critically.

### **Step 3: Benchmarking the "North Star"**

Compare the team's results against flagship projects like **Lender** or **Tidal**.

* "On project Tidal, the team saved 30% of grooming time by using a specific Persona Prompt. How close are we to that workflow?"

### **Step 4: Action Planning (The "AI Sprint Goal")**

Identify the **two lowest-scoring questions**. These should not just be "fixed," but turned into a sprint goal.

* *Goal:* "In Sprint 24, we will move our 'Test Case Design' score from 2 to 4 by integrating the QA Prompt Library into our Definition of Ready."

### **Step 5: Metric Correlation**

The DM cross-references the assessment scores with the **V×E×Q metrics**. If maturity is high but Velocity is stagnant, the team may be using AI for the "wrong" things or experiencing "prompt-bloat" (spending too much time tweaking prompts).

