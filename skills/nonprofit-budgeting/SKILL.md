---
name: nonprofit-budgeting
description: "Builds a nonprofit's annual operating budget: probability-weighted revenue, expenses tagged by program, functional roll-up, choice of budgeting method, board approval calendar and budget-to-actual setup. Use when asked to 'build our operating budget,' 'we need a zero-based budget this year,' 'draft a budget narrative for the finance committee,' or 'set up a budget calendar.' Not for audited financial statements (use nonprofit-financial-statements), reserve targets or cash timing (use nonprofit-reserves-cash-flow), indirect cost rates or shared-cost allocation methods (use nonprofit-cost-allocation), or approval thresholds and internal controls (use nonprofit-financial-controls)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "The board adopts this; errors propagate through the whole year."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Budgeting

## Boundaries

- This skill produces the plan. GAAP-format statements from actuals: `nonprofit-financial-statements`.
- Reserve targets and in-year cash timing: `nonprofit-reserves-cash-flow`.
- Formal indirect cost rates and the shared-cost allocation basis: `nonprofit-cost-allocation`.
- Who approves what dollar threshold: `nonprofit-financial-controls`.

## Core Framework

Build the budget at the account/program level and roll it up to functional categories for external
reporting. Treat it as three linked documents, not one:

1. **Revenue budget** — grants, contracts, individual giving, events, earned income, investment
   income, in-kind — each line tied to a named source or a documented assumption (e.g., "renewal
   probability 80% based on 3-year history").
2. **Expense budget** — built by natural category (salaries, benefits, occupancy, professional fees,
   travel, supplies) *and* tagged by program/department, so it can be re-sliced into functional
   categories.
3. **Functional allocation** — the same expense dollars re-cut into Program Services, Management &
   General, and Fundraising, per FASB ASC 958-720. This is what a board and outside reviewers (Charity
   Navigator, GuideStar/Candid, grantors) will judge.

## Budgeting Methodologies — Choosing and Naming the Approach

- **Incremental budgeting**: prior year actuals ± a percentage adjustment. Fast, low-conflict, but
  perpetuates existing allocation and hides sunk-cost programs. Default for stable organizations.
- **Zero-based budgeting (ZBB)**: every line must be justified from zero each cycle, program by
  program. Surfaces programs that no longer earn their keep; expensive in staff time. Recommend for
  organizations that haven't reassessed program mix in 3+ years, post-merger, or after a major
  revenue shock.
- **Priority-based (a.k.a. Budgeting for Outcomes)**: rank programs against mission/strategic
  priorities first, then fund top-ranked programs fully before funding lower-ranked ones — useful
  when revenue is flat or declining and across-the-board cuts would hurt high-performing programs as
  much as weak ones.
- **Program/activity-based budgeting**: build the budget by program (each with its own mini P&L)
  rather than only by natural expense category — needed once an org has 3+ distinct programs with
  different funding mixes, since it exposes which programs are subsidized by unrestricted revenue.
- **Rolling/multi-year forecast**: 12-month budget plus a 2-3 year projection updated quarterly — pair
  with `nonprofit-strategic-planning` outputs when the board wants the budget to visibly fund
  strategic priorities.

State which method is being used and why; do not silently default to incremental when the
organization's situation (declining revenue, program pruning, post-merger) calls for ZBB or
priority-based.

## Program-vs-Admin-vs-Fundraising Allocation

Tag each cost as direct (one program) or shared, and allocate shared costs on a documented basis
(time studies are the most audit-defensible for split personnel). Use `nonprofit-cost-allocation` for
choosing and documenting the allocation basis and for any formal indirect rate. There is no single
"correct" overhead ratio; benchmark against organizations of similar size/sector rather than a flat
15%/85% rule of thumb, and be ready to explain the ratio's composition rather than just the number.

## Step-by-Step: Building the Annual Budget

1. **Set the calendar.** Work backward from the fiscal year start and the board's final vote date.
   Typical timeline for a June 30 fiscal year end: kickoff/assumptions in February, department/program
   drafts in March, finance committee review in April, board first read in May, board approval in
   June. Adjust similarly for a December 31 fiscal year end.
2. **Set budget assumptions first, in writing** — salary increase %, benefits inflation, known grant
   renewals/losses, new program launches, inflation on occupancy/insurance. Circulate assumptions to
   department heads before they draft numbers so everyone budgets against the same baseline.
3. **Build revenue first, conservatively.** Use a probability-weighted approach for uncommitted
   revenue (committed/contracted = 100%, highly likely = 75-90%, prospective/unconfirmed = 25-50%).
   Never budget to a fundraising goal that has no plan behind it — cross-check every revenue line
   against the development plan/pipeline (see `nonprofit-donor-pipeline` for the underlying pipeline).
4. **Build expenses program-by-program and department-by-department**, tagging each line with the
   program/department it belongs to so the functional roll-up is mechanical, not a re-derivation.
5. **Reconcile to net.** Decide upfront whether the board requires a balanced budget, allows a planned
   deficit funded from reserves (state the dollar amount and reserve impact explicitly — see
   `nonprofit-reserves-cash-flow`), or requires a modest surplus to build reserves.
6. **Run the functional allocation** and check the resulting Program / M&G / Fundraising percentages
   against the prior year and peer benchmarks before it goes to committee — large swings need a
   one-line explanation ready for the board.
7. **Finance committee review.** Expect questions on: variance vs. prior year actuals, any new FTEs,
   assumptions behind the largest revenue lines, and the M&G ratio. Bring a one-page assumptions memo,
   not just the spreadsheet.
8. **Board approval.** Most bylaws require full board vote on the annual budget (check
   `nonprofit-bylaws-policy` if unclear); present a summary page (revenue by source, expense by
   function, net, reserve impact) plus the detail as an appendix — do not hand the board the full
   general-ledger-level workbook as the primary document.
9. **Set up budget-to-actual monitoring** — monthly or quarterly variance reports against this
   approved budget, with a defined threshold (e.g., >10% or >$5,000 variance) that triggers a written
   explanation to the finance committee.
10. **Amend formally when needed.** A material shift (new large grant, lost major funder, unplanned
    hire) should go back to the board or finance committee as a budget amendment, not be silently
    absorbed — keep an amendment log for audit trail.

## Board Budget Summary Template

```
[Organization] Operating Budget, FY [year] (for board vote on [date])
Method: [incremental / zero-based / priority-based] because [reason]

| Revenue by source        | Prior-yr actual | Proposed | Change | Basis (committed / weighted %) |
|--------------------------|-----------------|----------|--------|--------------------------------|
| Government grants/contracts |              |          |        |                                |
| Foundation grants        |                 |          |        |                                |
| Individual giving        |                 |          |        |                                |
| Events / earned income   |                 |          |        |                                |
| Total revenue            |                 |          |        |                                |

| Expense by function      | Prior-yr actual | Proposed | % of total |
|--------------------------|-----------------|----------|------------|
| Program services         |                 |          |            |
| Management & general     |                 |          |            |
| Fundraising              |                 |          |            |
| Total expense            |                 |          |            |

Net surplus / (deficit): [amount]
Reserve impact: [drawdown or addition; months of reserve after] (see reserve policy)
Key assumptions: [3-5 bullets from the assumptions memo]
Requested action: [motion text]
```

## Standard Deliverables

- Budget assumptions memo (1 page)
- Revenue detail by source with probability weighting
- Expense detail by natural category, tagged by program/department
- Functional expense summary (Program / M&G / Fundraising %)
- Board-facing budget summary (1 page) + full detail appendix
- Budget calendar with named owners and dates
- Budget-to-actual variance report template (monthly/quarterly)

## Verify Before Acting

- [ ] Every revenue line names a source or pipeline entry and a probability weight; no line is a bare goal.
- [ ] The assumptions memo figures (salary %, benefits, renewals) match the numbers in the workbook.
- [ ] Functional roll-up totals equal the natural-category expense total.
- [ ] Any deficit states the dollar amount and is checked against the reserve policy
      (`nonprofit-reserves-cash-flow`).
- [ ] Program / M&G / Fundraising swings vs. prior year have a one-line explanation.
- [ ] The approval path (committee, full board vote) matches the bylaws before the packet goes out.

## Common Failure Modes

- Budgeting revenue to a fundraising *goal* rather than a *pipeline* — creates a mid-year crisis when
  the gap surfaces in month 8.
- No written assumptions, so a board member's "why did salaries jump 12%?" has no ready answer.
- Treating the functional allocation as an afterthought done only for the 990, instead of building it
  into the budget structure from day one — this causes a scramble every year and inconsistent
  methodology year to year.
- No variance monitoring cadence set at approval time, so the board only learns of a problem at
  year-end.
- Approving a deficit budget without an explicit reserve drawdown plan and reserve-policy check.
- Dumping all occupancy, IT, and admin salaries into Management & General without allocation, which
  inflates the reported overhead ratio and triggers funder/watchdog scrutiny (Charity Navigator and BBB
  Wise Giving Alliance both flag high M&G ratios). Fix by allocating a reasonable share of shared costs
  to programs based on actual usage.
- Over-allocating to programs to make the overhead ratio look artificially low; this fails an audit or
  a funder cost review when the allocation basis isn't documented and reproducible. Every allocation
  percentage must be traceable to a stated method (see `nonprofit-cost-allocation`).

## For advisors

- Frame budget review as a governance and strategy conversation: is the functional allocation
  defensible to funders and watchdogs, and does the revenue mix match the strategic plan's priorities?
- Push back diplomatically on incremental "add 3% to everything" budgets when revenue decline or
  program underperformance calls for zero-based or priority-based budgeting.
