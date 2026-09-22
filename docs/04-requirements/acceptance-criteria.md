# Acceptance Criteria

## Purpose

These acceptance criteria provide testable conditions for the proposed user stories. They are written at a business level and require stakeholder review before being used for implementation or testing.

## Case creation, validation and triage

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-01 | US-01 | An authorised intake user has the required complaint information | The user creates a case | The solution creates one case record with a unique identifier and records its creation date and user |
| AC-02 | US-02 | One or more mandatory fields are incomplete | The user attempts to progress the case | The solution identifies each missing field and prevents progression unless an authorised exception is recorded |
| AC-03 | US-02 | An authorised user accepts an incomplete case | The user records the approved exception reason | The solution retains the reason, user, date and time in the case history |
| AC-04 | US-03 | Another case meets the approved potential-match criteria | A complaint is created or reviewed | The solution displays a potential duplicate or related-case warning without automatically merging the records |
| AC-05 | US-03 | A potential match has been displayed | An authorised user reviews it | The user can confirm, reject or link the match, and the action is recorded |
| AC-06 | US-04 | Required classification information is available | A triage assessment is requested | The solution produces a recommendation using the approved rules |
| AC-07 | US-04 | A triage recommendation has been produced | The user reviews the recommendation | The solution displays the contributing factors and applicable rule version |
| AC-08 | US-05 | A priority recommendation is available | The authorised user confirms it | The selected priority is saved with the confirming user, date and time |
| AC-09 | US-05 | An authorised user selects a different priority | The user submits the change | The solution requires and records an override reason |
| AC-10 | US-06 | A case contains an approved priority or vulnerability indicator | The case is assessed | The solution flags the case for human review and does not make an automatic merit or outcome decision |

## Allocation and ownership

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-11 | US-07 | A case is ready for allocation | An allocation recommendation is requested | The solution considers the approved capability, availability and workload criteria |
| AC-12 | US-07 | An allocation recommendation is generated | The user views it | The proposed owner or team and the contributing criteria are displayed |
| AC-13 | US-08 | An authorised user does not accept the allocation recommendation | The user selects another eligible owner | The solution requires and records an override reason before completing the allocation |
| AC-14 | US-09 | An active case has been allocated | An authorised user opens the case | The current owner and accountable team are clearly displayed |
| AC-15 | US-10 | A case has been reassigned | The reassignment is completed | The previous owner, new owner, reason, user, date and time are retained in the history |
| AC-16 | US-10 | Reassignments exceed the approved threshold | The case is viewed or monitored | The solution displays the approved exception or attention indicator |

## Case work and monitoring

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-17 | US-11 | An authorised user opens an active case | The case summary is displayed | The stage, status, priority, owner and key dates are visible together |
| AC-18 | US-12 | An authorised user is working on a case | The user creates a task | The task is linked to the case and records its owner, status and due date |
| AC-19 | US-12 | A task has been completed | The authorised user marks it complete | The completion date and completing user are recorded |
| AC-20 | US-13 | A case or task meets an approved alert condition | The monitoring process runs | The appropriate user or team receives a visible alert containing sufficient information to act |
| AC-21 | US-13 | An alert condition is resolved | The case or task is updated | The alert is cleared or marked resolved without removing its history |
| AC-22 | US-14 | An authorised user records a material note, activity or decision | The entry is saved | It is added to the chronological case history with the user, date and time |
| AC-23 | US-14 | A standard user views the case history | The history is displayed | Protected historical entries cannot be silently altered or deleted |
| AC-24 | US-15 | A case is ready to transfer between stages or teams | The user initiates the handover | The solution checks that all approved handover information is present |
| AC-25 | US-15 | Required handover information is missing | The user attempts to complete the transfer | The solution identifies the missing information and prevents transfer unless an authorised exception is recorded |

## Communications and documents

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-26 | US-16 | An authorised user records a communication | The entry is saved | The communication type, participant, direction, date and related case are recorded |
| AC-27 | US-16 | An authorised user adds a document | The upload or link is completed | The document is associated with the correct case and visible only to authorised users |
| AC-28 | US-17 | An approved template is available | A user prepares the relevant communication | The solution applies the current approved template and allows authorised review before sending |
| AC-29 | US-18 | Approved communication preferences or accessibility requirements are recorded | A user prepares a communication | The relevant requirements are clearly displayed to the user |
| AC-30 | US-19 | A user does not have permission to access restricted information | The user attempts to view it | Access is denied and handled according to the approved security rules |
| AC-31 | US-19 | An authorised user accesses restricted information | The information is viewed or changed | The access or material change is recorded according to the approved audit rules |

## Outcome and closure

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-32 | US-20 | Required outcome or closure information is incomplete | A user attempts to close the case | The solution identifies the missing information and prevents closure |
| AC-33 | US-20 | All approved closure conditions are satisfied | An authorised user confirms closure | The case is closed with its outcome, closure reason, user, date and time recorded |
| AC-34 | US-21 | A closed case requires further action | An authorised user initiates reopening | The solution requires a reopening reason before changing the case status |
| AC-35 | US-21 | A case has been reopened | The user views its history | The original closure details and the reopening details remain visible and unchanged |

## Oversight, reporting and administration

| AC ID | Story | Given | When | Then |
|---|---|---|---|---|
| AC-36 | US-22 | A team leader has permission to view operational information | The user opens the approved management view | Workload, ageing, priority, stage and exception information is displayed using approved definitions |
| AC-37 | US-23 | The same approved data and reporting period are used | A report is generated more than once | The report produces consistent and reconcilable results |
| AC-38 | US-23 | A reporting user views a measure | The measure information is requested | Its approved definition, reporting period and relevant limitations are available |
| AC-39 | US-24 | An authorised user identifies a process exception | The user records it | The exception receives a category, status, owner and creation date |
| AC-40 | US-24 | An exception has been resolved | The authorised user closes it | The resolution action, user and date are retained |
| AC-41 | US-25 | An authorised administrator changes an approved configurable item | The change is submitted | The solution records the previous value, new value, approver and effective date |
| AC-42 | US-25 | A configuration change has not received required approval | An activation is attempted | The solution prevents the change from becoming effective |
| AC-43 | US-26 | A reviewer has the required permission | The reviewer searches the audit history | Relevant material actions can be identified by case, user, action and date range |
| AC-44 | US-26 | A standard user attempts to alter an audit record | The action is submitted | The solution denies the action |

## Acceptance-criteria quality checks

Before approval, each criterion must be reviewed to confirm that it is:

- clear and unambiguous;
- independently testable;
- traceable to a user story and requirement;
- based on an approved business rule;
- free from unconfirmed internal-process assumptions; and
- supported by agreed test data and user permissions.