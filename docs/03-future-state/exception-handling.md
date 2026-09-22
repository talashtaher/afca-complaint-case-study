# Proposed exception-handling approach

## Purpose

This document defines how the future-state complaint process should identify, control, resolve and audit situations that cannot follow the normal workflow.

Exception handling should keep unusual cases visible without allowing them to disappear into informal workarounds.

The proposed approach requires operational validation before implementation.

## Exception-handling principles

1. Every exception should have a clear owner.
2. The reason for the exception should be recorded.
3. Urgent, sensitive and security-related exceptions should be visible immediately.
4. An exception should not remove the underlying case from normal reporting.
5. Manual workarounds should be time-limited and traceable.
6. Overrides should require an authorised user and recorded explanation.
7. Resolution should be verified before the exception is closed.
8. Repeated exceptions should be reviewed for process or system improvement.

## Exception lifecycle

The proposed exception lifecycle is:

1. **Detect** — identify the issue through a rule, alert, user report or monitoring control.
2. **Record** — create an exception record linked to the complaint.
3. **Classify** — record the type, severity and business impact.
4. **Contain** — prevent inappropriate progression, access or closure where necessary.
5. **Assign** — allocate the exception to a responsible person or queue.
6. **Resolve** — complete the required corrective action.
7. **Verify** — confirm that the case can safely return to the normal process.
8. **Close** — record the resolution, date, owner and any follow-up action.

## Severity guidance

| Severity | Description | Proposed response |
|---|---|---|
| Critical | Potential immediate harm, serious privacy or security concern, or risk of an inappropriate material decision | Contain the issue and route it for immediate authorised review |
| High | Prevents an urgent or important complaint from progressing appropriately | Assign for priority review and management visibility |
| Medium | Disrupts normal progression but has an available controlled workaround | Assign to the responsible operational or support queue |
| Low | Minor data-quality or administrative issue with limited immediate impact | Record and resolve through standard work management |

Exact severity definitions and response targets require stakeholder approval.

## Exception register

| Exception ID | Trigger | Immediate response | Proposed owner | Resolution condition |
|---|---|---|---|---|
| EX-01 | Mandatory information is missing | Identify missing information and pause affected progression | Responsible operational queue | Required information is received or an authorised exception is recorded |
| EX-02 | A possible duplicate or related complaint is detected | Display matching records and prevent automatic merging | Operational reviewer | Records are confirmed as duplicate, related or separate |
| EX-03 | The financial firm, product or complaint type cannot be identified | Route the case for classification review | Designated review queue | Classification is confirmed and recorded |
| EX-04 | No eligible owner or queue is available | Place the case in a visible unallocated-work queue and alert management | Operational manager | An appropriate owner is assigned or capacity action is recorded |
| EX-05 | A required action becomes overdue | Alert the owner and escalate according to the approved path | Case owner and operational manager | The action is completed or a revised authorised plan is recorded |
| EX-06 | A high-priority case has no recent activity | Flag the case for immediate review | Case owner or priority-review queue | A valid next action and owner are recorded |
| EX-07 | A stage handover is incomplete | Prevent normal acceptance into the next stage | Sending and receiving operational functions | Required handover information is completed or an exception is accepted |
| EX-08 | A case is reassigned repeatedly | Flag the case for management review | Operational manager | Ownership is stabilised and the cause of reassignment is recorded |
| EX-09 | Communication with a party repeatedly fails | Record failed attempts and prompt an alternative communication review | Case owner | An approved communication approach or next action is recorded |
| EX-10 | An accessibility or communication need cannot be met through the standard process | Route for appropriate support and prevent unsuitable communication | Responsible operational or accessibility-support role | An appropriate adjustment or alternative approach is confirmed |
| EX-11 | Possible inappropriate access or disclosure is detected | Restrict affected access where appropriate and notify the control owner | Privacy or security function | The concern is investigated and required action is completed |
| EX-12 | The complaint-management system is unavailable | Activate the approved continuity procedure and record affected work | Technology support and operational management | Service is restored and temporary records are reconciled |
| EX-13 | A business rule produces conflicting or unclear results | Stop automatic progression and request authorised review | Business-rule owner or designated reviewer | The case decision and rule interpretation are recorded |
| EX-14 | Reported figures do not reconcile with source case data | Flag the report and prevent unsupported conclusions | Data or reporting owner | The cause is corrected or the difference is explained |
| EX-15 | A user attempts closure with unresolved actions or missing outcome information | Prevent or warn against closure according to the approved rule | Responsible case owner | Required closure information and actions are complete |
| EX-16 | A closed case needs to be reopened | Preserve the previous closure record and require a reason | Authorised operational role | The reopened case has a valid status, owner and next action |

## Required exception information

Each exception record should include:

- exception identifier;
- related complaint identifier;
- exception type;
- severity;
- date and time detected;
- detection source;
- description;
- business impact;
- assigned owner or queue;
- containment action;
- due date or review date;
- status;
- escalation history;
- resolution action;
- verification result;
- closure date; and
- linked evidence or communication.

## Escalation considerations

Escalation may be required when:

- potential harm or a serious security concern exists;
- a high-priority case remains blocked;
- no responsible owner can be identified;
- the same exception occurs repeatedly;
- a deadline continues to be missed;
- an override affects fairness or access;
- a workaround creates further risk;
- a business rule is producing unexpected outcomes; or
- resolution requires authority beyond the current owner.

The escalation path, responsible roles and response targets must be agreed during implementation planning.

## Management visibility

Future-state reporting should show:

- open exceptions by type and severity;
- exceptions without an owner;
- overdue exceptions;
- average time to resolve;
- repeated exceptions by process stage;
- cases with multiple exceptions;
- rule overrides;
- failed handovers;
- repeated reassignments;
- access or security exceptions; and
- recurring root-cause themes.

These measures should be used to improve the process rather than automatically assess individual employee performance.

## Closure controls

An exception should only be closed when:

- the corrective action is complete;
- the underlying complaint can safely continue or close;
- the resolution has been verified;
- required evidence is attached or referenced;
- any temporary workaround has been reconciled;
- affected stakeholders have been informed where required; and
- follow-up improvement work has been recorded.

## Review and improvement

Recurring exceptions should be reviewed to determine whether the cause relates to:

- unclear process guidance;
- incomplete data capture;
- training needs;
- workload or capacity;
- unsuitable business rules;
- system configuration;
- integration failure;
- access design; or
- external communication difficulties.

Any proposed change should follow controlled approval, testing and release processes.