---
name: nonprofit-executive-dashboard
description: "Designs a one-page ED/COO KPI dashboard and a matching quarterly board scorecard: picks 8-15 cross-functional KPIs, balances leading and lagging indicators, sets targets and yellow/red thresholds, names owners and data sources, and sets review rhythms. Use when someone says 'design our ED dashboard,' 'our board scorecard has 40 metrics, cut it down,' or 'what leading indicators should we track.' Not for the financial statements (use nonprofit-financial-statements), program outcome design (use nonprofit-outcomes-measurement), full EOS rollout (use nonprofit-eos-traction), the strategic plan (use nonprofit-strategic-planning), or the CEO's board narrative (use nonprofit-ceo-board-partnership)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Board-facing KPIs drive decisions; a wrong indicator misdirects the org."
  last_reviewed: "2026-09-07"
  date_added: "2026-09-07"
  date_added_source: "git:34f6bfb6b4bc8cabe1683622f7fc16704d6a80b9"
---

# Nonprofit Executive Dashboard

## Boundaries

This skill designs the dashboard *system* — metric selection, targets, thresholds, owners,
layouts, and review rhythms — not the underlying data.

- Financial statements that feed the finance KPIs: `nonprofit-financial-statements`.
- Program outcome indicators, theory of change, evaluation methodology:
  `nonprofit-outcomes-measurement` (this skill *pulls from* those indicators but does not design
  them).
- Installing EOS across the organization (V/TO, L10, Rocks, People Analyzer):
  `nonprofit-eos-traction`; this skill borrows only the scorecard discipline.
- The strategic plan the dashboard measures: `nonprofit-strategic-planning`.
- The CEO's narrative board report that *uses* this dashboard: `nonprofit-ceo-board-partnership`.

## Core Framework: Two Dashboards, Not One

The single most common failure is one dashboard trying to serve both the leadership team and the
board. They have different jobs, different time horizons, and different audiences — split them:

- **ED/COO operational dashboard**: 8–15 KPIs, reviewed monthly by the leadership team (weekly for a
  smaller "pulse" subset). Answers "are we on track this quarter?" Includes leading indicators the
  team can *act on* between meetings. Owned by the ED.
- **Board scorecard**: 5–8 KPIs, reviewed quarterly by the board. Answers "is the organization
  healthy and on strategy?" Skews toward lagging outcome and financial-health indicators, plus a
  narrative on the one or two things that matter most this quarter. Owned by the board chair with
  the ED.

If the board is looking at monthly cash disbursements by vendor, the governance/management line is
broken (see `nonprofit-board-governance`). If the ED's team is only looking at quarterly
lagging outcomes, they cannot steer.

## Frameworks and Defaults

- **Balanced Scorecard, adapted for mission**: four perspectives — **mission impact** (replaces
  "customer" as the top perspective), **financial health**, **stakeholder/constituent**, and
  **learning & growth (people/culture)**. Force at least one KPI per perspective so the dashboard
  cannot silently collapse into all-finance or all-output-counts.
- **Finance panel — default: Nonprofit Finance Fund indicators**: **months of cash / liquid
  unrestricted net assets (LUNA)**, **operating reliance** (share of expenses covered by reliably
  renewable revenue), **debt ratio**, and **operating surplus/deficit margin**. These are the
  finance floor for any ED dashboard. Alternative: Propel Nonprofits' balance-sheet +
  income-statement indicators (receivables aging, revenue composition, expense mix, change in net
  assets) when the finance panel needs more than a single "months of cash" number.
- **Scorecard discipline (Rockefeller Habits / EOS)**: every KPI has a **named human owner**, an
  actual number entered on cadence, and a red/yellow/green status — reviewed at a standing
  leadership meeting. The point is the review meeting that closes the loop, not the spreadsheet.
- **Leading indicators**: a dashboard with no leading indicators is a rearview mirror. Nonprofit
  examples: stage-weighted major gift pipeline, grant proposals submitted this month, staff eNPS,
  program waitlist growth. Aim for at least one leading indicator per perspective.
- **Targets set before the period starts**, never reverse-engineered from what was hit.
- **One metric that matters most this quarter**: a single north-star KPI per quarter (or per
  strategic priority) that both the leadership team and board watch.

## Numbered Checklist: Building the Dashboard

Follow in order — skipping steps is what produces the failure modes below.

1. **Start from the strategic plan**, not from available data. List the 3–5 strategic objectives.
   Every KPI must trace to an objective; if it doesn't, cut it or cut the objective.
2. **Brainstorm candidate indicators per Balanced Scorecard perspective** — mission impact,
   financial, stakeholder, learning & growth. Expect 30–50 candidates.
3. **Cut to 8–15 KPIs for the ED dashboard, and 5–8 for the board scorecard.** More than 15 and the
   monthly review becomes a status readout instead of a decision meeting.
4. **Tag each KPI leading or lagging.** If the dashboard is more than ~70% lagging, add leading
   indicators until every perspective has at least one.
5. **Set a SMART target and yellow/red thresholds for each KPI** (e.g., green ≥ 3 months of cash,
   yellow 1.5–3, red < 1.5). Thresholds are what trigger action — no threshold, no trigger, no
   action.
6. **Assign a single named owner per KPI** (not "Finance" — the CFO by name). The owner is
   accountable for the number appearing on time and for narrating variance.
7. **Pick the authoritative data source and cadence per KPI** — one system of record per metric,
   documented, so two people never report different numbers for the same KPI.
8. **Design the one-page layout**: group by Balanced Scorecard perspective, show target vs. actual
   vs. threshold status, sparkline or trend arrow for direction, and reserve the top-right for the
   "one metric that matters most this quarter." Pick the chart form to match the question — trend
   line for direction over time, bullet chart for actual vs. target vs. threshold, stacked bar for
   composition (e.g., revenue mix), gauge only if a bounded % vs. threshold is what a non-analyst
   viewer must grasp in three seconds.
9. **Wire the review rhythm**: monthly leadership-team review of the full ED dashboard on a standing
   agenda (see below); optional weekly 15-minute pulse on a 3–5 KPI subset; quarterly board
   scorecard review at the regular board meeting.
10. **Schedule the annual reset** (see checklist below) at the same time each year, right after the
    strategic plan is refreshed and the next-year budget is approved.

## Standard Deliverables

- **One-page ED/COO KPI dashboard** grouped by Balanced Scorecard perspective, with target, actual,
  threshold status, trend, and the quarter's north-star metric highlighted.
- **Board scorecard** (fewer metrics, longer time horizon — typically trailing 4–8 quarters shown),
  paired with the CEO narrative from `nonprofit-ceo-board-partnership`.
- **KPI definitions document**, one row per KPI: name, plain-English definition, exact formula,
  system of record, owner (by name), cadence, target, yellow/red thresholds, leading/lagging tag,
  strategic-objective link. Format (rows are placeholders, not benchmarks):

  | KPI | Definition / formula | System of record | Owner | Cadence | Target | Yellow / red | Lead/lag | Objective |
  |-----|----------------------|------------------|-------|---------|--------|--------------|----------|-----------|
  | Months of cash | Unrestricted cash ÷ avg monthly expenses | Accounting system | [CFO name] | Monthly | [ ] | [ ] / [ ] | Lag | [ ] |
  | Weighted major gift pipeline | Sum of ask × stage probability | Donor CRM | [Dev director] | Monthly | [ ] | [ ] / [ ] | Lead | [ ] |
  | Staff eNPS | Pulse survey score | HR survey tool | [HR lead] | Quarterly | [ ] | [ ] / [ ] | Lead | [ ] |
- **Leadership-team monthly review agenda**: quick red/yellow scan (5 min) → focused discussion of
  every red and any newly-yellow KPI, owner narrates variance and proposed action (30–40 min) →
  north-star metric deep-dive (10 min) → decisions and owners captured. Reviews of green items are
  skipped by default.
- **Quarterly OKR set aligned to the strategic plan** — 3–5 objectives, 2–4 key results each,
  explicitly cross-referenced to the dashboard KPIs that measure them.
- **Annual dashboard reset checklist**: re-confirm strategic objectives; retire KPIs that no longer
  tie to an objective or no longer drive action; add KPIs for any new objective; rebaseline targets
  and thresholds against the new budget; confirm owners and data sources; refresh the one-page
  layout; recommit to the review rhythm on the calendar.

## Verify Before Acting

Before the dashboard or board scorecard goes to the leadership team or board:

- [ ] Every KPI traces to a named strategic objective; untraceable KPIs are cut.
- [ ] Every KPI has a named owner (a person), one system of record, a cadence, a target, and
      yellow/red thresholds.
- [ ] Each Balanced Scorecard perspective has at least one KPI and at least one leading indicator.
- [ ] Counts hold: 8–15 KPIs on the ED dashboard, 5–8 on the board scorecard, one north-star metric.
- [ ] Finance KPI values reconcile to the latest financial statements from the finance lead.
- [ ] Program indicators match the definitions used in `nonprofit-outcomes-measurement` work.

## Common Failure Modes

- **Too many metrics / vanity-metric bloat** — a 40-KPI dashboard is a report, not a decision tool.
- **Board scorecard = ED dashboard** — governance/management line broken. Split them and defend
  the split (see `nonprofit-board-governance`).
- **No thresholds** — everything is a number with no red/yellow/green, so nothing ever triggers
  action. Set thresholds or the review meeting devolves into narration.
- **No named owner per KPI** — "Finance owns it" means no one owns it. Assign a human by name.
- **Data source ambiguity** — two people report different numbers for the same KPI because they
  pulled from different systems. Name one system of record per metric in the KPI definitions doc.
- **Dashboard never revisited** — the strategic plan evolved, the dashboard didn't, and the two
  drift apart. Run the annual reset on a fixed calendar date.
- **Conflating a plan with a scorecard** — the strategic plan lists intended activities; the
  scorecard measures whether they moved the needle. If the "dashboard" is a task list, it is a plan,
  not a scorecard.

## For advisors

- Bring one authored draft (candidate KPIs, targets, thresholds, owners) to the leadership team
  rather than co-designing from a blank page; dashboard-by-committee reliably lands at 30+ metrics.
- Diagnose before designing: tag each current metric leading vs. lagging, map it to an objective,
  and count owners — the gaps name themselves and become the redesign brief.
- Deliver two artifacts (ED dashboard *and* board scorecard) plus the KPI definitions document and
  the review-rhythm calendar, not just a prettier one-pager.
