---
name: nonprofit-program-design
description: "Builds logic models and theories of change that connect a nonprofit program's inputs, activities, and outputs to short-, mid-, and long-term outcomes, with assumptions and external factors named. Use when asked to \"build a logic model for our program,\" \"we need a theory of change,\" \"show the funder how our activities lead to outcomes,\" or \"why isn't this program producing results.\" Not for writing the model into a funder narrative (use nonprofit-grant-writing), measuring whether outcomes occurred (use nonprofit-outcomes-measurement), establishing need (use nonprofit-needs-assessment), or adapting to new sites (use nonprofit-program-scaling)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Logic models set what the program promises to achieve."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Program Design

## Boundaries

- Turning a finished model into funder-facing prose for a specific RFP: `nonprofit-grant-writing`.
- What to measure, how to collect data, and reporting results against the model:
  `nonprofit-outcomes-measurement` (this skill defines what should happen; that skill defines how
  you'll know if it did).
- Whether the program is needed at all: `nonprofit-needs-assessment` (program design assumes need is
  established or hands off from it).
- Adapting a working model to new sites/populations: `nonprofit-program-scaling`.

## Core Frameworks

### 1. Logic Model (linear, single-program)

Default layout: Kellogg's five components (inputs, activities, outputs, outcomes, impact), shown as
six columns because outcomes are split by time horizon, in the sequence funders (United Way, W.K.
Kellogg Foundation, CDC) expect:

| Inputs | Activities | Outputs | Short-Term Outcomes | Mid-Term Outcomes | Long-Term Outcomes / Impact |
|---|---|---|---|---|---|
| Resources invested: staff, funding, volunteers, curriculum, partners, facilities | What the program *does* with those resources | Direct, countable products of activities (units of service) | Change in knowledge, attitude, skill (0-1 yr) | Change in behavior or practice (1-3 yr) | Change in condition/status — the ultimate impact (3+ yr) |
| Example (illustrative): 2 job coaches, employer partners, curriculum | Job-readiness workshops and mock interviews | [#] workshops; [#] participants completing | Participants gain interview skills | Participants secure interviews and are hired | Participants retain employment and stable income |

Rules of thumb that catch most first-draft errors:
- **Outputs are not outcomes.** "50 workshops delivered" or "200 meals served" is an output — it
  counts activity, not change in a person or system. If a cell says "number of X provided/attended,"
  it belongs in Outputs, not Outcomes.
- **Outcomes must be verb-of-change statements about the participant/system**, not the program:
  "Participants demonstrate increased financial literacy" (outcome) vs. "We ran 6 financial literacy
  classes" (output).
- **Every arrow needs a plausible mechanism.** If you can't say *why* an output would cause the next
  outcome, the model has a logic gap — flag it rather than paper over it.

### 2. Theory of Change (ToC)

Broader and less linear than a logic model — a ToC states the program's change hypothesis, usually
as an "If...then...because..." backwards-mapped chain starting from the long-term goal:

> "If [population] receives [intervention], then [short-term change] will occur, which will lead to
> [mid-term change], ultimately resulting in [long-term impact], because [the underlying assumption
> or evidence base]."

A full ToC additionally documents, beyond the logic model's columns:
- **Assumptions**: conditions that must hold true for the chain to work (e.g., "participants have
  reliable transportation to attend sessions").
- **Preconditions/pathways**: intermediate changes required before the outcome, often shown as a
  "pathway of change" map with multiple parallel tracks (individual, organizational, systemic).
- **Rationale/evidence base**: the research or prior experience justifying each link — cite it. A
  ToC with no evidence base is an opinion, not a theory.
- **External/contextual factors**: forces outside the program's control that could help or hinder
  (policy shifts, funding cycles, seasonality, community trust).

Use a **logic model** when a funder or board wants a compact, boxed one-pager tied to a specific
program. Use a **theory of change** when the organization needs to articulate or defend the
underlying causal hypothesis — new program design, strategic planning, or when a funder explicitly
asks "what is your theory of change."

### 3. Related Frameworks

- **Results-Based Accountability (RBA, "Turn the Curve")** — use its population-results vs.
  performance-measures split when the program is one contributor among many to a community outcome.
- **Collective Impact** — when the program sits inside a multi-org initiative, show contribution to
  the shared outcome, not sole attribution.
- Default to the Kellogg layout above unless the funder specifies its own template.

## Instructions

1. **Confirm the unit of design.** Is this a single program, a department, or the whole
   organization's ToC? Logic models work best scoped to one program; a full-org ToC sits one level
   above and can spawn multiple program-level logic models.
2. **Start from the long-term outcome/impact and work backward** (backward mapping). Ask: "What
   condition are we ultimately trying to change?" Then: "What would have to be true right before that
   for it to happen?" Repeat until you reach activities the program actually controls.
3. **Draft outputs and activities forward** from current/planned resources, then check they actually
   connect to the backward-mapped outcome chain. Where they don't connect, either the activity is
   unnecessary or an outcome step is missing.
4. **Stress-test every arrow** with "so that..." — "We deliver job-readiness workshops, SO THAT
   participants gain interview skills, SO THAT participants secure interviews, SO THAT participants
   are hired." If a "so that" doesn't hold logically, revise.
5. **Name the assumptions and external factors explicitly** in a dedicated section/row — don't leave
   them implicit. This is the single most commonly skipped step and the first thing a sophisticated
   funder or evaluator will probe.
6. **Distinguish outputs from short-term outcomes** with a gut-check: "Is this a count of activity,
   or a change in a person/system?" Move miscategorized items.
7. **Right-size the time horizons** to the program's actual cycle — short-term (0–1 yr), mid-term
   (1–3 yr), long-term (3+ yr) is a default, not a rule; a 6-week intervention may compress these.
8. **Validate with the people closest to delivery** (program staff, participants/beneficiaries if
   possible) before finalizing — designs built only by leadership frequently encode assumptions frontline
   staff know to be false.
9. **Produce the standard deliverable**: a one-page logic model table (for board/funder use) plus,
   for new or contested programs, a 1–2 page theory-of-change narrative with assumptions and evidence
   base called out separately.
10. **Hand off cleanly**: flag which outcomes need indicators and measurement plans
    (→ `nonprofit-outcomes-measurement`) and which sections a grant writer will need lifted into
    narrative form (→ `nonprofit-grant-writing`).

## Common Failure Modes

- **Output/outcome conflation** — the most frequent error; "number served" dominates the outcomes
  column. Fix by applying the change-verb test in Step 6.
- **Missing assumptions** — a model that looks airtight on paper but silently depends on unstated
  conditions (transportation, digital access, family support) that later explain "unexpected"
  underperformance.
- **Outcome overreach / attribution creep** — claiming long-term, systemic impact (e.g., "reduces
  community poverty") that a single modest program cannot plausibly claim alone; use RBA's
  population-vs-performance distinction to right-size the claim, or explicitly frame it as
  contribution within a collective-impact effort.
- **Designing in isolation from delivery staff** — leads to a model nobody on the ground recognizes
  or can execute against.
- **No evidence base** — a theory of change asserted without citing prior research, pilot data, or
  comparable-program evidence reads as aspirational rather than credible to funders and boards.
- **One-size logic model reused for structurally different programs** — copy-pasting a model across
  dissimilar programs instead of re-deriving it; surface-level edits leave stale, mismatched logic.

## For Advisors/Consultants

When facilitating this for a client:
- Run the backward-mapping (Step 2) as a live facilitated exercise with program staff and at least
  one board or leadership representative in the room — the disagreements that surface are the design
  work, not a distraction from it.
- Bring an external framework name (logic model vs. ToC vs. RBA) into the room explicitly; clients
  often conflate "outcomes" and "outputs" and having a named framework to point to depersonalizes the
  correction.
- Keep the assumptions/risk memo separate from the model itself so it survives as a standing risk
  register.
- Flag scope explicitly to the client: this engagement builds the model; recommend
  `nonprofit-outcomes-measurement` as a distinct follow-on engagement (often a different SOW) rather
  than assuming measurement design is included.

## Standard Deliverables

- One-page logic model (six-column table, Kellogg-style, as above)
- Theory-of-change narrative (1–2 pages) with assumptions, pathways, and evidence base
- Assumptions/risk register (bulleted list, owner-assigned)
- Handoff notes flagging which outcomes need indicators (for `nonprofit-outcomes-measurement`) and
  which sections need funder-narrative treatment (for `nonprofit-grant-writing`)
