# Future-state design principles

## Purpose

These principles guide the proposed future-state complaint-management process and solution requirements.

They respond to the project objective of improving case visibility, monitoring, allocation and triage while protecting fairness, security and consistency during periods of high complaint demand.

The principles are design choices for this case study. They are not presented as confirmed AFCA policy.

## Design principles

| ID | Principle | Why it matters | Future-state design response |
|---|---|---|---|
| DP-01 | Human judgement remains accountable | Complaint circumstances can be complex and may not be suitable for fully automated decisions | Automation should support classification, reminders and recommendations, while authorised users remain responsible for material decisions |
| DP-02 | Fairness must be visible and explainable | Triage, priority and allocation decisions can affect how complaints are handled | Rules, overrides and allocation decisions should be recorded with clear reasons and available for review |
| DP-03 | Every case has clear ownership | Unclear ownership can lead to missed actions, repeated follow-up and delayed progression | Each active case should have an identifiable owner or responsible queue, with controlled reassignment and history |
| DP-04 | Status information should support action | A status label alone may not explain what needs to happen next | The case view should show current stage, status, next action, responsible party, due date and blocking issue |
| DP-05 | Triage should be consistent but adaptable | Standard rules improve consistency, but unusual or sensitive complaints may require different handling | The solution should apply documented triage rules while allowing authorised users to override recommendations with a recorded reason |
| DP-06 | Allocation should consider more than availability | Equal case counts do not necessarily represent equal workloads | Allocation should consider workload, complaint complexity, priority and relevant capability, subject to validation of business rules |
| DP-07 | Exceptions should be made visible early | Urgent, vulnerable, overdue or blocked cases may require prompt attention | Exception indicators, alerts and escalation paths should be available without relying only on manual monitoring |
| DP-08 | Privacy and security should be built into the process | Complaint records may contain sensitive personal, financial and supporting information | Access should follow business roles and need-to-know principles, with protected documents and traceable access or changes |
| DP-09 | Actions and decisions must be auditable | Complaint handling may require users to explain what occurred, when and why | Material actions, status changes, ownership changes, communications, decisions and overrides should be timestamped and attributable |
| DP-10 | Information should be captured once and reused | Re-entering the same information increases effort and the risk of inconsistency | Validated complaint information should flow between stages without unnecessary duplication |
| DP-11 | Reporting definitions should be consistent | Different interpretations of status, ageing or closure can reduce confidence in reporting | Measures should use agreed definitions, documented calculations and controlled source data |
| DP-12 | Accessibility should be considered throughout | People may have different communication, language or accessibility needs | Communication preferences and accessibility needs should be recorded and considered during case handling |
| DP-13 | The design should support changing demand | Public data shows that monthly complaint volumes vary | Queues, dashboards, alerts and workload views should support monitoring and reprioritisation during higher-demand periods |
| DP-14 | Business rules should be maintainable | Policies, priorities and operational practices may change | Appropriate rules should be configurable through controlled governance rather than embedded invisibly in manual workarounds |

## Automation boundaries

The proposed solution may support:

- validation of required information;
- duplicate warnings;
- rule-based triage recommendations;
- workload-aware allocation recommendations;
- task and due-date creation;
- reminders and escalation alerts;
- standard communication templates;
- exception identification; and
- management reporting.

The proposed solution should not automatically make final decisions about:

- complaint merit;
- formal outcomes;
- whether evidence is credible;
- sensitive exceptions;
- fairness disputes; or
- matters requiring professional judgement.

These decisions should remain with authorised people and retain an auditable explanation.

## Design trade-offs

The future-state design must balance:

- speed with careful review;
- consistency with appropriate discretion;
- transparency with privacy;
- automation with human accountability;
- workload efficiency with fair allocation; and
- standardisation with accessibility needs.

Where these objectives conflict, the decision and its rationale should be visible rather than hidden within an automated process.

## Validation questions

1. Which decisions must always remain with a human?
2. Which triage factors may be used safely and fairly?
3. Who can override priority, allocation or escalation rules?
4. What explanation must be recorded for an override?
5. What information should each role be permitted to access?
6. Which actions require a permanent audit record?
7. How should workload and complaint complexity be measured?
8. Which accessibility needs must be captured?
9. Which business rules should be configurable?
10. Who owns and approves changes to those rules?