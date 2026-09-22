# UAT Approach and Scenarios

## Purpose

This document defines a proposed User Acceptance Testing approach for the complaint-management solution.

UAT would confirm that the implemented solution supports the approved business process, requirements and user needs. The roles, environments, test data, dates and approval authorities are illustrative and require stakeholder confirmation.

## UAT objectives

UAT should confirm that:

- core complaint-management workflows can be completed by authorised users;
- business rules operate as approved;
- human review and override controls are preserved;
- case ownership, history and exceptions remain visible;
- sensitive information is appropriately restricted;
- reporting measures are consistent and explainable;
- accessibility requirements are supported; and
- critical defects are resolved before release approval.

## UAT scope

### In scope

- case creation and mandatory-field validation;
- duplicate and related-case warnings;
- classification, triage and priority;
- allocation, ownership and reassignment;
- tasks, due dates, alerts and exceptions;
- structured handovers;
- communications and documents;
- outcomes, closure and reopening;
- role-based access and audit history;
- operational views and reports; and
- representative accessibility checks.

### Outside UAT scope

The following would normally be assessed through other testing activities:

- detailed code-level testing;
- penetration testing;
- infrastructure resilience testing;
- full performance and load testing;
- disaster-recovery certification;
- third-party platform certification; and
- assessment of complaint merit or professional decisions.

UAT may review the results of these tests where they affect business acceptance.

## Proposed UAT participants

| Role | Proposed responsibility |
|---|---|
| Business sponsor or delegate | Confirms business acceptance and unresolved-risk decisions |
| UAT lead | Coordinates scope, schedule, evidence, defects and reporting |
| Business process representatives | Execute realistic end-to-end scenarios |
| Privacy and security representatives | Review access, sensitive information and audit controls |
| Accessibility representative | Reviews representative workflows and communication needs |
| Reporting representative | Validates measures, filters and reconciliations |
| Delivery and support representatives | Investigate defects and support retesting |

These are generic testing responsibilities rather than confirmed AFCA roles.

## Entry criteria

UAT should begin only when:

- the agreed UAT scope and requirements baseline are available;
- testable acceptance criteria have been approved;
- the UAT environment is stable and accessible;
- required integrations or approved substitutes are available;
- representative and privacy-safe test data has been prepared;
- required user roles and permissions have been configured;
- system and integration testing have reached the agreed completion level;
- no unresolved defect prevents meaningful UAT execution; and
- participants have received sufficient process and system guidance.

## Exit criteria

UAT may be recommended for completion when:

- all critical business scenarios have been executed;
- agreed acceptance criteria have been assessed;
- no unresolved critical defect remains;
- high-severity defects have been resolved or formally accepted with treatment plans;
- required regression testing has been completed;
- reporting and access controls have been validated;
- outstanding limitations and residual risks are documented; and
- the authorised approver has recorded the release decision.

Exact thresholds and approval authorities require stakeholder agreement.

## Test-data approach

UAT data should:

- be synthetic or appropriately de-identified;
- represent standard, incomplete, duplicate, priority and exception cases;
- include different ownership, stage and status combinations;
- cover permitted and restricted access scenarios;
- avoid unnecessary personal or sensitive information;
- support reporting and reconciliation scenarios; and
- be reset or disposed of according to the approved test-data procedure.

## Defect management

Each defect should record:

- a unique identifier;
- related scenario and requirement;
- summary and reproduction steps;
- expected and actual results;
- evidence;
- severity and priority;
- owner and status;
- resolution details; and
- retest outcome.

Proposed severity categories are:

| Severity | Description |
|---|---|
| Critical | Prevents a core process or creates an unacceptable security, privacy or data-integrity risk |
| High | Materially affects an important business outcome with no acceptable workaround |
| Medium | Affects a function but an acceptable temporary workaround exists |
| Low | Minor usability, presentation or documentation issue |

Severity definitions require formal approval before UAT.

## UAT scenarios

| Scenario ID | Scenario | Expected business outcome | Related criteria |
|---|---|---|---|
| UAT-01 | Create a case with all mandatory information | A unique case is created with complete creation history | AC-01 |
| UAT-02 | Attempt to progress an incomplete case | Missing information is identified and uncontrolled progression is prevented | AC-02–AC-03 |
| UAT-03 | Create a complaint matching an existing case | A warning is displayed and the user can confirm, reject or link the match | AC-04–AC-05 |
| UAT-04 | Generate and review a triage recommendation | The recommendation and contributing factors are displayed | AC-06–AC-07 |
| UAT-05 | Confirm and override a recommended priority | Confirmation is recorded and an override requires a reason | AC-08–AC-09 |
| UAT-06 | Process a case containing an approved vulnerability or priority indicator | The case is flagged for human review without an automated outcome decision | AC-10 |
| UAT-07 | Generate an allocation recommendation | Approved allocation factors and the proposed owner or team are displayed | AC-11–AC-12 |
| UAT-08 | Override an allocation and reassign a case | Reasons and ownership history are retained | AC-13–AC-16 |
| UAT-09 | Open an active case and review its summary | Stage, status, priority, owner and key dates are visible | AC-17 |
| UAT-10 | Create, assign and complete a task | Task ownership, status, due date and completion history are recorded | AC-18–AC-19 |
| UAT-11 | Trigger and resolve an approved alert | The alert becomes visible and its resolution history is preserved | AC-20–AC-21 |
| UAT-12 | Record notes, activities and decisions | Entries appear chronologically and protected history cannot be silently changed | AC-22–AC-23 |
| UAT-13 | Attempt a handover with missing required information | Missing information is identified and uncontrolled transfer is prevented | AC-24–AC-25 |
| UAT-14 | Record a communication and attach a document | Both are linked to the correct case and protected by approved access | AC-26–AC-27 |
| UAT-15 | Prepare communication using an approved template and accessibility requirement | The current template and relevant communication requirement are presented | AC-28–AC-29 |
| UAT-16 | Attempt to access restricted information using permitted and unpermitted roles | Authorised access succeeds, unauthorised access is denied and required activity is recorded | AC-30–AC-31 |
| UAT-17 | Attempt closure with incomplete information, then complete closure | Incomplete closure is prevented and valid closure details are recorded | AC-32–AC-33 |
| UAT-18 | Reopen a closed case | A reason is required and the original closure history remains visible | AC-34–AC-35 |
| UAT-19 | Review workload, ageing, priority, stage and exception information | Approved operational information is displayed consistently | AC-36 |
| UAT-20 | Run and reconcile an approved report | Results are repeatable and the measure definition is available | AC-37–AC-38 |
| UAT-21 | Create, assign, resolve and close an exception | The exception remains visible and retains its resolution history | AC-39–AC-40 |
| UAT-22 | Change an approved configurable rule | Approval and version history are required before activation | AC-41–AC-42 |
| UAT-23 | Search and attempt to alter audit history | Authorised search succeeds and unauthorised alteration is prevented | AC-43–AC-44 |
| UAT-24 | Complete representative workflows using keyboard navigation and approved assistive technology | Core functions remain understandable and operable | NFR-11–NFR-15 |
| UAT-25 | Simulate a failed transaction or unavailable integration | No unexplained duplicate or incomplete case is created, and the failure is visible | NFR-20, NFR-24, NFR-27 |

## UAT evidence

Evidence may include:

- completed test scripts;
- screenshots or recordings containing no uncontrolled sensitive information;
- generated records and reports;
- audit-history extracts;
- defect and retest records;
- accessibility review results;
- reconciliation results; and
- formal approval or conditional-approval decisions.

## UAT limitations

This document is a proposed business-testing approach. It cannot define confirmed test dates, participants, environments, service levels or release thresholds without stakeholder and technical input.