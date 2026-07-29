---
name: project-status-to-exec-summary
description: >
  Condenses a lengthy project status report into a structured executive summary
  for stakeholder communication. Use when Amy says "summarize this status report,"
  "create an exec summary," "turn this into a stakeholder update," or "condense
  this project report."
triggers:
  - "summarize this status report"
  - "create an exec summary"
  - "turn this into a stakeholder update"
  - "condense this project report"
  - "executive summary from this"
author: Amy (RGP)
version: 1.0
---

## Project Status → Executive Summary

Use this skill when Amy provides a project status report, update document, or similar source material and needs a concise, stakeholder-ready executive summary — either for senior leadership or a technical audience.

---

### Step-by-Step Procedure

**1. Ingest and orient.**
Read the full source document before writing anything. Note the project name, reporting period, and any existing RAG/health indicator. If these are missing, flag them at the end.

**2. Identify the audience.**
Determine whether the summary is for **executive leadership** (business outcomes, financials, decisions, risk exposure — minimize technical detail) or a **technical/delivery team** (system-level risks, implementation blockers, sprint/milestone specifics). If Amy hasn't specified, ask before proceeding.

**3. Extract the seven required elements.**
Pull and organize findings under these categories — skip none, mark "No update" if truly absent:
- 🔴🟡🟢 **Project Health** — Overall RAG status with one-line rationale
- 💰 **Budget & Financials** — Spend to date, forecast vs. budget, variance flag
- 📅 **Timeline & Milestones** — Key milestones: completed, on track, at risk
- ⚠️ **Risks & Issues** — Active risks/issues, owner, and mitigation status
- 🙋 **Decisions Needed** — Specific asks of stakeholders, with deadline if known
- 👥 **Team & Resource Updates** — Staffing changes, capacity concerns
- ✅ **Next Steps & Action Items** — Concrete actions, owners, and due dates

**4. Draft the summary.**
Write to the identified audience. Target **200–300 words** using **6–8 structured bullet points or 2–3 short paragraphs** — never both formats combined. For executive leadership: lead with health status and financials, close with decisions needed. For technical stakeholders: lead with milestones and blockers, close with action items.

**5. Format for readability.**
Use the RAG emoji indicator prominently at the top. Use **bold labels** for each section. Keep sentences short. Avoid jargon when writing for leadership; use precise technical terms when writing for delivery teams.

**6. Quality check before delivering.**
Confirm:
- [ ] All seven elements are present or explicitly noted as absent
- [ ] Word count is within 200–300 words
- [ ] Tone and detail level match the stated audience
- [ ] No critical data (budget figures, dates, risk owners) was fabricated — flag any gaps for Amy to fill
- [ ] Decisions needed are clearly framed as asks, not observations

If any check fails, revise before responding.
