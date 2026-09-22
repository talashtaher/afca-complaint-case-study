# Requirements Traceability Matrix

## Purpose

This matrix connects the proposed business requirements to supporting evidence, functional and non-functional requirements, user stories and acceptance criteria.

Traceability helps confirm that each proposed capability addresses an identified business need and that each user story can be verified through acceptance criteria.

All requirements remain subject to stakeholder validation.

## Traceability matrix

| Business requirement | Source or rationale | Functional requirements | Non-functional requirements | User stories | Acceptance criteria | Status |
|---|---|---|---|---|---|---|
| BR-01 — Maintain a consistent and controlled complaint-management process | `public-process-map.md`; `pain-point-register.md`; `future-state-process.md` | FR-01–FR-07, FR-18–FR-20, FR-24–FR-25, FR-31–FR-32 | NFR-09, NFR-14, NFR-18–NFR-20, NFR-25–NFR-27 | US-01–US-04, US-11–US-12, US-15, US-20 | AC-01–AC-07, AC-17–AC-19, AC-24–AC-25, AC-32–AC-33 | Proposed |
| BR-02 — Provide visibility of volumes, stages, ownership and workload | `findings.md`; `context-diagram.md`; `pain-point-register.md` | FR-18, FR-36 | NFR-16–NFR-17 | US-11, US-22 | AC-17, AC-36 | Proposed |
| BR-03 — Apply transparent and consistent assessment and priority criteria | `pain-point-register.md`; `decision-rules.md` | FR-07–FR-12 | NFR-07, NFR-10 | US-04–US-06 | AC-06–AC-10 | Proposed |
| BR-04 — Maintain clear ownership and accountability | `context-diagram.md`; `pain-point-register.md`; `future-state-process.md` | FR-13, FR-15–FR-16, FR-18–FR-20, FR-24 | NFR-07 | US-07, US-09, US-11–US-12, US-15 | AC-11–AC-12, AC-14–AC-15, AC-17–AC-19, AC-24 | Proposed |
| BR-05 — Consider capability, availability, workload and case needs during allocation | `design-principles.md`; `decision-rules.md` | FR-13–FR-14 | NFR-16–NFR-17 | US-07–US-08 | AC-11–AC-13 | Proposed |
| BR-06 — Preserve professional judgement through controlled overrides | `design-principles.md`; `decision-rules.md`; `solution-boundaries.md` | FR-04, FR-06, FR-10–FR-11, FR-14, FR-33 | NFR-07–NFR-08 | US-05, US-08, US-21 | AC-03, AC-05, AC-08–AC-09, AC-13, AC-34–AC-35 | Proposed |
| BR-07 — Maintain a traceable case history | `design-principles.md`; `exception-handling.md` | FR-11, FR-16, FR-22–FR-27, FR-33–FR-34, FR-39 | NFR-07–NFR-10, NFR-20, NFR-22 | US-08, US-10, US-14–US-16, US-21, US-26 | AC-13, AC-15, AC-22–AC-27, AC-34–AC-35, AC-41–AC-44 | Proposed |
| BR-08 — Identify cases and exceptions requiring attention | `pain-point-register.md`; `exception-handling.md` | FR-17, FR-20–FR-21, FR-25, FR-35–FR-36 | NFR-23–NFR-24 | US-10, US-13, US-15, US-22, US-24 | AC-16, AC-20–AC-21, AC-24–AC-25, AC-36, AC-39–AC-40 | Proposed |
| BR-09 — Protect complaint information | `design-principles.md`; `solution-boundaries.md` | FR-30, FR-40 | NFR-01–NFR-08, NFR-23, NFR-28 | US-19, US-26 | AC-30–AC-31, AC-43–AC-44 | Proposed |
| BR-10 — Support accessible and appropriate communication | `design-principles.md`; `exception-handling.md` | FR-12, FR-28–FR-29 | NFR-11–NFR-15 | US-06, US-17–US-18 | AC-10, AC-28–AC-29 | Proposed |
| BR-11 — Use consistently defined management measures | `findings.md`; `design-principles.md` | FR-31, FR-36–FR-37 | NFR-09–NFR-10 | US-20, US-22–US-23 | AC-32–AC-33, AC-36–AC-38 | Proposed |
| BR-12 — Maintain business rules through controlled governance | `decision-rules.md`; `design-principles.md` | FR-38–FR-39 | NFR-21–NFR-22, NFR-25 | US-25 | AC-41–AC-42 | Proposed |
| BR-13 — Identify changing demand, workload and exception patterns | `findings.md`; `pain-point-register.md` | FR-35–FR-37 | NFR-16–NFR-17, NFR-24 | US-22–US-24 | AC-36–AC-40 | Proposed |
| BR-14 — Capture information once and reuse it appropriately | `design-principles.md`; `future-state-process.md` | FR-05–FR-06, FR-28 | NFR-09, NFR-27 | US-03, US-17 | AC-04–AC-05, AC-28 | Proposed |

## Coverage summary

| Requirement type | Identifier range | Coverage |
|---|---|---|
| Business requirements | BR-01–BR-14 | All business requirements are represented in this matrix |
| Functional requirements | FR-01–FR-40 | All functional requirements trace to at least one business requirement |
| Non-functional requirements | NFR-01–NFR-28 | All non-functional requirements support one or more business requirements |
| User stories | US-01–US-26 | All user stories trace to proposed requirements |
| Acceptance criteria | AC-01–AC-44 | All user stories have associated acceptance criteria |

## Traceability status definitions

- **Proposed** — documented for the case study but not validated by authorised stakeholders.
- **Validated** — reviewed and accepted by an authorised stakeholder.
- **Approved** — formally authorised for delivery.
- **Implemented** — delivered in the target solution.
- **Verified** — successfully assessed against approved acceptance criteria.
- **Deferred** — intentionally postponed with an approved reason.
- **Removed** — withdrawn through an approved change decision.

Only **Proposed** is used in this case study because stakeholder approval has not occurred.

## Traceability controls

During a real delivery:

1. every requirement should have an identified source and accountable owner;
2. requirement changes should be recorded and approved;
3. removed or deferred requirements should retain their decision history;
4. user stories should not enter delivery without agreed acceptance criteria;
5. tests should reference the relevant acceptance-criteria identifiers;
6. defects should be traceable to the affected requirement or criterion; and
7. the matrix should be reviewed whenever scope, rules or priorities change.

## Current limitations

This matrix demonstrates proposed end-to-end traceability but does not represent formal AFCA approval.

Implementation components, test cases, defects, release identifiers and stakeholder approvals cannot be included until a delivery environment and governance process are confirmed.