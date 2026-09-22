# Non-Functional Requirements

## Purpose

This document defines the proposed quality, security and operational characteristics of the complaint-management solution.

Exact service levels, technical standards and performance thresholds must be confirmed with authorised business, technology, privacy, security and accessibility stakeholders.

## Security and privacy

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-01 | Access to case information must be controlled according to approved user roles and responsibilities. | Role-access testing confirms that users can access only authorised functions and information. | Must | BR-09 |
| NFR-02 | Users must be securely authenticated before accessing the solution. | Authentication controls pass security testing against the approved standard. | Must | BR-09 |
| NFR-03 | Sensitive information must be protected during transmission and storage using approved security controls. | Security review confirms compliance with approved encryption and information-protection standards. | Must | BR-09 |
| NFR-04 | The solution must prevent unauthorised modification or deletion of protected case records. | Permission and negative-access tests confirm that restricted actions are blocked. | Must | BR-07, BR-09 |
| NFR-05 | The solution must support approved information-retention and disposal rules. | Retention tests confirm that records are retained, archived or disposed of according to approved rules. | Must | BR-09 |
| NFR-06 | Sensitive information displayed in reports, exports and notifications must be limited to authorised business need. | Privacy review confirms that unnecessary sensitive data is excluded or appropriately protected. | Must | BR-09 |

## Auditability and data integrity

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-07 | Audit records must identify the relevant user, action, date and time for material case changes. | Audit testing confirms that selected case actions produce complete records. | Must | BR-07 |
| NFR-08 | Audit records must be protected from unauthorised alteration. | Security testing confirms that standard users cannot amend or remove audit entries. | Must | BR-07, BR-09 |
| NFR-09 | The solution must preserve the accuracy and consistency of case information across approved functions and integrations. | Reconciliation and integrity tests identify no unexplained loss, duplication or alteration of test data. | Must | BR-01, BR-11 |
| NFR-10 | Approved reporting measures must produce repeatable results from the same source data and reporting period. | Repeated report execution returns consistent results and reconciles to approved source totals. | Must | BR-11 |

## Accessibility and usability

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-11 | Core case-management functions must be usable with keyboard navigation and supported assistive technologies. | Accessibility testing is completed with representative workflows and approved assistive technologies. | Must | BR-10 |
| NFR-12 | Information must not rely on colour alone to communicate status, priority, warnings or errors. | Visual and accessibility review confirms the use of labels, text or other non-colour indicators. | Must | BR-10 |
| NFR-13 | User interfaces and generated communications must meet the organisation’s approved accessibility standard. | Formal assessment confirms conformance with the approved standard; WCAG 2.2 Level AA is the proposed baseline for validation. | Must | BR-10 |
| NFR-14 | Validation messages must identify the affected field and explain the corrective action required. | Usability testing confirms that users can understand and correct representative errors. | Must | BR-01, BR-10 |
| NFR-15 | Common case-management tasks should use consistent terminology, navigation and interaction patterns. | Representative users complete agreed tasks during usability testing without material navigation issues. | Should | BR-01, BR-10 |

## Performance, availability and recovery

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-16 | Core case searches, record retrieval and updates must complete within approved response-time targets under expected demand. | Performance testing confirms compliance with stakeholder-approved targets and workload assumptions. | Must | BR-02 |
| NFR-17 | The solution must support expected concurrent usage and data volumes without material degradation. | Load testing confirms acceptable performance against approved volume and concurrency assumptions. | Must | BR-02, BR-13 |
| NFR-18 | The solution must meet approved service-availability targets during required operating periods. | Service monitoring demonstrates compliance with the approved availability target. | Must | BR-01 |
| NFR-19 | Case information must be recoverable following an approved range of service failures. | Recovery testing meets approved recovery-time and recovery-point objectives. | Must | BR-01, BR-07 |
| NFR-20 | Failed transactions must not create unexplained duplicate, incomplete or inconsistent case records. | Failure and recovery tests confirm that transactions are completed, reversed or clearly flagged for resolution. | Must | BR-01, BR-07 |

## Maintainability and support

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-21 | Approved business rules, categories and templates should be configurable without modifying core application code. | Configuration testing confirms that authorised administrators can maintain approved items through controlled functions. | Should | BR-12 |
| NFR-22 | Configuration changes must be version-controlled and traceable to an authorised approval. | Review confirms that change history, approver and effective date are recorded. | Must | BR-07, BR-12 |
| NFR-23 | System errors must be logged with enough information for authorised support personnel to investigate them. | Support testing confirms that representative failures create useful diagnostic records without exposing unnecessary sensitive data. | Must | BR-08, BR-09 |
| NFR-24 | The solution must support monitoring of service health, failed integrations and unsuccessful automated actions. | Operational testing confirms that approved failures generate visible monitoring events or alerts. | Must | BR-08 |
| NFR-25 | Technical and user documentation must be maintained for implemented functions, controls and support procedures. | Documentation review confirms that approved materials are complete and current before release. | Should | BR-01, BR-12 |

## Compatibility and integration

| ID | Non-functional requirement | Proposed verification | Priority | Related business requirement |
|---|---|---|---|---|
| NFR-26 | The solution must operate on the organisation’s approved devices, browsers and technology environment. | Compatibility testing passes across the approved environment matrix. | Must | BR-01 |
| NFR-27 | Data exchanged with approved systems must use controlled formats, validation and error handling. | Integration testing confirms successful processing and appropriate handling of invalid or unavailable data. | Must | BR-01, BR-07 |
| NFR-28 | Interfaces must avoid exposing more case information than required for their approved purpose. | Interface and privacy reviews confirm adherence to data-minimisation requirements. | Must | BR-09 |

## Items requiring stakeholder approval

The following values have intentionally not been invented for this case study:

- response-time targets;
- concurrent-user and transaction-volume assumptions;
- availability percentage and operating hours;
- recovery-time and recovery-point objectives;
- retention and disposal periods;
- approved authentication and encryption standards;
- supported browsers, devices and assistive technologies;
- accessibility conformance standard;
- monitoring and support response targets; and
- integration protocols and dependent systems.