# Proposed Solution Data Dictionary

## Purpose

This data dictionary defines the principal information proposed for the complaint-management solution.

It is a conceptual business artefact, not a physical database design. Field names, formats, mandatory rules, classifications and retention requirements must be validated with authorised business, data, privacy, security and technology stakeholders.

## Data-classification note

The classifications below are preliminary:

- **Operational** — process information with no intended personal content.
- **Personal** — information that identifies or relates to an individual.
- **Potentially sensitive** — information that may require additional protection depending on its content and context.
- **Security-controlled** — information used for access, monitoring or audit.

## Case record

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Case ID | Unique identifier assigned to the complaint case | Text or system-generated identifier | System | Operational | Must be unique and immutable |
| Case title | Short description used to identify the case | Text | Yes | Potentially sensitive | Must avoid unnecessary sensitive detail |
| Received date and time | Date and time the complaint was received | Date and time | Yes | Operational | Source and timezone must be defined |
| Receipt channel | Channel through which the complaint was received | Controlled list | Yes | Operational | Values require approval |
| Case stage | Current high-level process stage | Controlled list | Yes | Operational | Proposed examples: Registration and Referral, Case Management, Decision |
| Case status | Current operational state of the case | Controlled list | Yes | Operational | Must be distinguished from case stage |
| Case priority | Confirmed operational priority | Controlled list | Yes | Operational | Priority levels and criteria require approval |
| Priority reason | Explanation supporting the confirmed priority | Text or coded reason | Conditional | Potentially sensitive | Required when specified by the approved priority rules |
| Created by | User or process that created the case | User or system identifier | System | Security-controlled | Retained in audit history |
| Created date and time | Date and time the case record was created | Date and time | System | Operational | Must not be manually altered |
| Last updated by | User or process that last changed the case | User or system identifier | System | Security-controlled | Derived from the latest material change |
| Last updated date and time | Date and time of the latest material change | Date and time | System | Operational | Must be system generated |

## Participants and communication needs

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Participant ID | Unique identifier for a person or organisation associated with a case | Identifier | System | Personal | Matching rules require validation |
| Participant role | Relationship of the participant to the case | Controlled list | Yes | Operational | Examples require stakeholder approval |
| Participant name | Name of the person or organisation | Text | Yes | Personal | Validation depends on participant type |
| Preferred contact method | Approved channel for contacting the participant | Controlled list | Conditional | Personal | Must be used where operationally appropriate |
| Contact details | Details required for approved communication | Structured text | Conditional | Personal | Access must be restricted |
| Communication accessibility requirement | Requirement affecting how communication should be prepared or delivered | Controlled value and notes | Conditional | Potentially sensitive | Must be visible only where required for service delivery |
| Representative indicator | Identifies whether an authorised representative is involved | Boolean | Conditional | Personal | Authority requirements must be confirmed |
| Representative authority status | Status of evidence authorising the representative | Controlled list | Conditional | Potentially sensitive | Must not imply authority unless confirmed |

## Classification and triage

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Complaint category | Approved primary classification of the complaint | Controlled list | Yes | Operational | Taxonomy requires stakeholder approval |
| Product or service category | Product or service associated with the complaint | Controlled list | Conditional | Operational | Must use governed reference data |
| Complexity indicator | Approved indication of expected case complexity | Controlled list | Conditional | Operational | Criteria require validation |
| Priority indicator | Approved factor relevant to priority assessment | Controlled list | Conditional | Potentially sensitive | Must trigger human review where required |
| Triage recommendation | Priority or pathway proposed by the approved rules | Controlled list | Conditional | Operational | Must not determine complaint merit or outcome |
| Triage explanation | Factors and rules contributing to the recommendation | Structured text | Conditional | Potentially sensitive | Must be understandable to an authorised reviewer |
| Triage rule version | Version of the rules used for the recommendation | Version identifier | System | Operational | Required for reproducibility and audit |
| Confirmed by | User who confirmed or amended the recommendation | User identifier | Conditional | Security-controlled | Required before approved progression |
| Override indicator | Identifies whether the recommendation was changed | Boolean | System | Operational | Derived from recommendation and confirmed result |
| Override reason | Reason an authorised user changed a recommendation | Controlled reason and notes | Conditional | Potentially sensitive | Required when an override occurs |

## Ownership and allocation

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Accountable team | Team currently accountable for the case | Controlled reference | Yes | Operational | Confirmed organisational values required |
| Case owner | User currently responsible for coordinating the case | User identifier | Yes for active cases | Security-controlled | Eligibility rules require approval |
| Allocation recommendation | Proposed owner or team generated by approved rules | Reference identifier | Conditional | Operational | Must remain a recommendation |
| Allocation explanation | Criteria contributing to the allocation recommendation | Structured text | Conditional | Operational | Must support authorised review |
| Allocation date and time | Date and time ownership was assigned | Date and time | System | Operational | Recorded for each allocation event |
| Reassignment reason | Reason ownership was changed | Controlled reason and notes | Conditional | Potentially sensitive | Required for reassignment |
| Previous owner | Owner immediately before reassignment | User identifier | Conditional | Security-controlled | Retained in allocation history |

## Tasks, monitoring and exceptions

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Task ID | Unique identifier for a case task | Identifier | System | Operational | Unique within the solution |
| Task description | Description of required case work | Text | Yes | Potentially sensitive | Must be linked to a case |
| Task owner | User or team responsible for the task | Reference identifier | Yes | Security-controlled | Eligibility rules require approval |
| Task status | Current state of the task | Controlled list | Yes | Operational | Approved status values required |
| Task due date | Date by which the task should be completed | Date or date and time | Conditional | Operational | Calculation rules require approval |
| Alert type | Category of attention or escalation alert | Controlled list | Conditional | Operational | Trigger rules require approval |
| Alert status | Current state of the alert | Controlled list | Conditional | Operational | Must preserve resolved-alert history |
| Exception ID | Unique identifier assigned to a process exception | Identifier | System | Operational | Must link to the relevant case or process event |
| Exception category | Approved classification of the exception | Controlled list | Yes for exceptions | Operational | Based on the exception-handling framework |
| Exception owner | User or team responsible for resolving the exception | Reference identifier | Yes for open exceptions | Security-controlled | Must remain visible until resolved |
| Exception resolution | Action taken to resolve the exception | Text or controlled reason | Conditional | Potentially sensitive | Required before exception closure |

## Communications, documents and history

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Communication ID | Unique identifier for a recorded communication | Identifier | System | Operational | Must link to the relevant case |
| Communication direction | Whether the communication was incoming or outgoing | Controlled list | Yes | Operational | Values require approval |
| Communication type | Channel or form of communication | Controlled list | Yes | Operational | Examples may include email, telephone or letter |
| Communication date and time | Date and time the communication occurred | Date and time | Yes | Operational | May differ from record-creation time |
| Communication summary | Business summary of the communication | Text | Yes | Potentially sensitive | Access and content standards require validation |
| Document ID | Unique identifier for a linked document | Identifier | System | Operational | Must link to the correct case |
| Document type | Approved classification of the document | Controlled list | Yes | Operational | Taxonomy and access rules require approval |
| Document sensitivity | Protection level applying to the document | Controlled list | Yes | Potentially sensitive | Determines authorised access |
| Case-history event | Material action or change recorded against the case | Structured record | System | Potentially sensitive | Must identify action, user, date and time |

## Outcome and closure

| Field | Definition | Proposed type or example | Required? | Proposed classification | Rules or notes |
|---|---|---|---|---|---|
| Outcome category | Approved classification of the case outcome | Controlled list | Required at closure | Potentially sensitive | Must not be inferred automatically |
| Outcome date | Date the outcome was confirmed | Date | Required at closure | Operational | Definition requires approval |
| Closure reason | Approved reason the case was closed | Controlled list | Required at closure | Operational | Must support consistent reporting |
| Closure date and time | Date and time the case was formally closed | Date and time | System | Operational | Created only after closure validation |
| Closed by | Authorised user who completed closure | User identifier | System | Security-controlled | Retained in audit history |
| Reopened indicator | Identifies whether a closed case has been reopened | Boolean | System | Operational | Must preserve original closure information |
| Reopening reason | Reason an authorised user reopened the case | Controlled reason and notes | Conditional | Potentially sensitive | Required when reopening occurs |

## Governance questions

The following matters require confirmation:

1. What information is mandatory at each process stage?
2. Which fields contain personal, sensitive or restricted information?
3. Which roles may create, view, update, export or delete each field?
4. Which taxonomies and reference-data values are already approved?
5. What validation, retention and disposal rules apply?
6. Which fields may be shared with external participants or systems?
7. Which events must create immutable audit records?
8. What data-quality rules and monitoring responsibilities are required?
9. Which system is the authoritative source for each data element?
10. What migration, archival and historical-data requirements apply?