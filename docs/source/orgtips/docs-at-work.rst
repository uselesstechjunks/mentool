############################################################################
Docs @ Work
############################################################################

.. warning::
    Write

        - **minimum** correct document
        - at the **earliest** useful time
        - for the **widest** necessary audience.

============================================================================
When, Why, Who, What?
============================================================================

------------------------------------------------------------------------
A. Before Building - Alignment & Planning
------------------------------------------------------------------------

- [verb:own] Design Docs: clarify problem, goals, trade-offs, proposed solution.
- [verb:review] PRDs: product-side framing of why/what to build.
- [verb:co-own] RFCs: socialize big or cross-team changes, gather feedback.

------------------------------------------------------------------------
B. During Development - Execution & Interfaces
------------------------------------------------------------------------

- [verb:own] Tech Specs / API Docs: define contracts, data schemas, interfaces.
- [verb:co-own] Meeting/Decision Notes: record ongoing decisions, unblockers, next steps.

------------------------------------------------------------------------
C. After Experimentation - Evaluation & Iteration
------------------------------------------------------------------------

- [verb:own] Experiment Docs: capture hypotheses, metrics, results, learnings.

------------------------------------------------------------------------
D. In Production - Operations & Maintenance
------------------------------------------------------------------------

- [verb:co-own] Runbooks / Playbooks: step-by-step guides for incidents & debugging.
- [verb:own] Onboarding/Knowledge Docs: long-term references to ramp up engineers and avoid institutional memory loss.

============================================================================
How?
============================================================================

------------------------------------------------------------------------
1. Design Docs (System/ML/Experiment)
------------------------------------------------------------------------
.. important::

    - Write when the problem or trade-offs are unclear.
    - Capture decisions and rejected alternatives explicitly.

- Best Practice: Keep decision rationale explicit; diagrams > text walls.
- Structure: Title: [System/Model Name] Design Doc

    - Context / Background
    - Problem Statement
    - Goals & Non-Goals
    - Proposed Solution (with diagram)
    - Alternatives Considered
    - Rollout Plan / Monitoring
    - Risks & Open Questions

------------------------------------------------------------------------
2. PRDs (Product Requirement Docs)
------------------------------------------------------------------------
.. important::

    - Problem and success metrics must be measurable.
    - If metrics are vague, stop and fix before execution.

- Best Practice: Clarify "why now" and measurable success upfront. Bother only if you partner with PMs.
- Structure: Title: [Feature/Project Name] PRD

    - Context / Motivation
    - Problem / User Need
    - Target Users & Use Cases
    - Requirements (Must / Nice to Have)
    - Success Metrics / KPIs
    - Out of Scope
    - Timeline & Dependencies

------------------------------------------------------------------------
3. RFCs (Request for Comments)
------------------------------------------------------------------------
.. important::

    - Use when cross-team impact or approval is required.
    - Publish early, before commitment or implementation.

- Best Practice: Keep decision logs so future engineers see why something was chosen.
- Structure: Title: RFC: [Proposed Change]

    - Summary
    - Motivation / Why Now
    - Detailed Proposal
    - Alternatives Considered
    - Impact (Teams, APIs, Infra)
    - Backward Compatibility / Migration
    - Open Questions

------------------------------------------------------------------------
4. Tech Specs / API Docs
------------------------------------------------------------------------
.. important::

    - Write once interfaces or schemas must be stable.
    - Treat it as a contract; update when compatibility changes.

- Best Practice: Keep concise, machine-readable schemas alongside human docs.
- Structure: Title: [Service / API Spec]

    - Overview / Purpose
    - Inputs & Outputs
    - Data Schema / Contracts
    - Endpoints / Interfaces
    - Example Requests & Responses
    - Edge Cases / Error Handling

------------------------------------------------------------------------
5. Meeting/Decision Notes
------------------------------------------------------------------------
.. important::

    - Write when decisions are made verbally.
    - Decisions and owners must be explicit and timestamped.

- Best Practice: Send out within 24h; decisions bolded.
- Structure: Meeting: [Name, Date]

    - Attendees
    - Agenda
    - Discussion Highlights
    - Decisions (bolded)
    - Action Items (with owners & deadlines)

------------------------------------------------------------------------
6. Experiment Docs
------------------------------------------------------------------------
.. important::

    - Every experiment must have a hypothesis and metrics.
    - Always record outcomes, even if decision is already made.

- Best Practice: Include links to dashboards, queries, PRDs.
- Structure: Experiment: [Name]

    - Background / Hypothesis
    - Experiment Design (groups, traffic split, duration)
    - Metrics (Primary / Guardrail)
    - Results & Analysis
    - Learnings
    - Next Steps
    - Links (dashboards, queries, PRs)

------------------------------------------------------------------------
7. Runbooks / Playbooks
------------------------------------------------------------------------
.. important::

    - Optimize for 3 AM usage by someone without context.
    - No design rationale; only symptoms and actions.

- Best Practice: Test them via dry-runs; keep "one-page quick actions" upfront.
- Structure: Service / Model: [Name]

    - Symptoms / Alerts
    - Diagnosis Steps
    - Known Issues
    - Mitigation / Recovery Steps
    - Escalation Paths
    - Quick Reference (one-liner commands, dashboards)

------------------------------------------------------------------------
8. Onboarding/Knowledge Docs
------------------------------------------------------------------------
.. important::

    - Answer “how does this system actually work end-to-end.”
    - Update when tribal knowledge causes repeated questions.

- Best Practice: Keep "getting started in < 1hr" flow at top.
- Structure: Topic: [System / Team Name]

    - Introduction / High-level Overview
    - Architecture Diagram
    - How to Get Started (setup in <1hr)
    - Common Workflows
    - Pitfalls / Gotchas
    - Resources (dashboards, repos, contacts)

============================================================================
Anything Else?
============================================================================
------------------------------------------------------------------------
Supporting Details Doc - [H1 20XX / H2 20XY]
------------------------------------------------------------------------

1. Career Alignment

    - Long-term aspiration: [e.g. Senior -> Staff -> Senior Staff, or technical leadership in XYZ domain]
    - Key themes this cycle: [Execution excellence, Technical depth, Mentorship, etc.]
    - Connection to company/organization goals: [short bullets]

2. Weekly Rhythm

    - Rituals: [standup, weekly reflection, learning block, 1:1 prep]
    - Weekly focus areas: [delivery, design reviews, infra deep dive, mentoring]
    - Status log: [table with week/date | wins | blockers | next focus]
    
3. Active Projects

    - Project 1: [title, owner, status, link to doc]
    
        - Key metrics: [...]
        - Next milestones: [...]
        - Commands/snippets/config notes: (inline or linked)
    - Project 2: ...

4. Work Artifacts

    - Owned Docs: [links]
    - Co-owned Docs: [links]
    - Reviews / RFCs: [links]
    - Code repos: [links]

5. Knowledge Base

    - Domain knowledge: [links to wikis, internal docs, papers]
    - Tech stack - inside company: [infra, APIs, pipelines]
    - Tech stack - outside company: [OSS libraries, blogs, references]

6. Retros & Checkpoints

    - Mid-cycle reflection: [notes]
    - End-cycle reflection: [impact vs goals, lessons learned]
