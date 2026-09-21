# Data dictionary

This dictionary describes the fields used in the monthly AFCA complaints dataset.

| Field | Type | Description | Analytical caution |
|---|---|---|---|
| `month` | Date | Reporting month, recorded as the first calendar day of the month. | Represents a monthly reporting period, not the date of an individual complaint. |
| `financial_year` | Text | Australian financial year covered by the dataset. | Used for reporting and filtering only. |
| `complaints_received` | Whole number | Complaints received at AFCA’s Registration and Referral stage during the reporting month. | Complaints received may later be resolved at R&R or progress to Case Management. |
| `complaints_resolved_rr` | Whole number | Complaints reported by AFCA as resolved during the Registration and Referral stage. | The public chart does not establish that these complaints came from the same month’s received cohort. |
| `complaints_progressed` | Whole number | Complaints that progressed from Registration and Referral and were accepted into Case Management during the reporting month. | This should not be treated as a direct monthly conversion rate from complaints received. |
| `complaints_closed` | Whole number | Complaints closed during Case Management in the reporting month. | AFCA states that this measure can include complaints brought to AFCA before the reporting period. |

## Process context

Registration and Referral is the first stage of AFCA’s complaint process. AFCA refers the complaint to the relevant financial firm and requests a response to both AFCA and the complainant. Complaints that are not resolved at this stage may progress to Case Management.

## Interpretation rule

The four monthly measures describe activity at different stages of the complaint process. They are not necessarily the same group of complaints moving through a single month.

For this reason, the analysis will compare volumes and trends but will not describe ratios such as `closed ÷ received` as true resolution or closure rates.

## Sources

- AFCA Datacube glossary: https://data.afca.org.au/glossary
- AFCA complaint process: https://data.afca.org.au/afcas-processes
- AFCA historical comparison: https://data.afca.org.au/historical-comparison