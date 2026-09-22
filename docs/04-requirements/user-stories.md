# User Stories

## Purpose

These user stories translate the proposed requirements into user-centred needs. The role names are generic case-study personas and do not claim to represent AFCA’s confirmed internal job titles or structure.

Detailed acceptance criteria are maintained separately so that each story can be reviewed and tested consistently.

## Intake and triage

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-01 | As an intake user, I want to create a complaint case with a unique identifier so that it can be tracked throughout its lifecycle. | Must | BR-01; FR-01–FR-02 |
| US-02 | As an intake user, I want missing mandatory information to be clearly identified so that incomplete cases can be addressed before progressing. | Must | BR-01; FR-03–FR-04 |
| US-03 | As an intake user, I want to see potential duplicate or related cases so that repeated information can be reviewed and appropriately linked. | Must | BR-01, BR-14; FR-05–FR-06 |
| US-04 | As a triage user, I want a recommendation based on approved rules so that complaints can be assessed consistently. | Must | BR-03; FR-07–FR-09 |
| US-05 | As a triage user, I want to confirm or amend the recommended priority so that professional judgement remains part of the decision. | Must | BR-03, BR-06; FR-10–FR-12 |
| US-06 | As a triage user, I want priority or vulnerability indicators to trigger human review so that relevant circumstances receive appropriate consideration. | Must | BR-03, BR-10; FR-12 |

## Allocation and ownership

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-07 | As an allocation user, I want an allocation recommendation that considers approved capability, availability and workload criteria so that work can be distributed appropriately. | Must | BR-04, BR-05; FR-13 |
| US-08 | As an authorised user, I want to override an allocation recommendation with a recorded reason so that exceptional circumstances can be handled transparently. | Must | BR-06, BR-07; FR-14, FR-16 |
| US-09 | As a case worker, I want every active case to show its owner and accountable team so that responsibility is clear. | Must | BR-04; FR-15 |
| US-10 | As a team leader, I want to see reassignment history and repeated transfers so that ownership issues can be investigated. | Should | BR-07, BR-08; FR-16–FR-17 |

## Case work and monitoring

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-11 | As a case worker, I want to see the case stage, status, priority, owner and key dates together so that I can understand the case quickly. | Must | BR-02, BR-04; FR-18 |
| US-12 | As a case worker, I want to create and manage tasks with owners and due dates so that required work is visible and controlled. | Must | BR-01, BR-04; FR-19–FR-20 |
| US-13 | As a case worker, I want alerts for cases and tasks requiring attention so that important work is not overlooked. | Must | BR-08; FR-21 |
| US-14 | As a case worker, I want to record case notes, activities and decisions so that the case history is complete. | Must | BR-07; FR-22–FR-23 |
| US-15 | As a receiving user, I want a structured handover containing the required information so that I can continue the case without unnecessary rework. | Must | BR-01, BR-04; FR-24–FR-25 |

## Communications and documents

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-16 | As a case worker, I want communications and supporting documents linked to the relevant case so that the case record is complete and accessible to authorised users. | Must | BR-07; FR-26–FR-27 |
| US-17 | As a case worker, I want approved communication templates so that routine communications are prepared consistently. | Should | BR-10, BR-14; FR-28 |
| US-18 | As a case worker, I want to see a participant’s approved communication preferences and accessibility requirements so that communication can be appropriately adapted. | Must | BR-10; FR-29 |
| US-19 | As a privacy-conscious user, I want sensitive documents and communications restricted to authorised roles so that confidential information is protected. | Must | BR-09; FR-30, FR-40 |

## Outcome and closure

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-20 | As a case worker, I want the solution to check required outcome and closure information so that incomplete cases are not closed unintentionally. | Must | BR-01, BR-11; FR-31–FR-32 |
| US-21 | As an authorised user, I want to reopen a closed case with a recorded reason so that further action can occur without losing the original history. | Must | BR-06, BR-07; FR-33–FR-34 |

## Oversight and administration

| ID | User story | Priority | Related requirements |
|---|---|---|---|
| US-22 | As a team leader, I want to view workload, ageing, priority, stage and exceptions so that I can identify cases requiring attention. | Must | BR-02, BR-08; FR-36 |
| US-23 | As a reporting user, I want reports based on approved definitions so that management information is consistent and explainable. | Must | BR-11; FR-37 |
| US-24 | As an authorised user, I want to record and manage process exceptions so that unusual cases remain visible until resolved. | Must | BR-08; FR-35 |
| US-25 | As a business administrator, I want approved rules, categories and templates to be configurable so that controlled changes can be made without unnecessary redevelopment. | Should | BR-12; FR-38–FR-39 |
| US-26 | As a security or privacy reviewer, I want access and material changes to be traceable so that potential misuse or control failures can be investigated. | Must | BR-07, BR-09; FR-39–FR-40; NFR-01, NFR-07–NFR-08 |

## Validation notes

Before these stories are approved:

- persona names must be replaced or mapped to confirmed organisational roles;
- story priorities must be reviewed with authorised stakeholders;
- workflow permissions and approval responsibilities must be confirmed;
- applicable privacy, accessibility and records-management obligations must be validated; and
- each story must have approved, testable acceptance criteria.