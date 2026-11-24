---
name: nonprofit-strategic-planning
description: "Runs an end-to-end nonprofit strategic planning process: scoping, environmental scan and stakeholder input, a priority-setting retreat, a 3-5 year plan with priorities, goals, objectives, and owners, a plan on a page, and board adoption. Use when someone says 'we need a strategic plan,' 'our strategic plan expires this year,' 'help me facilitate a board retreat to set priorities,' or 'how do we structure a 3-year plan.' Not for program logic models (use nonprofit-program-design), weekly execution systems like EOS (use nonprofit-eos-traction), KPI dashboards (use nonprofit-executive-dashboard), or vetting specific revenue streams (use nonprofit-revenue-diversification)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "A board-adopted 3-5 year plan that allocates everything."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Strategic Planning

## Boundaries

- Logic model / theory of change for a program a priority names: `nonprofit-program-design`.
- Weekly/quarterly execution habits for the approved plan (Rocks, scorecards, L10s):
  `nonprofit-eos-traction`. This skill produces the plan; EOS runs it day to day.
- The ED dashboard and board scorecard that measure the plan: `nonprofit-executive-dashboard`.
- Feasibility of specific earned-income or social enterprise models under a "diversify revenue"
  priority: `nonprofit-revenue-diversification`. This skill names the priority and its measure.
- Leading the organization through the disruption a plan causes (layoffs, restructuring, pivot
  communication): `nonprofit-change-management`.

## Core Framework: The Five-Phase Planning Cycle

1. **Prepare & Scope** — Charter the process before content work starts.
2. **Scan** — Gather internal and external data (environmental scan).
3. **Focus** — Synthesize the scan into a small number of strategic priorities.
4. **Draft** — Turn priorities into a written plan with goals, objectives, and metrics.
5. **Adopt & Cascade** — Board approval, staff rollout, and annual check-in rhythm.

Most failed nonprofit strategic plans fail at Phase 3 (too many priorities, no real choices made)
or Phase 5 (plan approved, then shelved and never referenced again).

### Phase 1: Prepare & Scope

1. Confirm the **planning horizon**: 3 years is standard for nonprofits (long enough to be
   strategic, short enough to stay relevant given funding volatility); use 1-year "bridge plans"
   for organizations in crisis or leadership transition, and 5-year plans only for stable,
   well-resourced organizations with a capital campaign or facilities horizon attached.
2. Decide **process ownership**: a Planning Committee (typically board chair, ED, 2-4 board
   members, 1-2 senior staff) owns the process; the full board approves the final plan. Staff below
   senior leadership should have an input channel but rarely sit on the committee itself.
3. Decide whether to engage an **outside facilitator**. Rule of thumb: use one when (a) the ED/board
   chair relationship is a topic the plan needs to address, (b) the last plan failed to get
   traction, or (c) budget allows (one rough range is $3,000-$25,000+ depending on org size and
   process depth; get current local quotes before budgeting). Small
   orgs with healthy dynamics can self-facilitate using this skill's agendas.
4. Set a **timeline**: typical cycle is 4-6 months from kickoff to board adoption. Compress to
   6-8 weeks only for bridge plans.
5. Build a **communication plan** for staff/stakeholders so the process doesn't feel like a black
   box — this is the single most common driver of post-adoption cynicism.

### Phase 2: Environmental Scan

Run these scans in parallel; each produces raw material for Phase 3, not a deliverable in itself.

- **SWOT** — collect via a facilitated staff session plus a separate board session; do not run
  them together, since board members often self-censor around staff and vice versa.
- **PEST/PESTLE** — use it to surface external trends the SWOT tends to miss, e.g., shifting
  government funding priorities, AI adoption in the sector, demographic change in the service area.
- **Stakeholder input**: board survey, staff survey, and — critically, and most often skipped —
  structured input from clients/beneficiaries, funders, and community partners. Use short (8-12
  question) surveys plus 6-10 one-on-one or small-group interviews with key informants (major
  funders, coalition partners, a sample of program participants).
- **Financial and programmatic trend review**: 3-5 year trend lines for revenue mix, program
  enrollment/outcomes, and unit costs. A strategic plan built without this data is opinion, not
  strategy — insist on it even when a committee wants to skip straight to brainstorming.
- **Competitive/peer landscape**: who else serves this mission or population, where are the gaps or
  duplications, what is this org's distinct value ("right to win")?

**Common failure mode**: scanning becomes an open-ended research project that drags the timeline out
3+ months. Timebox the scan phase to 4-6 weeks and cut off new data collection at the deadline.

### Phase 3: Focus — Priority-Setting

1. Convene a **priority-setting retreat** (half-day to full-day, board + senior staff) after
   circulating a scan summary in advance — never present raw scan data live; people need time to
   digest before deciding.
2. Use an **affinity-clustering exercise**: post every scan finding and stakeholder theme on
   sticky notes (physical or virtual/Miro), cluster into 5-8 themes, then dot-vote to narrow to
   3-5 **strategic priorities** (also called pillars or focus areas). Five is a practical ceiling —
   plans with 8-10 "priorities" are not prioritized at all and will not survive contact with a
   real budget.
3. For each candidate priority, stress-test with: Is this truly strategic (a real choice with
   tradeoffs) or just an ongoing operational duty restated? Does it require the board's attention,
   or is it staff's job to just do it? Naming "run great programs" as a strategic priority is a
   red flag — that's the baseline, not the differentiator.
4. Name explicitly what the organization will **stop doing or de-prioritize** — a plan with only
   additions and no subtractions has not actually made strategic choices.
5. Draft **goals** under each priority (the 3-year outcome) and **objectives** (annual, measurable
   milestones toward the goal). Each objective needs an owner and a metric — an objective without an
   owner becomes nobody's job by month two.

### Phase 4: Draft the Plan Document

Standard structure (aim for a document a board member can read in 15 minutes, plus an internal
staff-facing appendix with more operational detail):

1. Mission/vision/values (restate, revise only if this plan is also a rebrand moment)
2. Planning process summary (who was involved, what data informed it — builds legitimacy)
3. 3-5 Strategic Priorities, each with: rationale, 3-year goal, annual objectives, success metrics,
   lead owner
4. Resource implications (does this plan require a capital campaign, new hires, new systems?) —
   flag but do not fully build these here; hand off to `nonprofit-budgeting` or
   `nonprofit-revenue-diversification` as needed
5. Implementation and monitoring approach (who reviews progress, how often)

Also produce a **one-page visual summary** (a "plan on a page") for staff-wide distribution — this
is the version that actually gets referenced day to day, not the full narrative document.

```
[Organization] Strategic Plan [start year]-[end year] — Plan on a Page
Mission: [one sentence]        Vision: [one sentence]        Values: [3-5 words]

Priority 1: [name]
  3-year goal: [outcome]
  Year-1 objectives: [objective] — owner: [name] — metric: [measure + target]
Priority 2: [name]   (same shape)
Priority 3: [name]   (same shape; 3-5 priorities maximum)

We will stop or de-prioritize: [items]
How we'll track it: quarterly board check-in; annual refresh in [month]
```

### Phase 5: Adopt & Cascade

1. Present to the full board for formal adoption (board vote/resolution, not just "discussion").
2. Cascade to staff: an all-staff meeting where the ED walks through the plan-on-a-page and
   explicitly connects it to department/team work plans.
3. Set a **quarterly check-in cadence** at board meetings (a standing 15-minute agenda item
   reviewing objective status by priority) and an **annual refresh** (revisit priorities, not a full
   re-plan, each year of the 3-year cycle).
4. Assign an internal owner (often the ED or a COO/deputy director) accountable for keeping the plan
   alive between board meetings — plans with no assigned owner are the ones that get shelved.

## For advisors

- Sell the *process design* (phase timeline, governance, facilitator role) before any content;
  reset the expectation that the consultant will supply the answer. Scope scan, facilitation, and
  drafting as separate phases so the client can self-serve parts.
- Frame the board's job as **ratifying tradeoffs**, not wordsmithing.
- If the ED is using the process to relitigate a board decision, or a board faction is using it to
  challenge the ED, name it with the board chair as a governance issue rather than papering over it.

## Verify Before Acting

Before the plan goes to the board for adoption:

- [ ] 3-5 priorities, each a real choice with tradeoffs, plus a written stop-doing list.
- [ ] Every annual objective has a named owner and a metric with a target.
- [ ] Trend data (revenue mix, enrollment/outcomes, unit costs) cited in the plan matches the
      finance and program records.
- [ ] Resource implications are flagged and handed to `nonprofit-budgeting` (or
      `nonprofit-revenue-diversification`) before adoption.
- [ ] Client/beneficiary, funder, and partner input is reflected, not only board and staff input.
- [ ] The adoption motion, quarterly check-in slot, and internal plan owner are set.

## Common Failure Modes

- **No owner between board meetings**: the plan is adopted in June and never mentioned again. Name
  the internal owner and put the quarterly check-in on the board calendar before the adoption vote.
- **Priority sprawl and operational duties**: 8+ "priorities," or baseline duties like "run great
  programs" listed as priorities, signal that no choice was made. Test each with "what would we stop doing to fund this?"
- **Scan without synthesis**: months of surveys and data with no facilitated session to turn it into
  decisions. Circulate a written scan summary before the retreat and cut off data collection at
  the deadline.
- **Input collected but not reflected**: staff and community gave input that never visibly shaped
  the plan, so buy-in is missing at rollout. Include a "what we heard and what changed" page.
- **No resourcing link**: priorities adopted with no budget, staffing, or fundraising discussion,
  so Year 1 objectives quietly fail. Cost Year 1 objectives against the next budget before adoption.
