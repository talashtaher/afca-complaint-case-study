# Success Measures

## Purpose

This document proposes measures for evaluating whether the complaint-management change achieves its intended outcomes.

No baseline or target has been invented. Each measure requires an approved definition, reliable data source, accountable owner and agreed target before it can be used for performance assessment.

## Measurement principles

Success measures should:

- connect directly to an approved business requirement;
- balance speed, quality, fairness, control and user experience;
- avoid treating recommendation acceptance as evidence of decision quality;
- distinguish process performance from individual employee performance;
- use clearly defined populations and reporting periods;
- state known data limitations;
- protect personal and sensitive information; and
- be reviewed for unintended behavioural effects.

## Proposed measures

| ID | Measure | Proposed calculation or assessment | Intended insight | Frequency | Related requirements |
|---|---|---|---|---|---|
| SM-01 | Complete case creation rate | Cases created with all approved mandatory information ÷ cases created | Whether required information is captured at intake | Weekly or monthly | BR-01 |
| SM-02 | Unowned active cases | Count of active cases without a valid current owner | Whether accountability is consistently established | Daily or weekly | BR-04 |
| SM-03 | Cases visible by stage and status | Percentage of active cases with valid stage and status values | Reliability of operational visibility | Weekly | BR-02 |
| SM-04 | Triage-review completion | Cases with completed human triage review ÷ cases requiring review | Whether human confirmation controls are operating | Weekly or monthly | BR-03, BR-06 |
| SM-05 | Priority override rate | Confirmed priority overrides ÷ priority recommendations | Whether recommendations frequently require adjustment | Monthly | BR-03, BR-06 |
| SM-06 | Allocation override rate | Allocation overrides ÷ allocation recommendations | Whether allocation recommendations remain operationally appropriate | Monthly | BR-05, BR-06 |
| SM-07 | Reassignment frequency | Reassignment events by case, category or stage | Whether ownership is stable or repeatedly transferred | Monthly | BR-04, BR-08 |
| SM-08 | Due-task completion | Tasks completed by their approved due date ÷ completed tasks with due dates | Whether planned case work is completed when expected | Weekly or monthly | BR-08 |
| SM-09 | Unresolved alerts | Count and ageing of active alerts | Whether attention conditions are being addressed | Daily or weekly | BR-08 |
| SM-10 | Open exceptions | Count and ageing of unresolved process exceptions by category | Where the standard process requires intervention | Weekly or monthly | BR-08 |
| SM-11 | Complete handover rate | Handovers completed with all approved required information ÷ total handovers | Whether cases transfer with usable information | Monthly | BR-01, BR-04 |
| SM-12 | Closure-validation failure rate | Closure attempts blocked for missing approved information ÷ closure attempts | Whether required closure information is commonly absent | Monthly | BR-01, BR-11 |
| SM-13 | Reopened-case rate | Reopened cases ÷ closed cases for the approved population and period | Whether closure may require further action | Monthly | BR-07 |
| SM-14 | Duplicate-review outcome | Potential matches confirmed, rejected or linked by outcome | Whether duplicate rules are useful and appropriately reviewed | Monthly | BR-01, BR-14 |
| SM-15 | Data-quality exceptions | Count and rate of records failing approved data-quality rules | Reliability of operational and reporting information | Weekly or monthly | BR-01, BR-11 |
| SM-16 | Report reconciliation | Difference between approved report totals and authoritative source totals | Reliability and repeatability of management reporting | Each reporting cycle | BR-11 |
| SM-17 | Unauthorised-access attempts | Count of denied or suspicious access events requiring review | Whether access controls may require investigation | According to security procedure | BR-09 |
| SM-18 | Audit completeness | Sampled material events containing the required user, action, date and time | Whether accountability records are complete | Monthly or quarterly | BR-07 |
| SM-19 | Accessibility acceptance | Representative workflows passing the approved accessibility assessment | Whether core functions support accessible use | Before release and after material change | BR-10 |
| SM-20 | Training completion | Users completing required role-based training ÷ users assigned training | Organisational readiness before release | Before each phase |
| SM-21 | User adoption | Approved core transactions completed through the intended process | Whether the solution is being used as designed | Weekly during transition |
| SM-22 | User confidence | Structured feedback on clarity, efficiency and decision support | Whether users understand and can operate the process | During UAT and after release |
| SM-23 | Support demand | Volume and themes of support requests after release | Areas requiring additional guidance or improvement | Daily during enhanced support |
| SM-24 | Rule-change traceability | Activated rule changes with complete approval and version history ÷ activated changes | Effectiveness of configuration governance | Each change cycle | BR-07, BR-12 |

## Baseline and target process

Before assigning targets:

1. confirm the measure definition and intended behaviour;
2. identify the authoritative data source;
3. assess current data quality;
4. establish a representative baseline where possible;
5. identify seasonal or volume effects;
6. agree the target and tolerance;
7. assign an accountable owner;
8. confirm reporting frequency and access;
9. document exclusions and limitations; and
10. review whether the measure could encourage unintended behaviour.

## Balanced interpretation

Measures must be interpreted together. For example:

- a lower override rate is not automatically positive if users are accepting unsuitable recommendations;
- faster task completion is not automatically positive if case quality declines;
- fewer alerts may indicate improvement or ineffective alert rules;
- fewer reopened cases may indicate better closure or barriers to reopening; and
- higher throughput must not be evaluated without quality, fairness and control measures.

## Public-data limitation

The aggregated AFCA public data used in this case study cannot establish internal baselines for:

- case ageing;
- ownership;
- individual or team productivity;
- service-level performance;
- backlog;
- recommendation quality;
- allocation fairness; or
- true case-level conversion and resolution rates.

These measures require validated internal case-level data.

## Review and governance

Success measures should be reviewed:

- before implementation;
- after each phased release;
- during the post-implementation review;
- when business rules or definitions change;
- when data-quality issues are identified; and
- when a measure produces unintended operational behaviour.