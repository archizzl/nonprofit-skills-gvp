---
name: nonprofit-capital-campaigns
description: "Plans and runs capital campaigns: feasibility studies, gift range tables, campaign phases (planning, quiet, public, close), campaign chair and cabinet structure, and public launch. Use when a user says 'can we realistically raise $5M?', 'build a gift range table for our campaign goal', 'plan our quiet phase before public launch' or 'structure a campaign cabinet'. Not for routine annual fundraising (use nonprofit-annual-appeals), the mechanics of an individual ask within the campaign (use nonprofit-major-gifts), or prospect stage tracking (use nonprofit-donor-pipeline)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Gift tables and feasibility findings set a public goal you must hit."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Capital Campaigns

## Boundaries

- Routine annual-fund operations: `nonprofit-annual-appeals`. Coordinate the two calendars so the
  same donors are not over-solicited.
- Ask amount, proposal and gift agreement for any single campaign gift: `nonprofit-major-gifts`.
- Prospect qualification and stage tracking behind the gift table: `nonprofit-donor-pipeline`.

This skill uses four phase names throughout: **planning**, **quiet**, **public**, and **close**.

## Feasibility Study

Before committing to a public goal, conduct a feasibility study — typically run by an outside
consultant to get candid input current staff/board relationships may not surface:

1. Draft a **case for support** (draft, not final) describing the proposed project and preliminary
   goal.
2. Identify 15-30 key stakeholders (top prospects, board members, community leaders) for
   confidential one-on-one interviews.
3. Ask about: reaction to the case, perceived campaign goal realism, willingness to give and at
   what approximate level, willingness to serve in campaign leadership, and candid concerns about
   organizational readiness or leadership.
4. Synthesize findings into a feasibility report: recommended goal (often adjusted down from the
   aspirational number), leadership candidates identified, case-for-support refinements needed, and
   a readiness assessment (is the board/staff capacity actually sufficient to run a multi-year
   campaign).
5. A feasibility study finding that fewer than roughly a third of interviewees express willingness
   to give a lead-level gift, or that no viable campaign chair emerges, is a signal to delay or
   rescope the campaign rather than proceed on the original goal.

## Gift Range Table

Most of the goal comes from very few gifts. Construct the table by working backward from the goal:

1. Set the lead gift at roughly 10-20% of the total goal (a single largest gift).
2. Build subsequent tiers, each roughly half the previous tier's gift size, with the number of
   gifts needed per tier increasing as size decreases (a common rule of thumb: you need
   meaningfully more prospects than gifts needed at each tier, since not every solicited prospect
   at a given level converts).
3. Confirm via the feasibility study and pipeline audit (`nonprofit-donor-pipeline`) that enough
   qualified prospects actually exist at each tier — a gift table is a planning tool, not a wish
   list; if the top 2-3 tiers have no identified prospect at all, the goal is not yet real.
4. Present the completed table to the board as the campaign's core planning document, since it
   drives both prospect assignment and the leadership solicitation order (leadership/cabinet
   members give first, at the top tiers, before any external solicitation begins).

### Output template: gift range table

Illustrative layout only; fill amounts and counts from the org's goal, feasibility results and
pipeline.

| Tier | Gift amount | Gifts needed | Prospects needed | Named prospects | Tier total | Cumulative total | % of goal |
|---|---|---|---|---|---|---|---|
| Lead | [10-20% of goal] | 1 | [org ratio x gifts] | [names] | [ ] | [ ] | [ ] |
| 2 | [~half of lead] | [ ] | [ ] | [names] | [ ] | [ ] | [ ] |
| 3 | [~half of tier 2] | [ ] | [ ] | [names] | [ ] | [ ] | [ ] |
| ... | ... | ... | ... | ... | ... | ... | ... |
| Below [amount] | Many | [ ] | [ ] | [segments] | [ ] | [goal] | 100% |

## Campaign Phases

1. **Planning** — case development, feasibility study, campaign leadership recruitment,
   internal (board/staff) gifts secured first — internal giving participation (ideally 100% of
   board) is a credibility signal used throughout the rest of the campaign.
2. **Quiet** — solicitation of lead and major gifts (top tiers of the gift table) before any public
   announcement; campaigns commonly aim to have 50-70%+ of the goal committed before public launch,
   since public momentum depends on visible early success.
3. **Public** — public announcement/launch event, broader donor base solicitation (mid-level
   and annual-fund-level asks), public progress reporting (e.g., a campaign thermometer), and
   community-wide engagement.
4. **Close** — final gift push to close any remaining gap, campaign close event,
   donor recognition (naming installations, donor walls), and transition of any campaign-specific
   staff/systems back to regular operations.

## Campaign Leadership Structure

- **Campaign chair(s)** — must make or secure their own lead gift and personally solicit other
  top-tier prospects; chair selection is often the single biggest determinant of quiet-phase
  success. Willingness to give visibly and ask peers matters more than general prominence.
- **Steering committee/cabinet** — divides responsibility by gift tier or constituency (major gifts,
  corporate/foundation, community); members are expected to give and get.
- **Staff campaign director** — coordinates logistics, prospect tracking, and materials; volunteer
  leadership drives relationships and asks.

## Standard Deliverables

- **Feasibility study report** with recommended goal and leadership candidates.
- **Case for support** (campaign-specific, more detailed than an annual case).
- **Gift range table** tied to identified prospects per tier.
- **Campaign timeline** across all four phases with named milestones.
- **Campaign leadership org chart** (chair, cabinet, staff roles).
- **Progress dashboard** — cumulative $ committed vs. goal, by phase and by tier, updated
  regularly for the board and campaign cabinet.

## Concrete Steps

1. Commission or run the feasibility study (above) before setting a public goal.
2. Build the gift range table and cross-check it against the actual qualified pipeline.
3. Recruit campaign chair(s) and steering committee, prioritizing chairs who can personally lead
   with a top-tier gift.
4. Secure 100% board participation and other internal (staff, close-in) gifts first.
5. Run the quiet phase: solicit top-tier prospects using major-gift mechanics
   (`nonprofit-major-gifts`) in the order the gift table implies (top tier first).
6. Set the public-launch threshold (commonly 50-70% of goal committed) before announcing publicly;
   do not launch publicly on a weak quiet-phase result.
7. Execute the public phase: launch event, expanded solicitation to mid-level/annual donor
   segments, progress communication.
8. Track cumulative progress against the gift table continuously; if a tier is underperforming,
   reallocate prospects or adjust the ask sequence rather than waiting until the campaign closes.
9. Plan and execute the closing push and recognition/celebration event; formally close the
   campaign with a final report to the board and donors.

## Verify Before Acting

Before presenting a goal to the board or announcing it publicly:

- [ ] The feasibility study supports the goal (lead-level willingness and a viable chair emerged).
- [ ] The gift range table foots to the goal, and the lead gift sits at roughly 10-20% of it.
- [ ] The top 2-3 tiers each have named, qualified prospects in the pipeline.
- [ ] Board participation is at or near 100% before external solicitation begins.
- [ ] For a public launch, committed gifts meet the threshold set in step 6 (commonly 50-70%).
- [ ] The campaign calendar has been reconciled with the annual appeal calendar.

## Common Failure Modes

- **Skipping feasibility**: setting a goal from aspiration rather than tested donor willingness,
  producing a public shortfall.
- **Launching publicly too early**: going public before the quiet phase has secured enough of the
  goal, losing the momentum effect that public campaigns depend on.
- **Weak internal giving**: soliciting external donors before securing full board participation,
  undermining credibility ("why would I give if your own board hasn't").
- **Gift table with no real prospects at the top tiers**: a table built on hope rather than an
  actual qualified pipeline.
- **No dedicated campaign leadership**: relying on staff alone to solicit top gifts instead of
  recruiting peer volunteer leadership, which typically converts at higher rates for major asks.
- **Campaign fatigue on the annual fund**: failing to explicitly coordinate campaign solicitation
  with the regular annual appeal calendar, over-soliciting the same donors and depressing both
  results.

## For advisors

- Advisors are often engaged to run the feasibility study, since candid donor input is more
  reliable when gathered by a neutral outside party.
- Present feasibility findings to the board even when unwelcome (a lower goal or a delay); the core
  value is preventing a launch the donor base cannot support.
- Make the progress dashboard a standing board agenda item for the campaign's duration so
  governance stays engaged between launch and close.
