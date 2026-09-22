# Functional Requirements

## Purpose

This document defines the proposed functions required to support the future-state complaint-management process.

These requirements describe required capabilities rather than a specific technology or product. They require validation with authorised stakeholders before implementation.

## Case creation and validation

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-01 | The solution must create a unique case record for each complaint. | Must | BR-01 |
| FR-02 | The solution must capture the mandatory information defined in the approved data dictionary. | Must | BR-01 |
| FR-03 | The solution must identify missing mandatory information before a case progresses. | Must | BR-01 |
| FR-04 | The solution must allow an authorised user to record why incomplete information has been accepted. | Must | BR-06, BR-07 |
| FR-05 | The solution must warn users about potential duplicate or related cases using approved matching criteria. | Must | BR-01, BR-14 |
| FR-06 | The solution must allow an authorised user to confirm, reject or link a potential duplicate. | Must | BR-06, BR-07 |

## Classification, triage and priority

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-07 | The solution must support complaint classification using approved categories. | Must | BR-01, BR-03 |
| FR-08 | The solution must generate a triage recommendation using approved and explainable rules. | Must | BR-03 |
| FR-09 | The solution must display the factors contributing to a triage recommendation. | Must | BR-03, BR-06 |
| FR-10 | An authorised user must confirm or amend the recommended priority before allocation. | Must | BR-03, BR-06 |
| FR-11 | The solution must record the user, date, time and reason when a recommendation is overridden. | Must | BR-06, BR-07 |
| FR-12 | The solution must flag cases containing approved priority or vulnerability indicators for human review. | Must | BR-03, BR-10 |

## Allocation and ownership

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-13 | The solution must generate an allocation recommendation using approved capability, availability and workload criteria. | Must | BR-04, BR-05 |
| FR-14 | An authorised user must be able to accept or override an allocation recommendation. | Must | BR-06 |
| FR-15 | The solution must record the current case owner and accountable team. | Must | BR-04 |
| FR-16 | The solution must record allocation and reassignment history, including reasons for change. | Must | BR-07 |
| FR-17 | The solution should identify cases that have been reassigned more often than an approved threshold. | Should | BR-08 |

## Case management and monitoring

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-18 | The solution must display the current case stage, status, priority, owner and key dates. | Must | BR-02, BR-04 |
| FR-19 | Authorised users must be able to create, assign, update and complete case tasks. | Must | BR-01, BR-04 |
| FR-20 | The solution must support due dates for cases and tasks. | Must | BR-08 |
| FR-21 | The solution must generate alerts when approved monitoring or escalation conditions are met. | Must | BR-08 |
| FR-22 | Authorised users must be able to record case notes, activities and decisions. | Must | BR-07 |
| FR-23 | The solution must maintain a chronological history of material case events and changes. | Must | BR-07 |
| FR-24 | The solution must support a structured handover when a complaint progresses between stages or teams. | Must | BR-01, BR-04 |
| FR-25 | The solution must identify incomplete handover information before responsibility is transferred. | Must | BR-01, BR-08 |

## Communications and documents

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-26 | Authorised users must be able to record incoming and outgoing case communications. | Must | BR-07 |
| FR-27 | The solution must associate relevant documents and evidence with the correct case. | Must | BR-07 |
| FR-28 | The solution should support approved communication templates. | Should | BR-10, BR-14 |
| FR-29 | The solution must record communication preferences and approved accessibility requirements. | Must | BR-10 |
| FR-30 | The solution must restrict access to sensitive communications and documents according to authorised roles. | Must | BR-09 |

## Outcomes and closure

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-31 | The solution must require an approved outcome and closure reason before a case is closed. | Must | BR-01, BR-11 |
| FR-32 | The solution must perform approved closure-validation checks before final closure. | Must | BR-01, BR-07 |
| FR-33 | An authorised user must be able to reopen a case with a recorded reason. | Must | BR-06, BR-07 |
| FR-34 | The solution must preserve the original closure information when a case is reopened. | Must | BR-07 |

## Exceptions, reporting and administration

| ID | Functional requirement | Priority | Related business requirement |
|---|---|---|---|
| FR-35 | The solution must allow authorised users to record, classify, assign and resolve process exceptions. | Must | BR-08 |
| FR-36 | The solution must provide authorised users with views of workload, case stage, priority, ageing and exceptions. | Must | BR-02, BR-08 |
| FR-37 | The solution must produce reports using approved measures and definitions. | Must | BR-11 |
| FR-38 | Authorised administrators must be able to maintain configurable business rules through a controlled process. | Should | BR-12 |
| FR-39 | The solution must record changes to business rules, including approver and effective date. | Must | BR-07, BR-12 |
| FR-40 | The solution must support role-based access to case functions and information. | Must | BR-09 |

## Assumptions and validation needs

- Mandatory fields and approved classifications have not yet been confirmed.
- Priority indicators and thresholds require authorised stakeholder approval.
- Allocation criteria and eligible ownership groups require validation.
- Alert and escalation conditions require validation.
- Reporting definitions must be agreed before implementation.
- Access roles, sensitive-data categories and retention rules require privacy and security review.
- Integration requirements will depend on the confirmed technology environment.