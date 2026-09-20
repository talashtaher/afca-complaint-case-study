# Working Method and Evidence Rules

## Why this document exists

This project must be credible even though the author does not have internal access to AFCA. The following rules prevent polished guesses from being presented as business facts.

## Evidence classification

| Label | Meaning | Example use |
|---|---|---|
| `FACT` | Directly supported by a cited public source | A published process step or complaint count |
| `FINDING` | Reproducibly calculated from cited data | Month-on-month change in complaints received |
| `ASSUMPTION` | A declared condition adopted for the case | Proposed users require role-based access |
| `HYPOTHESIS` | A possible cause requiring validation | Manual routing may contribute to allocation delay |
| `RECOMMENDATION` | A proposed change derived from the analysis | Introduce rules-assisted triage with human review |

## Quality rules

1. Record a source before using it as evidence.
2. Preserve raw data unchanged and transform a copy.
3. Give every processed field a definition and transformation rule.
4. Do not invent interview notes, workshop outcomes or internal metrics.
5. Link each proposed requirement to a documented need, risk or objective.
6. Make acceptance criteria observable and testable.
7. Record major design choices and rejected alternatives in the decision log.
8. Use plain language and explain domain terms in the glossary.
9. Retain calculations and intermediate outputs needed to reproduce findings.
10. Treat accessibility, privacy, security, auditability and fairness as design constraints, not afterthoughts.

## Validation language

Use wording such as:

- "Public information indicates..."
- "The published data shows..."
- "A plausible explanation is..., but internal validation would be required."
- "This case study proposes..."

Avoid wording such as:

- "Staff confirmed..." unless a real, citable statement exists.
- "The system cannot..." without evidence about the internal system.
- "The root cause is..." when only aggregate data is available.
- "The solution will save..." without an auditable calculation.
