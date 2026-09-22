# Business Requirements

## Purpose

This document defines the business outcomes required from the proposed complaint-management solution.

The requirements are based on the public-data analysis, current-state risk hypotheses and future-state design. They are proposed requirements for the case study and would require validation with authorised stakeholders before implementation.

## Business requirements

| ID | Business requirement | Business value | Evidence or rationale | Priority |
|---|---|---|---|---|
| BR-01 | The organisation must maintain a consistent and controlled complaint-management process from receipt to closure. | Supports reliable case handling and reduces process variation. | Current-state process analysis and future-state design principles. | Must |
| BR-02 | Operational teams must have timely visibility of complaint volumes, case stages, ownership and workload. | Supports planning, allocation and management oversight. | Public data shows sustained monthly demand and meaningful volume variation. | Must |
| BR-03 | Complaints must be assessed and prioritised using transparent and consistently applied criteria. | Supports fair treatment and timely attention to higher-priority cases. | Current-state triage risk hypothesis and future-state decision rules. | Must |
| BR-04 | Every active complaint must have a clearly identified owner and accountable team. | Reduces uncertainty, unowned work and avoidable handover delays. | Current-state ownership and allocation risk hypotheses. | Must |
| BR-05 | Allocation decisions must consider relevant capability, availability, workload and case requirements. | Supports fair and practical distribution of work. | Future-state allocation design. | Must |
| BR-06 | Authorised users must be able to exercise professional judgement and override system recommendations with a recorded reason. | Preserves human accountability while maintaining transparency. | Future-state human-judgement and auditability principles. | Must |
| BR-07 | Case activities, decisions, communications, documents and changes must be traceable through a reliable history. | Supports accountability, review and audit. | Future-state auditability principle and current-state traceability risk hypothesis. | Must |
| BR-08 | Cases requiring attention must be identifiable through due dates, alerts and exception monitoring. | Supports timely intervention and reduces the risk of overlooked work. | Current-state monitoring risk hypothesis and future-state exception design. | Must |
| BR-09 | Complaint information must be protected through appropriate access controls, privacy safeguards and audit records. | Protects sensitive information and supports governance obligations. | Future-state privacy and security principles. | Must |
| BR-10 | The solution must support accessible and appropriate communication with complainants and other participants. | Supports inclusive service delivery and clear case communication. | Future-state accessibility principle and exception handling design. | Must |
| BR-11 | Management reporting must use clear and consistently defined measures. | Supports reliable oversight and reduces misinterpretation of operational data. | Public-data limitations and future-state reporting principle. | Must |
| BR-12 | Business rules and decision criteria must be maintainable through controlled governance. | Allows the process to adapt while preserving consistency and accountability. | Future-state maintainability principle and decision-rules framework. | Should |
| BR-13 | The organisation should be able to identify changes in demand, workload and exception patterns. | Supports capacity planning and early operational response. | Public-data analysis identified sustained demand and monthly variation. | Should |
| BR-14 | Information should be captured once and reused where authorised and appropriate. | Reduces repeated entry and improves consistency across the case lifecycle. | Future-state capture-once design principle. | Should |

## Prioritisation method

Priorities use the MoSCoW method:

- **Must** — required for the proposed solution to meet its core business purpose.
- **Should** — important but may be delivered after the core capability if necessary.
- **Could** — beneficial but not essential to the initial solution.
- **Won't for now** — explicitly excluded from the current delivery scope.

These priorities are preliminary and require stakeholder validation.

## Validation questions

The following matters must be confirmed during stakeholder engagement:

1. Which business outcomes are mandatory for the initial release?
2. Which roles are accountable for complaint ownership, priority and allocation?
3. What approved criteria determine complaint priority?
4. What workload and capability information may be used for allocation?
5. Which events require alerts, escalation or management review?
6. What reporting measures and definitions are currently approved?
7. What privacy, retention, accessibility and audit obligations apply?
8. Which business rules may be configured, and who may approve changes?
9. How should success against these requirements be measured?