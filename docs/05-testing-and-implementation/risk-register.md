# Implementation Risk Register

## Purpose

This register identifies risks that may affect the proposed complaint-management change.

The ratings and owners are preliminary. They demonstrate a structured risk-assessment approach and require validation through the organisation’s approved risk-management process.

## Rating approach

- **Likelihood:** Low, Medium or High
- **Impact:** Low, Medium or High
- **Overall rating:** Preliminary judgement based on likelihood and impact
- **Status:** Proposed, Open, Monitoring, Treated or Closed

No numerical scoring model has been assumed.

## Risk register

| ID | Risk | Likelihood | Impact | Overall rating | Proposed treatment | Proposed owner | Trigger or indicator | Status |
|---|---|---|---|---|---|---|---|---|
| R-01 | Requirements are implemented before sufficient stakeholder validation | Medium | High | High | Establish requirement owners, walkthroughs, approval points and controlled baselines | Business lead | Conflicting interpretations or repeated requirement changes | Proposed |
| R-02 | Triage or priority rules produce inconsistent or unfair recommendations | Medium | High | High | Validate rules with representative scenarios, retain human confirmation and monitor overrides | Process and governance lead | High override rates or unexplained outcome differences | Proposed |
| R-03 | Allocation recommendations distribute work inappropriately | Medium | High | High | Validate capability and workload factors, permit controlled overrides and review allocation patterns | Operational lead | Repeated reassignment or concentrated workload | Proposed |
| R-04 | Users treat recommendations as mandatory decisions | Medium | High | High | Use clear interface language, training and controls that preserve human accountability | Change and process lead | Users cannot explain decisions beyond the recommendation | Proposed |
| R-05 | Sensitive complaint information is accessed or disclosed inappropriately | Medium | High | High | Apply role-based access, data minimisation, audit monitoring and privacy review | Privacy and security lead | Unauthorised access attempts or excessive permissions | Proposed |
| R-06 | Data migration creates incomplete, duplicated or inaccurate case records | Medium | High | High | Profile source data, define reconciliation rules, test migration and retain rollback arrangements | Data and technology lead | Reconciliation differences or failed record validation | Proposed |
| R-07 | Integration failure interrupts case activity or creates inconsistent records | Medium | High | High | Define error handling, monitoring, reconciliation and manual continuity procedures | Technology lead | Failed messages, unavailable services or inconsistent updates | Proposed |
| R-08 | Incomplete business definitions produce unreliable management reports | Medium | High | High | Approve measure definitions, data ownership and reconciliation before report acceptance | Reporting and business lead | Different reports produce conflicting totals | Proposed |
| R-09 | Accessibility needs are identified too late | Medium | High | High | Include accessibility in design reviews, test planning and representative UAT | Accessibility and change lead | Core workflows fail keyboard or assistive-technology testing | Proposed |
| R-10 | Users are not prepared for changed roles, controls or workflows | Medium | High | High | Complete change-impact assessment, role-based training, communications and readiness checks | Change lead | Low training completion or high early support demand | Proposed |
| R-11 | Poor-quality or incomplete test data leaves important scenarios untested | Medium | Medium | Medium | Define representative synthetic data covering standard, sensitive and exception scenarios | UAT lead | Scenarios blocked or important conditions absent from test data | Proposed |
| R-12 | Critical defects remain unresolved near release | Medium | High | High | Apply entry and exit criteria, defect triage, regression testing and release-governance decisions | UAT and delivery leads | Critical or high defects remain open at decision point | Proposed |
| R-13 | Configurable rules change without appropriate approval | Low | High | Medium | Apply role restrictions, approval workflow, version history and effective dates | Business-rule owner | Unauthorised or unexplained rule changes | Proposed |
| R-14 | Alert volumes become excessive and are ignored | Medium | Medium | Medium | Validate alert thresholds, assign ownership and monitor repeated or unresolved alerts | Operational lead | Large volumes of dismissed or overdue alerts | Proposed |
| R-15 | Historical or audit information can be altered or cannot be retrieved | Low | High | Medium | Protect audit records, test search and retention, and restrict modification permissions | Security and records lead | Missing events or unauthorised alteration attempts | Proposed |
| R-16 | Delivery scope expands beyond agreed business outcomes | Medium | Medium | Medium | Maintain scope boundaries, backlog priorities and formal change control | Business sponsor or delegate | Unplanned features enter delivery without trade-off decisions | Proposed |
| R-17 | Phased implementation creates inconsistent processes across teams | Medium | Medium | Medium | Define transition procedures, interim ownership and clear entry criteria for each phase | Implementation lead | Different teams apply conflicting processes or definitions | Proposed |
| R-18 | Early operational performance is disrupted after release | Medium | High | High | Use phased deployment, enhanced support, monitoring and rollback or contingency arrangements | Implementation and operational leads | Increased errors, unresolved cases or support demand | Proposed |
| R-19 | Retention, archival or disposal rules are not confirmed before implementation | Medium | High | High | Obtain records and privacy decisions before migration and production use | Records and privacy lead | Unclear treatment of historical or closed records | Proposed |
| R-20 | Success measures encourage unintended behaviour or cannot be calculated reliably | Medium | Medium | Medium | Use balanced measures, document limitations and review behavioural effects | Business and reporting lead | Users optimise a measure at the expense of service quality | Proposed |

## Risk-review cadence

During a real implementation, the register should be reviewed:

- at requirement and design approval points;
- before UAT begins;
- at regular delivery-governance meetings;
- before each implementation phase;
- during enhanced post-release support; and
- when a material defect, incident or scope change occurs.

## Escalation considerations

A risk should be considered for escalation when:

- it may cause unacceptable harm, privacy exposure or loss of information;
- it threatens a critical business outcome or implementation decision;
- treatment actions are overdue or ineffective;
- the residual risk exceeds the authorised tolerance; or
- accountable owners cannot resolve the issue within their authority.

## Limitations

This register does not claim knowledge of AFCA’s internal risk appetite, controls, systems or accountabilities. Confirmed ratings, owners, tolerances and escalation routes require authorised stakeholder input.