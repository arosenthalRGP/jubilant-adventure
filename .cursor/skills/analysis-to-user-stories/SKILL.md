---
name: analysis-to-user-stories
description: >
  Synthesizes raw analytical inputs — data exports, meeting notes, SME transcripts, existing documentation, or any combination — into structured, stakeholder-ready user stories with acceptance criteria, dependencies, and UI/UX specifications.
  Use this skill when Amy says "write user stories from this," "turn this analysis into requirements," "draft stories from these notes," or "synthesize this into user stories."
methodology: Agile/SAFe
required_elements:
  - user story (role/goal/reason format)
  - acceptance criteria (testable conditions)
  - dependencies (other stories or systems)
  - UI/UX or wireframe specifications (when applicable)
---

## Analysis to User Stories

Use this skill whenever you have raw analytical inputs — data exports, interview notes, meeting transcripts, existing documentation, or a mix — and need to produce structured, stakeholder-aligned user stories that both business and technical teams can act on.

---

### Step-by-Step Procedure

**1. Ingest and inventory the inputs.**
Read all provided materials in full. Note the source type for each (e.g., SME interview, data export, existing spec, meeting notes). Flag any gaps — missing actor context, unclear business rules, or ambiguous data — and list them at the end for Amy to resolve.

**2. Identify the user roles and goals.**
Extract the distinct user types referenced across the inputs. Map each to a clear goal they are trying to achieve and the business reason behind it. These become the basis for your story personas.

**3. Draft each user story in SAFe format.**
Write each story as:
> *As a [specific user role], I want to [specific action or capability] so that [measurable business outcome].*

Avoid vague roles ("user," "admin") — use the specific persona surfaced in step 2. One story per discrete capability; split compound stories.

**4. Write acceptance criteria as testable conditions.**
For each story, provide 3–6 acceptance criteria using Given/When/Then format:
> *Given [precondition], When [action], Then [expected result].*

Each criterion must be independently verifiable by a QA tester or business stakeholder. Avoid criteria that require interpretation.

**5. Document dependencies.**
For each story, list:
- **Upstream dependencies**: other stories, APIs, data feeds, or systems that must exist first.
- **Downstream dependencies**: what this story unblocks.
- Label with story title or system name (not just "TBD").

**6. Add UI/UX specifications.**
Where inputs reference screens, flows, or interactions, include a concise UI/UX note per story:
- Reference any wireframe or design artifact mentioned in the inputs.
- If none exists, describe the expected interaction pattern (e.g., modal form, inline edit, read-only display).
- Flag stories where a wireframe should be created before development begins.

**7. Organize the output.**
Present stories in a logical sequence (epic or workflow order when determinable). Use this structure per story:

```
### [Story Title]
**User Story:** As a...
**Acceptance Criteria:**
- Given / When / Then...
**Dependencies:** [upstream / downstream]
**UI/UX Notes:** [spec or flag]
**Open Questions:** [if any]
```

---

### Quality Check Before Responding

- [ ] Every story follows the SAFe role/goal/reason format with a specific persona.
- [ ] All acceptance criteria are testable — no subjective language ("easy," "fast," "appropriate").
- [ ] Dependencies are named specifically, not left as placeholders.
- [ ] UI/UX notes are present for every story, even if only a flag.
- [ ] Stories are scoped to a single capability (no compound stories).
- [ ] Open questions are surfaced clearly, not silently omitted.
- [ ] Output is readable by a non-technical stakeholder without prior context.
