# Prioritised Backlog

## Purpose

This backlog organises the proposed user stories into an initial delivery sequence. Priorities are preliminary and must be reviewed with authorised stakeholders before delivery planning.

The sequence considers business value, risk, dependencies and the need to establish controlled case records before introducing more advanced capabilities.

## Prioritisation approach

The backlog uses MoSCoW priorities:

- **Must** — required for the core complaint-management capability.
- **Should** — important but may follow the core capability.
- **Could** — beneficial if capacity permits.
- **Won't for now** — outside the current proposed release.

Rank indicates the proposed implementation order within this case study. It is not a confirmed delivery schedule.

## Proposed backlog

| Rank | Story | Backlog item | Epic | Priority | Key dependency or rationale |
|---:|---|---|---|---|---|
| 1 | US-26 | Control access and maintain traceable material actions | Security and audit | Must | Foundational control required across the solution |
| 2 | US-01 | Create a complaint case with a unique identifier | Case intake | Must | Establishes the core case record |
| 3 | US-02 | Identify and manage missing mandatory information | Case intake | Must | Depends on the case record and approved mandatory fields |
| 4 | US-03 | Identify and review potential duplicate or related cases | Case intake | Must | Reduces fragmented records before later processing |
| 5 | US-04 | Generate an explainable triage recommendation | Triage | Must | Requires validated case information and approved rules |
| 6 | US-05 | Confirm or override the recommended priority | Triage | Must | Preserves human judgement and accountability |
| 7 | US-06 | Flag approved priority or vulnerability indicators for review | Triage | Must | Supports appropriate human attention and accessible handling |
| 8 | US-07 | Generate a workload-aware allocation recommendation | Allocation | Must | Requires confirmed priority and approved allocation criteria |
| 9 | US-08 | Override an allocation recommendation with a recorded reason | Allocation | Must | Supports controlled handling of exceptional circumstances |
| 10 | US-09 | Display the current case owner and accountable team | Allocation | Must | Establishes visible responsibility for active work |
| 11 | US-11 | Display core case status and key information together | Case management | Must | Supports efficient case understanding |
| 12 | US-12 | Create and manage case tasks and due dates | Case management | Must | Supports controlled execution of case work |
| 13 | US-13 | Alert users to cases and tasks requiring attention | Monitoring | Must | Depends on approved tasks, dates and alert rules |
| 14 | US-14 | Record notes, activities and decisions in case history | Case management | Must | Supports continuity, accountability and audit |
| 15 | US-15 | Complete a structured handover between stages or teams | Case management | Must | Depends on defined stages, ownership and required handover data |
| 16 | US-16 | Link communications and documents to the relevant case | Communications | Must | Supports a complete and usable case record |
| 17 | US-18 | Display communication preferences and accessibility requirements | Communications | Must | Supports appropriate and accessible communication |
| 18 | US-19 | Restrict sensitive information to authorised roles | Security and privacy | Must | Applies privacy controls to documents and communications |
| 19 | US-20 | Validate required information before case closure | Outcome and closure | Must | Depends on approved outcomes and closure rules |
| 20 | US-21 | Reopen a case without losing its original closure history | Outcome and closure | Must | Supports controlled continuation of closed cases |
| 21 | US-24 | Record, assign and resolve process exceptions | Exception management | Must | Supports visibility of cases outside the standard path |
| 22 | US-22 | View workload, ageing, priority, stage and exceptions | Operational oversight | Must | Depends on reliable operational case data |
| 23 | US-23 | Produce reports using approved definitions | Reporting | Must | Depends on agreed measures and reliable source data |
| 24 | US-10 | Identify reassignment history and repeated transfers | Allocation | Should | Enhances ownership monitoring after core allocation is established |
| 25 | US-17 | Use approved communication templates | Communications | Should | Improves consistency after core communication recording is available |
| 26 | US-25 | Configure approved rules, categories and templates | Administration | Should | Requires governance, permissions and version-control arrangements |

## Suggested delivery increments

### Increment 1 — Controlled case foundation

- US-26: access and audit controls;
- US-01: case creation;
- US-02: mandatory-information validation;
- US-09: ownership visibility;
- US-11: case summary; and
- US-14: case history.

### Increment 2 — Triage and allocation

- US-03: duplicate and related-case review;
- US-04: triage recommendation;
- US-05: priority confirmation and override;
- US-06: human review indicators;
- US-07: allocation recommendation; and
- US-08: controlled allocation override.

### Increment 3 — Case work and communication

- US-12: tasks and due dates;
- US-13: alerts;
- US-15: structured handover;
- US-16: communications and documents;
- US-18: communication and accessibility requirements; and
- US-19: sensitive-information restrictions.

### Increment 4 — Closure, exceptions and oversight

- US-20: closure validation;
- US-21: controlled reopening;
- US-24: exception management;
- US-22: operational views; and
- US-23: management reporting.

### Increment 5 — Optimisation

- US-10: reassignment monitoring;
- US-17: communication templates; and
- US-25: configurable rules, categories and templates.

## Prioritisation factors requiring validation

Stakeholders must confirm:

- which capabilities are mandatory for the first usable release;
- whether any legal, privacy, security or accessibility requirements change the sequence;
- technical dependencies and integration constraints;
- availability of approved business rules and reference data;
- implementation effort and delivery capacity;
- migration and operational-readiness requirements; and
- the definition of success for each increment.