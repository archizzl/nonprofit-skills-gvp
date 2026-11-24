---
name: nonprofit-grant-research
description: "Finds and vets foundation, government and corporate grant funders: prospect research and fit scoring, 990-PF giving checks, funder database searches (Candid/Foundation Directory, grants.gov, state portals), RFP/NOFO tracking, and a grant calendar of deadlines and renewals. Use when a user says 'find foundations that fund our program', 'is this funder a good fit?', 'build us a grants calendar' or 'which funders are due for renewal?'. Not for writing the LOI or proposal (use nonprofit-grant-writing) or corporate sponsorship and cause marketing (use nonprofit-corporate-sponsorships)."
license: MIT
metadata:
  supervision: "unsupervised"
  supervision_note: "Prospect research and calendars; a wrong entry costs a look."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Grant Prospect Research & Pipeline Tracking

## Boundaries

- Stop at "we should apply to this funder for this program by this date" and hand off to
  `nonprofit-grant-writing` for drafting, with the funder profile brief attached.
- Cause-marketing and sponsorship engagement with businesses: `nonprofit-corporate-sponsorships`.

## Funder Types & Sources

- **Private/family foundations** — search via Candid's Foundation Directory Online (FDO), the
  foundation's own 990-PF (public on ProPublica's Nonprofit Explorer or Candid), and its published
  guidelines/annual report. 990-PFs disclose actual grants made in the prior year — the single best
  source for confirming true grant size and true funding priorities versus stated ones.
- **Community foundations** — often regionally restricted; check geographic eligibility first, a
  common instant disqualifier.
- **Corporate foundations/giving programs** — check both the corporate foundation (often has its
  own 990) and separate corporate giving/CSR programs, which may have different eligibility rules;
  cause-marketing/sponsorship engagement is a different track (`nonprofit-corporate-sponsorships`)
  from a corporate foundation's grant program.
- **Government grants** — federal via grants.gov (search by CFDA/Assistance Listing number) and
  agency-specific NOFOs; state/local via each state's grants portal; these carry compliance
  obligations (2 CFR 200 Uniform Guidance, indirect cost rate rules) heavier than most private
  funders — flag this distinction for the writing/finance team early, and confirm the current
  text of 2 CFR 200 at eCFR rather than relying on a remembered version.
- **Donor-advised fund and giving-circle referrals** — often sourced through board/staff
  relationships rather than databases; log these in the same pipeline even though discovery method
  differs.

## Funder Fit Scoring

Score each candidate funder on a simple weighted rubric before adding to the active pipeline:

1. **Mission/priority alignment** — does the funder's published priority area explicitly match
   your program, not just adjacent language?
2. **Geographic eligibility** — confirm service area match; this is the most common instant
   disqualifier and should be checked first to avoid wasted research time.
3. **Grant size fit** — compare the funder's typical/median grant size (from 990-PF history or FDO
   data) to what you'd realistically request; a funder whose median gift is $5K is a poor target
   for a $100K ask.
4. **Applicant eligibility** — org type, budget size floor/ceiling, years of operation, prior
   relationship requirements (some funders are invitation-only or require a prior LOI relationship).
5. **Funding cycle timing** — does their next open cycle align with your program's funding need
   timeline?
6. **Relationship strength** — existing board/staff connection to a program officer or trustee,
   which materially raises win probability beyond a cold application.

Assign each factor a score (e.g., 0-2) and set a minimum threshold (e.g., 8/12) before committing
research and writing time — this keeps the team from chasing prestigious but poor-fit funders.

Example row (illustrative funder, not real data):

| Funder | Mission | Geography | Size fit | Eligibility | Timing | Relationship | Total | Decision |
|---|---|---|---|---|---|---|---|---|
| [Example Family Foundation] | 2 (funds early literacy explicitly) | 2 (county in service area) | 1 (median grant below ask) | 2 | 1 (cycle opens after need date) | 0 (no contact) | 8/12 | Add; request a smaller first grant |

## Standard Deliverables

1. **Funder prospect list** — funder name, type, typical grant range, priority areas, geographic
   restriction, application process (LOI-gated vs. open, invitation-only), fit score, next
   deadline, relationship owner.
2. **Grant calendar** — a rolling 12-18 month view of LOI deadlines, full-proposal deadlines,
   decision dates, and report due dates for every funder in the active pipeline (both prospective
   and currently funded) — this is the shared planning tool that keeps writing capacity from being
   blindsided by clustered deadlines.
3. **Funder profile brief** — for a shortlisted funder: giving history (last 3 years of actual
   grants from 990-PF/FDO), current priorities and any recent strategy shifts, key contacts
   (program officer, trustees), application requirements, and a fit-score rationale.
4. **Renewal tracker** — currently funded relationships with renewal eligibility date, whether a
   report is required before reapplication, and historical grant size trend per funder.

## Concrete Steps

1. Define the search brief: program area, requested amount range, geography, and eligibility
   constraints (budget size, years incorporated, 501(c)(3) status).
2. Search Candid/FDO, grants.gov/state portals, and 990-PF filings for candidates matching the
   brief; also mine peer organizations' publicly listed funders (often on their own annual reports
   or websites) as leads.
3. Pull each candidate's actual grant history (990-PF or annual report) to verify stated priorities
   against actual giving — funders often fund more narrowly in practice than their website implies.
4. Score each candidate on the fit rubric; drop anything below threshold before investing further
   research time.
5. Build the funder profile brief for each qualifying candidate.
6. Add every deadline (LOI, full proposal, report) to the shared grant calendar immediately —
   deadlines discovered but not calendared are the most common cause of missed opportunities.
7. Flag capacity conflicts: if three proposals cluster in the same two-week window, escalate to
   the development lead to sequence or reassign drafting before it becomes a crisis.
8. Review the renewal tracker quarterly; flag any funded relationship approaching its
   renewal-eligibility window with no report yet filed.
9. Hand off qualified, calendared opportunities to `nonprofit-grant-writing` with the funder
   profile brief attached.

## Common Failure Modes

- **Priority-matching on website language alone**: funders' public priority statements often lag
  or overstate actual giving patterns; always cross-check the 990-PF grant list.
- **Ignoring geographic/eligibility gates**: wastes research and writing time on ineligible
  funders — screen this first, always.
- **No shared calendar**: deadlines living only in one researcher's head or inbox, causing missed
  submissions when that person is out.
- **Chasing prestige over fit**: pursuing a well-known foundation with a poor size/geography match
  instead of a strong-fit, lower-profile funder.
- **Cold prospecting before mining renewals**: many clients have an underused pipeline of good-fit
  renewal or lapsed funders that outperforms cold prospecting; review it before chasing new names.
- **Stale funder data**: reusing a funder profile from 2+ years ago without checking for new
  leadership, strategy pivots, or closed funding cycles.

## For advisors

- Build the fit-scored prospect list and grant calendar as the first deliverable before
  recommending any specific new funder chase.
- Translate findings into a writing-capacity plan (how many LOIs/proposals per month staff time
  supports) so the prospect list does not outgrow what the client can execute.
