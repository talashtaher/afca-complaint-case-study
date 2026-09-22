# Proposed decision rules

## Purpose

This document defines proposed business rules for complaint validation, triage, priority, allocation, monitoring and closure.

The rules translate the future-state process into testable business logic. They are case-study proposals and require validation with authorised stakeholders before implementation.

No rule should make a final decision about complaint merit or outcome.

## Rule principles

The rules should be:

- transparent to authorised users;
- applied consistently;
- configurable through controlled governance;
- explainable when they affect priority or allocation;
- subject to human review for sensitive or exceptional cases;
- recorded in the audit history; and
- tested for unintended or unfair outcomes.

## Evaluation order

Rules should be evaluated in the following order:

1. validate required information;
2. identify possible duplicates or related cases;
3. identify urgent, vulnerable, complex or accessibility circumstances;
4. recommend priority;
5. identify eligible owners or queues;
6. recommend allocation;
7. create tasks, dates and monitoring alerts;
8. monitor exceptions throughout the case; and
9. validate outcome and closure information.

## Validation rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| VR-01 | Mandatory complaint information is missing | Prevent normal progression and identify the missing fields | An authorised user may permit limited progression where appropriate and record the reason |
| VR-02 | A document cannot be opened or does not meet an accepted format | Flag the document and request a usable version | A user confirms whether alternative evidence is acceptable |
| VR-03 | Key dates are invalid or inconsistent | Display a validation error or warning | A user corrects or explains the exception |
| VR-04 | The financial firm or product cannot be identified confidently | Route the case for manual review | A user confirms the correct firm or classification |
| VR-05 | Required communication or accessibility information is incomplete | Prompt the user to complete or confirm it | A user determines whether the case can proceed safely |

## Duplicate and related-case rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| DR-01 | Key identifiers match an existing complaint | Display a possible-duplicate warning | A user decides whether the complaint is duplicate, related or separate |
| DR-02 | Complaints involve the same complainant, firm and issue within a relevant period | Suggest linking the records | A user confirms the relationship |
| DR-03 | A possible duplicate includes materially different issues | Do not automatically merge the records | A user determines the appropriate record structure |
| DR-04 | Records are linked or merged | Retain the original identifiers and action history | The action and reason must be auditable |

## Triage rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| TR-01 | Information indicates urgent circumstances or risk of material harm | Flag for immediate review and recommend higher priority | An authorised user confirms the urgency and handling approach |
| TR-02 | Vulnerability indicators are recorded | Flag the need for appropriate support and review | A user confirms the handling needs; vulnerability must not determine complaint merit |
| TR-03 | Accessibility or communication needs are recorded | Display the required adjustment prominently to authorised users | A user confirms how the need will be supported |
| TR-04 | The complaint has multiple issues, parties, products or substantial evidence | Recommend a complexity review | A user confirms complexity and specialist needs |
| TR-05 | The complaint involves a sensitive or unusual circumstance | Route it to a designated review queue | An authorised user determines the appropriate handling |
| TR-06 | No exceptional indicator is identified | Apply the standard triage pathway | A user may still record an exception with a reason |

## Priority rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| PR-01 | One or more confirmed urgent factors apply | Recommend urgent priority | Human confirmation is mandatory |
| PR-02 | The complaint requires prompt attention but does not meet urgent criteria | Recommend high priority | A user confirms or changes the recommendation |
| PR-03 | No higher-priority factor applies | Recommend standard priority | A user may override with a recorded reason |
| PR-04 | Multiple priority factors apply | Recommend the highest applicable priority | The factors and final decision must be visible |
| PR-05 | Priority is increased or reduced after confirmation | Record the previous value, new value, user and reason | Only authorised roles may change confirmed priority |
| PR-06 | A priority recommendation is based on incomplete information | Mark the recommendation as provisional | A user reviews it when the missing information is received |

Exact priority categories and service targets require stakeholder approval.

## Allocation rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| AR-01 | A case requires specific product or complaint knowledge | Limit the recommendation to eligible owners or queues | A user confirms the required capability |
| AR-02 | More than one eligible owner is available | Consider active workload and case complexity | A user can review the allocation basis |
| AR-03 | An existing owner is already handling a directly related case | Consider continuity of ownership | A user confirms whether continuity is appropriate |
| AR-04 | An eligible owner is unavailable or has exceeded an agreed workload threshold | Exclude or deprioritise that owner temporarily | A manager can approve an exception |
| AR-05 | No eligible owner is available | Place the case in a visible exception queue and alert the responsible manager | Manual assignment or capacity action is required |
| AR-06 | A recommended allocation is overridden | Require an override reason | The change must be recorded in the audit history |
| AR-07 | A case is reassigned | Retain the previous owner, date and reason | An authorised user confirms the reassignment |
| AR-08 | Eligible owners have comparable workload and capability | Use an agreed neutral allocation method | The method must be documented and reviewable |

Allocation should not use personal characteristics unrelated to the work.

## Monitoring and escalation rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| ER-01 | A case has no assigned owner after an agreed period | Alert the responsible queue or manager | A user assigns or records the reason for delay |
| ER-02 | A required action is approaching its due date | Notify the responsible owner | The owner updates the action or due date where authorised |
| ER-03 | A required action becomes overdue | Escalate according to the agreed path | A user records the recovery action |
| ER-04 | A high-priority case has no recent recorded activity | Generate an exception alert | A user reviews the case and records the next action |
| ER-05 | Information required from an external party remains outstanding | Create a follow-up task based on the approved schedule | A user may adjust the follow-up where appropriate |
| ER-06 | A case is reassigned repeatedly | Flag it for management review | A manager investigates the reason |
| ER-07 | A stage handover is incomplete | Prevent acceptance or route it to an exception queue | An authorised user may accept an exception with a reason |
| ER-08 | An access or audit-control exception occurs | Alert the appropriate control owner | Investigation and resolution remain human responsibilities |

Specific time thresholds and escalation levels require operational validation.

## Closure rules

| Rule ID | Condition | Proposed system response | Human control |
|---|---|---|---|
| CR-01 | A user attempts to close a case without an outcome and closure reason | Prevent closure | The user completes the required information |
| CR-02 | Required actions remain open | Warn or prevent closure according to the approved rule | An authorised user resolves or accepts the exception |
| CR-03 | Final communication has not been recorded | Flag the missing communication | A user confirms the communication requirement |
| CR-04 | A formal assessment or decision requires approval | Prevent final closure until approval is recorded | An authorised decision-maker completes the approval |
| CR-05 | Closure information passes validation | Record the closure date, outcome, user and final status | The responsible user confirms completion |
| CR-06 | A closed case is reopened | Preserve the original closure information and record the reason | Only authorised roles may reopen the case |

## Fairness and control requirements

The decision rules must not:

- determine complaint merit automatically;
- disadvantage a complainant because of an accessibility need;
- use irrelevant personal characteristics for priority or allocation;
- conceal why a priority or allocation recommendation was made;
- prevent authorised users from handling genuine exceptions; or
- allow overrides without an attributable reason.

Periodic review should examine:

- priority patterns;
- allocation distribution;
- override frequency;
- reassignment frequency;
- exception volumes;
- overdue cases; and
- whether any rule produces unintended outcomes.

## Governance requirements

Each implemented rule should have:

- a named business owner;
- an approved definition;
- a version and effective date;
- documented inputs and outputs;
- user roles permitted to override it;
- test scenarios;
- monitoring measures; and
- a controlled change and approval process.