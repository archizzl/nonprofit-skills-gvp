---
name: nonprofit-grant-writing
description: "Drafts letters of inquiry (LOIs), full grant proposals and grant reports for foundation, government and corporate funders: needs statements, program narratives, outcomes and evaluation sections, and budget narratives written to a specific funder's guidelines. Use when a user says 'write an LOI for this funder', 'draft the program narrative for this RFP', 'write a budget narrative' or 'write our year-end grant report'. Not for finding, vetting or scoring funders or tracking deadlines (use nonprofit-grant-research), building a logic model from scratch (use nonprofit-program-design), or calculating indirect cost rates (use nonprofit-cost-allocation)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Proposals are binding representations to a funder about what you will deliver."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Grant Writing: LOIs, Proposals & Reports

## Boundaries

- Finding and vetting the funder, tracking deadlines, scoring fit: `nonprofit-grant-research`
  first.
- Building the logic model or theory of change: `nonprofit-program-design` first. This skill
  assumes that design work exists and translates it into funder-ready narrative and budget
  language.
- Indirect cost rate selection, MTDC calculations and Federal rate questions:
  `nonprofit-cost-allocation`.
- Measurement approach behind the evaluation plan: `nonprofit-outcomes-measurement`.

## Standard Proposal Structure

Most funder applications map onto this sequence even when section names vary; use it as the
default skeleton and then re-map to the funder's exact required headers:

1. **Executive summary / cover letter** — one paragraph each on: who you are, the problem, the ask
   amount, and the expected outcome. Written last, read first.
2. **Statement of need** — the problem, backed by data specific to your service area (not national
   statistics alone), told with urgency but without exploitative framing (dignity-preserving
   framing guidance lives in `nonprofit-storytelling`; apply it here).
3. **Program description / methodology** — what you will do, drawn directly from the program's
   logic model (activities and outputs); name the model type if funders expect it (e.g.,
   evidence-based, evidence-informed, promising practice).
4. **Goals, objectives, and outcomes** — SMART objectives; outcomes map to the logic model's
   outcome tier, not activities (see the outputs-vs-outcomes failure mode below).
5. **Evaluation plan** — how outcomes will be measured, what data collection tools, and reporting
   timeline; keep this consistent with whatever the org actually tracks (coordinate with
   `nonprofit-outcomes-measurement` rather than promising a measurement approach the org can't
   execute).
6. **Organizational capacity** — track record, key staff bios, relevant past grants delivered
   successfully.
7. **Budget and budget narrative** — see below.
8. **Sustainability plan** — how the program continues after this grant period (diversified
   funding, earned revenue, embedded costs).

## Letters of Inquiry (LOI)

An LOI is a 1-2 page gate before a full proposal invitation. Include: brief org description,
problem statement (2-3 sentences), proposed project and amount requested, alignment to the
funder's stated priorities (cite their specific language), and one differentiator. Cut everything
that would appear in the full proposal — an LOI's job is to earn the invitation, not tell the whole
story.

## Budget Narrative

A budget narrative justifies every line item in the budget spreadsheet in prose, tied to the
program description:

- State the basis for each figure (e.g., "0.5 FTE Program Coordinator at $58,000 annual salary +
  22% fringe = $35,380") rather than a bare number.
- Separate direct and indirect costs; do not assume every administrative cost is indirect.
  State the finance-approved rate, base, effective period, and authority. For Federal funding,
  distinguish a Federal negotiated rate, a pass-through-negotiated rate, and an eligible de minimis
  election of **up to 15% of MTDC**, not an automatic 15% or a universal 10%. Eligibility requires
  no current Federal negotiated rate, including a provisional rate. Do not invent missing approval
  or eligibility. See [2 CFR 200.414](https://www.law.cornell.edu/cfr/text/2/200.414) and
  [200.332(b)(4)](https://www.law.cornell.edu/cfr/text/2/200.332).
- Show the MTDC arithmetic and exclusions, not a percentage of the entire project budget. Route
  rate selection, MTDC exclusions (including the revised subaward limit), which award terms govern
  (revised rules are not retroactive; an existing NICRA's approved base is not silently changed),
  and Federal cap authority to `nonprofit-cost-allocation`, and use its calculation. See
  [200.1](https://www.law.cornell.edu/cfr/text/2/200.1).
- Flag restricted expense categories and distinguish private-funder caps from Federal requirements.
  For Federal funds, ask finance to verify the legal authority for a conflicting cap; a pass-through's
  preference alone does not override the protections for negotiated or elected rates in
  [200.414(c)–(f)](https://www.law.cornell.edu/cfr/text/2/200.414).
- Reconcile the requested amount against the total project budget — clearly show what other
  revenue sources cover the balance if this grant is partial funding.

## Concrete Steps

1. Read the RFP/NOFO or funder guidelines in full before drafting; extract every required section
   header, word/page/character limit, required attachments, and submission mechanics (portal,
   email, hard deadline time zone).
2. Confirm the program design/logic model source material exists and is current; if not, route to
   `nonprofit-program-design` before drafting outcomes language.
3. Draft in the funder's required order and exact section names, even if it differs from the
   skeleton above — reviewers score against their own rubric, not general best practice.
4. Write the statement of need with locally specific data and named sources.
5. Draft goals/objectives as SMART statements distinct from activities.
6. Build the budget narrative line-by-line against the numeric budget; reconcile totals and match
   the indirect rate, base, and cost period to finance's approved calculation. Keep unresolved rate
   assumptions visibly marked for review rather than presenting them as approved.
7. Trim to the funder's word/page/character limit — cutting adjectives and repeated context first,
   never cutting the ask amount, outcomes, or evaluation plan.
8. Route for internal review: program staff check factual/programmatic accuracy, finance checks
   the budget, ED or board chair signs off on institutional commitments before submission.
   Escalate unresolved Federal rate, base, or applicability questions to the qualified reviewer
   required by `nonprofit-cost-allocation`; ordinary proposal drafting remains staff-reviewed.
9. Submit ahead of the deadline accounting for portal upload time, after ticking the checklist in
   Verify Before Acting.
10. On award, calendar the reporting schedule and build the report from the same
    outcomes/evaluation language promised in the proposal — do not let the report drift from what
    was funded.

## Grant Reports

Structure interim/final reports around the original proposal's stated objectives: report progress
against each SMART objective, actual spend against the approved budget (flag and explain material
variances), a challenges/lessons-learned section (funders read this for candor, not just success
stories), and specific plans for the next period if renewal is possible.

## Verify Before Acting

Before submission:

- [ ] Every required section header, in the funder's order and wording, is present and within its
  word/page/character limit.
- [ ] Narrative figures foot to the budget spreadsheet; the requested amount reconciles to the total
  project budget and other sources.
- [ ] The indirect rate, base and period match finance's approved calculation; unresolved rate
  assumptions are visibly marked, and Federal rate questions went through `nonprofit-cost-allocation`.
- [ ] Objectives are outcomes, not outputs, and the evaluation plan matches what the org actually
  tracks.
- [ ] Required attachments are in hand (commonly W-9, 501(c)(3) determination letter, board list,
  audited financials, org chart, plus any funder-specific items).
- [ ] Program staff, finance, and the ED or board chair have signed off as described in step 8.

## Common Failure Modes

- **Recycled boilerplate**: submitting the same narrative to every funder without mapping to their
  specific stated priorities and section names — lowers scoring even when the program itself is
  strong.
- **Outputs mislabeled as outcomes**: "served 200 clients" is an output; "72% of clients improved
  reading level by one grade" is an outcome — funders increasingly require the latter.
- **Budget-narrative mismatch**: numbers in the narrative don't foot to the attached budget
  spreadsheet — always reconcile before submission.
- **Mishandling restrictions**: ignoring a valid expense restriction, or accepting a conflicting
  Federal indirect-cost cap without checking its authority; resolve with finance before submission.
- **Missing attachments**: technically compliant narrative but incomplete required-attachments
  checklist, causing an administrative rejection regardless of narrative quality.
- **Rewriting prose on instinct**: to raise a win rate, first audit 3-5 recent declined proposals
  for the pattern (funder-fit misses go to `nonprofit-grant-research`; narrative or outcomes
  clarity stays here).
- **Program description and evaluation conflated**: keep what you will do separate from how you
  will measure it.

## For advisors

- Recommend a centrally maintained boilerplate library (mission, org history, capacity statements)
  so writers spend drafting time on the funder-specific need and outcomes sections that move
  scores.

Targeted federal indirect-cost check: September 16, 2026. Verify current agency and award terms
at use; this check does not certify the rest of the proposal or authorize submission.
