---
name: project-risk-assessment
description: >
  Analyzes uploaded project documents to identify, assess, and document key risks across four categories: schedule delays, stakeholder alignment, scope creep, and budget overruns. Use this skill when Amy says "run a risk assessment," "assess project risks," "analyze risks for this project," or "write a risk assessment" and provides project documents.
trigger_phrases:
  - "run a risk assessment"
  - "assess project risks"
  - "write a risk assessment"
  - "analyze risks for this project"
  - "identify project risks"
---

## Project Risk Assessment Skill

Use this skill when Amy uploads project documents (status reports, budget snapshots, requirements, scope docs, or change orders) and asks for a structured risk assessment. The goal is to surface risk signals from the documents and produce a detailed, actionable mitigation playbook she can use or share with stakeholders.

---

### Step 1: Confirm Inputs

Before analyzing, verify the uploaded documents. Identify what was provided (e.g., status report dated X, budget snapshot, requirements doc). If a critical document type is missing — especially a current status report or budget — note the gap and flag that findings may be incomplete.

---

### Step 2: Extract Risk Signals

Read through all uploaded documents. Extract specific evidence — not assumptions — that point to risk in each of the four categories:

- **Schedule / Timeline Risks**: Look for milestone slippage, dependency blockers, resource gaps, overdue tasks, or compressed timelines mentioned in status reports.
- **Stakeholder Alignment / Communication Risks**: Look for unresolved decisions, missing approvals, conflicting direction from sponsors or business owners, low engagement, or unclear ownership.
- **Scope Creep / Requirement Change Risks**: Look for informal feature additions, open requirement items, change requests pending approval, unclear acceptance criteria, or scope that has expanded since project initiation.
- **Budget / Financial Risks**: Look for burn rate trends, actuals vs. forecast variance, unapproved spending, open change orders, or forecast warnings in budget documents.

---

### Step 3: Score and Prioritize Each Risk

For each identified risk, assign:
- **Likelihood**: High / Medium / Low
- **Impact**: High / Medium / Low
- **Overall Risk Level**: High / Medium / Low (based on the combination)

List risks in descending priority order within each category.

---

### Step 4: Write Detailed Mitigation Playbooks

For each High and Medium risk, produce a mitigation playbook that includes:
1. **Risk description**: One sentence, grounded in evidence from the documents.
2. **Option A – Proactive mitigation**: Steps Amy can take now to prevent or reduce the risk.
3. **Option B – Reactive mitigation**: Steps to take if the risk materializes.
4. **Trade-offs**: Note the effort, stakeholder impact, or timeline implications of each option.
5. **Recommended owner**: Suggest who on the project should own this risk (e.g., PM, sponsor, BA, vendor).

For Low risks, include a one-line watchlist note without a full playbook.

---

### Step 5: Produce the Output Document

Structure the final output as follows:

```
# Project Risk Assessment — [Project Name or "Unnamed Project"] — [Date]

## Summary
[3–5 sentence executive summary of overall risk posture]

## Risk Register
[Table: Risk ID | Category | Risk Description | Likelihood | Impact | Risk Level]

## Mitigation Playbooks
[One section per High/Medium risk, using the playbook format above]

## Watchlist (Low Risks)
[Bulleted list]

## Document Sources Referenced
[List the documents analyzed and their apparent dates]
```

---

### Quality Check Before Responding

Before delivering the assessment, verify:
- [ ] Every risk claim is traceable to something in the uploaded documents — no invented risks.
- [ ] All four risk categories are addressed, even if a category has no findings (state that explicitly).
- [ ] Every High and Medium risk has a full playbook with both options and trade-offs.
- [ ] The executive summary accurately reflects the risk register below it.
- [ ] The output is formatted for an executive or client audience — professional, clear, no internal AI commentary.
