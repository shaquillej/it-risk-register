# IT Risk Register — Access, Compliance & Third-Party Risk

Self-directed GRC portfolio project by Shaquille Jackson. Applies standard risk-assessment methodology to a simulated healthcare organization (Wasatch Family Health Clinic) — the same environment used in the Okta IAM, HIPAA audit, and ServiceNow projects in this portfolio.

## Overview

A 10-entry IT risk register scoring each risk on Likelihood x Impact, with documented treatment plans, named owners, and a review cadence. This is a self-directed exercise built to demonstrate risk register construction and maintenance — not a record of a real employer's actual risk environment.

Two entries (R-04, R-07) are deliberately cross-validated against findings already surfaced independently by the [HIPAA-Aligned User Access Review & Compliance Audit](https://github.com/shaquillej/hipaa-user-access-review-compliance-audit) project, to show the register and the audit arrive at consistent severity ratings without being copy-pasted from each other.

## What Was Built

- A full 10-risk register spanning Access Control, Third-Party/Vendor, Governance, Data Governance, and Technical/Operational categories.
- Likelihood (1–5) x Impact (1–5) scoring for every risk, banded 1–6 Low / 7–14 Medium / 15–25 High.
- A documented treatment plan (mitigate, transfer, accept, or avoid), named owner role, and current status for every entry.
- A companion Word document (`IT_Risk_Register.docx`) formatted as a deliverable a GRC or IT risk analyst would actually hand to a manager or auditor.

## Design Approach

Each risk was scored independently using the same likelihood/impact criteria before checking it against related portfolio findings — R-04 (vendor DPA gap) and R-07 (over-broad role definitions) both landed at High risk on their own, then were cross-checked against the HIPAA audit's F-01 and F-02 findings, which flagged the same underlying issues. Agreement between the two independent exercises is the point: it shows the scoring methodology is repeatable, not reverse-engineered from a desired answer.

## Tools and Skills Demonstrated

Risk scoring methodology (likelihood x impact), risk register construction and maintenance, treatment planning, cross-functional ownership assignment, and review-cadence documentation.

## Risk Summary

| ID | Risk | Category | L | I | Score | Band | Owner | Status |
|----|------|----------|---|---|-------|------|-------|--------|
| R-01 | Excessive/orphaned access retained after a role change or offboarding event | Access Control | 4 | 4 | 16 | High | IAM Analyst | Mitigating |
| R-02 | Shared/generic accounts used in place of individually attributable accounts | Access Control | 2 | 4 | 8 | Medium | IAM Analyst | Open |
| R-03 | Quarterly User Access Review missed or completed incompletely | Governance | 2 | 3 | 6 | Low | IAM Analyst / Compliance | Mitigated |
| R-04 | Vendor/sub-processor handles data with no documented data protection agreement on file | Third-Party / Vendor | 3 | 5 | 15 | High | GRC / Procurement | Open |
| R-05 | Vendor-managed application component runs an outdated version between patch cycles | Technical / Operational | 2 | 3 | 6 | Low | IT / Vendor | Open |
| R-06 | MFA / step-up authentication not enforced consistently across all access tiers | Access Control | 3 | 4 | 12 | Medium | IAM Analyst | Mitigating |
| R-07 | Role definitions grant broader access than the HIPAA minimum-necessary standard requires | Compliance | 3 | 5 | 15 | High | Compliance / IAM | In Progress |
| R-08 | No formal incident response / breach notification runbook exists | Governance | 2 | 5 | 10 | Medium | GRC / IT | Open |
| R-09 | Support-ticket and access-log data retention/disposal schedule is undocumented | Data Governance | 2 | 3 | 6 | Low | IT / Compliance | Open |
| R-10 | New SaaS vendors can be onboarded without a documented risk assessment | Third-Party / Vendor | 3 | 3 | 9 | Medium | GRC | Mitigated |

**Totals: 3 High, 4 Medium, 3 Low.** Access control and third-party/vendor risk account for the majority of High-severity entries — consistent with where the HIPAA audit project independently found its highest-severity findings. Highest-priority open items: a documented vendor DPA/onboarding requirement (R-04) and closing the 2 over-broad role definitions already identified by the HIPAA audit (R-07).

Review cadence: full register reviewed quarterly alongside the User Access Review cycle; individual risks re-scored immediately if a related control changes (e.g., a new vendor onboarded, a role redefined).

## Repo Contents

- `IT_Risk_Register.docx` — full formatted register with methodology notes and summary.

---
Part of a broader self-directed GRC/IAM/Healthcare IT portfolio: [github.com/shaquillej](https://github.com/shaquillej)


---

## Project Status
Actively maintained as part of a coordinated 8-project portfolio spanning Healthcare IT, IAM, and GRC. See the full set and how they connect at [github.com/shaquillej](https://github.com/shaquillej), or the write-ups at the [portfolio site](https://sites.google.com/view/shaquille-jackson-healthcare-i).
