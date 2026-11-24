---
name: nonprofit-donor-pipeline
description: "Builds and manages donor pipeline and moves-management systems: prospect identification and qualification, cultivation move plans, stage tracking, portfolio assignment, and stage-to-stage conversion analysis. Use when a user says 'build a moves-management pipeline', 'write next-move plans for my portfolio', 'who in this prospect list is stalled?' or 'how many prospects do we need to hit our goal?'. Not for setting ask amounts or writing major-gift proposals (use nonprofit-major-gifts), acknowledgments and lapsed-donor win-back (use nonprofit-donor-retention), or CRM selection and setup (use nonprofit-donor-crm)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Moves management runs on donor records and personal information."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Donor Pipeline & Moves Management

## Boundaries

- Ask strategy, amount-setting and proposal structure: `nonprofit-major-gifts`.
- Acknowledgment workflows, thank-you SLAs, the donor journey and lapsed-donor win-back:
  `nonprofit-donor-retention`.
- CRM software selection and configuration: `nonprofit-donor-crm`.
- Low-touch track for downgraded prospects: `nonprofit-annual-appeals`.

## Stages

Treat every prospect as sitting in exactly one stage at a time:

1. **Identification** — Suspect enters the pipeline from a data source: wealth screening flags,
   board/staff referral, event sign-in, volunteer roster, grateful-client list, digital engagement
   score. Not yet a "prospect" until minimally qualified.
2. **Qualification** — Confirm the three qualification axes: **capacity** (ability to give),
   **affinity** (connection to mission), and **propensity** (giving history/philanthropic
   behavior). Prospect researchers often call this "linkage, ability, interest" (LAI): linkage =
   affinity, ability = capacity, interest = propensity. This skill uses capacity, affinity and
   propensity throughout; `nonprofit-major-gifts` adds readiness (timing) when setting the ask.
   Assign a qualification rating (e.g., A/B/C or $ capacity band) and a suggested portfolio owner.
3. **Cultivation** — A sequence of relationship-building moves (1:1 visits, tours, small
   convenings, briefings, volunteer roles) intended to deepen affinity and confirm interest area.
   Each move should have a stated purpose tied to what you still need to learn or build.
4. **Solicitation** — The ask itself. Pipeline work ends at "ready to solicit" and hands off ask
   strategy, amount-setting, and proposal structure to `nonprofit-major-gifts`; for
   pipeline purposes, track only that the ask stage was entered, the date, and the outcome.
5. **Stewardship** — Post-gift relationship maintenance and impact reporting. Pipeline tracking
   should log that a donor moved to stewardship, but acknowledgment workflows, thank-you SLAs, and
   the donor journey itself belong to `nonprofit-donor-retention`.

## Standard Deliverables

1. **Pipeline stage matrix** — columns: Stage, Definition, Entry Criteria, Exit Criteria, Typical
   Duration, Required Moves, Owner. Set explicit time-in-stage caps (e.g., no prospect sits in
   Qualification longer than 90 days without a disposition) so stalls are visible, not implicit.
2. **Portfolio move plan** — per prospect: current stage, last move date, next move (specific
   action + date + purpose), rating, portfolio owner. Standard portfolio size for a major-gift
   officer is 100-150 active prospects (fewer if the portfolio skews principal-gift).
3. **Pipeline/funnel report** — count and $ value of prospects at each stage, converted to a
   funnel visual, run monthly at minimum. Pair with a **stage conversion rate** (% moving
   Identification→Qualification→Cultivation→Solicitation→Closed) to find the leaking stage.
4. **Prospect rating scale** — document the capacity bands and the capacity/affinity/propensity
   scoring rubric used, so ratings
   are consistent across gift officers.

## Concrete Steps

1. Pull all active donor/prospect records and bucket each into exactly one current stage using the
   entry/exit criteria above — do not allow a prospect to sit unassigned.
2. For each prospect with no move logged in the last 60-90 days (a "stalled" prospect), flag for
   triage: either assign a next move with a date, downgrade the rating, or move to a
   low-touch/annual-appeal track (handoff point to `nonprofit-annual-appeals` mass channels).
3. Calculate the pipeline math backward from the goal: if the major-gift goal is $2M and average
   major gift is $25K, you need roughly 80 closed asks; at a typical 30-50% solicitation-to-close
   rate, you need 160-270 prospects actively in Solicitation-ready status, which in turn requires a
   qualification pipeline several multiples larger — build this ratio table explicitly rather than
   asserting a headcount.
4. Assign portfolios by rating and relationship fit, capping each officer near 100-150 prospects.
5. Draft next-move plans: each move must specify purpose (what question it answers or what
   relationship step it advances), not just an activity ("coffee meeting" is not a move; "coffee
   meeting to gauge interest in the new clinic building before drafting a proposal" is).
6. Set a recurring pipeline review cadence (weekly for officers, monthly for the ED/board
   development committee) reporting stage counts, $ value by stage, and stalled-prospect counts.
7. Recalculate conversion rates quarterly and diagnose the weakest stage transition before adding
   more top-of-funnel volume — a common failure mode is chasing more suspects while
   Cultivation→Solicitation conversion is the actual bottleneck.

## Verify Before Acting

Before a pipeline report or portfolio plan ships:

- [ ] Every record sits in exactly one stage, and none is unassigned.
- [ ] Every active prospect has one portfolio owner and a dated next move with a stated purpose.
- [ ] Stalled prospects (no move in 60-90 days) are counted and each has a disposition.
- [ ] Portfolio sizes are near or under the 100-150 cap.
- [ ] Stage counts and $ values by stage sum to the pipeline totals, and the backward pipeline math
  uses the org's own average gift and close rates where available.
- [ ] Donor personal information in the report is limited to what the audience needs.

## Common Failure Modes

- **Ghost pipeline**: prospects listed in the CRM with no stage movement in 6+ months and no
  disposition decision — audit and clear these quarterly.
- **Stage skipping**: soliciting a prospect who was never truly qualified, producing low close
  rates and donor fatigue; enforce exit criteria before allowing a stage transition.
- **Officer hoarding**: gift officers holding oversized portfolios "just in case," diluting
  attention; cap portfolio size and require a reassignment trigger after a set stall period.
- **No move specificity**: "keep in touch" logged as a move — reject vague moves; require a stated
  purpose and next action date.
- **Training instead of diagnosis**: a client asking for "more major donor training" often has a
  stalled-Cultivation problem that no training fixes. Open with a pipeline health audit (stage
  counts, time-in-stage, conversion rates) before recommending new tactics.
- **Conflating qualification with wealth alone**: capacity without affinity or propensity produces
  wasted cultivation time; always score all three axes (capacity, affinity, propensity).

## For advisors

- Present findings to the board/ED as a funnel diagram with the weakest transition highlighted, and
  frame recommendations as capacity questions ("you have enough suspects; you lack qualification
  bandwidth") rather than generic best-practice lists.
- Recommend formalizing the stage matrix and portfolio caps in a written gift officer job aid — the
  unwritten pipeline is the single most common root cause of inconsistent major-gift performance in
  small-to-mid shops.
