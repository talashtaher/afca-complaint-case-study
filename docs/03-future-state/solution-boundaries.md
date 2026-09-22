# Proposed solution boundaries

## Purpose

This document defines the proposed boundary of the complaint-management solution used in this case study.

The boundary clarifies which capabilities are being considered, which activities remain outside the solution and which dependencies require further discovery.

This is a business-analysis scope definition, not a commitment to a particular software product or implementation.

## Solution objective

The proposed solution will support consistent and traceable complaint handling from registration through closure by improving:

- case visibility;
- data quality;
- triage and priority;
- allocation and ownership;
- task and deadline monitoring;
- stage handover;
- exception management;
- auditability;
- privacy and access control; and
- operational reporting.

## In-scope capabilities

| Capability area | In-scope capability |
|---|---|
| Case registration | Create a unique complaint record and capture required intake information |
| Data validation | Identify missing, invalid or inconsistent information before progression |
| Classification | Record financial firm, product, complaint type, issues and relevant categories |
| Duplicate management | Identify possible duplicate or related complaints for human review |
| Triage | Produce explainable recommendations based on approved triage factors |
| Priority | Record recommended and confirmed priority, including override reasons |
| Allocation | Recommend and record ownership using approved capability and workload rules |
| Case visibility | Display stage, status, owner, next action, due date and blocking issue |
| Work management | Create tasks, reminders, due dates and escalation actions |
| Stage handover | Apply information checks before movement between process stages |
| Communication records | Record communications, requests, responses and communication status |
| Document handling | Attach or reference complaint evidence with appropriate access controls |
| Case management | Maintain case notes, activities, evidence, issues and resolution history |
| Decision support | Present relevant information to authorised decision-makers without deciding complaint merit automatically |
| Outcome and closure | Record outcome, closure reason, final communication and quality checks |
| Exception handling | Record, assign, monitor, escalate and close process exceptions |
| Audit history | Retain attributable records of material actions, decisions and changes |
| Access control | Restrict information and actions according to approved business roles |
| Operational reporting | Provide demand, workload, ageing, exception and outcome information |
| Rule governance | Maintain approved versions of configurable operational rules |

## In-scope users

The conceptual solution may support:

- Registration and Referral users;
- Case Management users;
- resolution or decision-making roles;
- operational managers;
- reporting and data users;
- system-support users;
- privacy, security and governance roles; and
- authorised external-facing support functions.

Exact role names and permissions require validation.

## In-scope information

The proposed information boundary includes:

- complaint identifier;
- received date and channel;
- complainant and contact information;
- communication and accessibility preferences;
- financial firm and product;
- complaint issues and description;
- classification, triage and priority;
- vulnerability or sensitive-handling indicators where appropriate;
- stage, status and closure reason;
- owner and assignment history;
- tasks, dates and escalation history;
- case notes and activities;
- communications;
- evidence and document references;
- related or duplicate cases;
- resolution activity;
- assessment or decision records;
- outcome;
- exceptions; and
- audit history.

Only information necessary for complaint handling should be collected and made available according to authorised need.

## External interfaces requiring validation

The solution may need to exchange information with:

- complaint-submission channels;
- financial-firm communication channels;
- email or correspondence services;
- document-storage services;
- identity and access-management services;
- reporting or analytics platforms; and
- approved reference-data sources.

These interfaces are discovery items. No existing AFCA integration is assumed.

## Out of scope

The following items are outside the current solution boundary:

- redesigning a financial firm’s internal dispute-resolution process;
- replacing financial firms’ internal systems;
- automatically deciding complaint merit or formal outcomes;
- replacing professional legal or operational judgement;
- processing compensation or financial payments;
- detailed legal interpretation of AFCA Rules;
- employee recruitment, payroll or general workforce management;
- full enterprise data-warehouse replacement;
- organisation-wide cybersecurity monitoring;
- public website redesign unrelated to complaint handling;
- selection or procurement of a specific CRM product;
- production infrastructure design;
- detailed data migration planning;
- implementation cost estimation;
- deployment and support operating models; and
- claims about existing AFCA technology.

These areas may become dependencies or separate projects but are not part of this case-study scope.

## Minimum viable capability

A minimum viable complaint-management solution should provide:

1. a central complaint record;
2. required-field validation;
3. stage, status, owner and next-action visibility;
4. documented triage and priority;
5. controlled allocation and reassignment;
6. tasks, due dates, reminders and escalation;
7. communication and document history;
8. stage-handover checks;
9. exception visibility;
10. role-based access;
11. material-action audit history; and
12. basic operational reporting.

## Possible later capabilities

Subject to evidence, governance and approval, later releases could consider:

- enhanced external self-service;
- direct financial-firm information exchange;
- advanced workload forecasting;
- configurable rule-management interfaces;
- enhanced data-quality monitoring;
- broader reporting integration;
- improved accessibility features;
- additional document automation; and
- trend-based capacity planning.

Predictive or automated recommendations should only be introduced where their inputs, fairness, explainability and human controls can be demonstrated.

## Assumptions

The scope currently assumes that:

- one complaint can move through several stages and statuses;
- authorised users require a shared case history;
- some cases need urgent or specialist handling;
- work can be assigned to a person or queue;
- tasks and due dates can be associated with a case;
- communications and documents need to be linked to the complaint;
- authorised users may override recommendations;
- overrides require reasons;
- sensitive information requires restricted access; and
- management requires operational visibility.

These assumptions must be validated.

## Constraints and unknowns

The case study does not currently have confirmed information about:

- existing applications;
- current integrations;
- detailed organisational roles;
- service-level targets;
- approved triage factors;
- workload thresholds;
- identity and access architecture;
- information-retention rules;
- technical hosting requirements;
- data volumes at case level; or
- implementation budget and timing.

These gaps limit solution-detail decisions and should remain visible in later requirements.

## Scope-control approach

A proposed requirement should be included only if it:

- supports the stated complaint-management objective;
- addresses an evidenced need or recorded hypothesis;
- fits within the agreed process boundary;
- has an identifiable stakeholder;
- can be tested or validated; and
- does not automate judgement that must remain human.

Requests outside this boundary should be recorded separately and assessed through a controlled scope-change process.