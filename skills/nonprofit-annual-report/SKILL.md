---
name: nonprofit-annual-report
description: "Plans and structures a nonprofit annual report: section architecture, impact highlights, a lay-reader financial summary, donor recognition, and print vs. digital format. Use when asked to \"outline our annual report,\" \"write the ED/board chair letter,\" \"structure our donor honor roll,\" or \"turn our 990 numbers into a one-page financial summary.\" Not for writing beneficiary narratives (use nonprofit-storytelling), brand voice or the messaging house (use nonprofit-brand-messaging), preparing audited financial statements (use nonprofit-financial-statements), or filing Form 990 (use nonprofit-form-990)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Summarises financials for lay readers; the numbers must match the statements."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Annual Report

## Boundaries

- This skill decides structure, content selection, and framing; it selects and places finished
  beneficiary narratives from `nonprofit-storytelling` rather than writing them.
- Brand voice and visual identity rules: `nonprofit-brand-messaging`.
- The audited statement of activities/financial position: `nonprofit-financial-statements`.
- The Form 990 filing itself: `nonprofit-form-990` (this skill only translates 990/audit numbers
  into lay-friendly summary graphics).

## Standard Deliverable: Annual Report Section Architecture

A complete nonprofit annual report has these sections, in this order, though length should flex to
organization size (a 2-page one-sheet for a small nonprofit still hits each beat in miniature):

1. **Cover + theme.** One sentence or phrase that frames the year (not just "20XX Annual Report") —
   ties every section back to a single narrative thread.
2. **Leadership letter** (Board Chair + ED, jointly signed or paired letters). States the year's
   biggest win, biggest challenge honestly, and forward-looking priority — not a generic thank-you.
3. **Mission/at-a-glance stats.** 3-5 headline numbers (people served, outcome rate, geographic
   reach) — pull from `nonprofit-outcomes-measurement` KPI work, not raw activity counts alone.
4. **Program impact narrative(s).** 1-3 stories or program deep-dives; source finished narratives
   from `nonprofit-storytelling` rather than drafting raw beneficiary quotes here.
5. **Financial summary.** Simplified, visual statement of activities and functional expense
   breakdown (program/admin/fundraising %) — see framing guidance below. Never substitute for or
   contradict the audited financials; numbers must tie to the audit/990.
6. **Donor & supporter recognition.** Giving-society tiers, cumulative/legacy society mentions,
   volunteer and board rosters. Accuracy here is a trust-critical deliverable — a misspelled or
   omitted donor name is a stewardship failure, not a typo.
7. **Board and staff leadership list.** Names, titles; often includes committee chairs.
8. **Call to action + contact/giving info.** How to give, volunteer, or engage next year.

## Financial Summary Framing (Practitioner Technique)

Boards and lay donors misread raw financial statements; the annual report's job is translation, not
duplication:

- Convert the functional expense allocation into a simple donut/bar chart showing Program %,
  Management & General %, Fundraising %, sourced from the audited statement of functional expenses.
  State the methodology briefly ("shared costs allocated by staff time") if allocation isn't obvious.
- Show a 2-3 year trend for total revenue and program expense, not just one year in isolation — a
  single year can mislead (e.g., a one-time bequest inflating revenue).
- Pair the efficiency ratio with a plain-language caveat: a very high program-expense ratio is not
  automatically "better" if it reflects underinvestment in infrastructure — brief the writer to avoid
  implying "lower overhead = better nonprofit," a framing that fuels the overhead myth and can
  pressure future underinvestment.
- Always reconcile: numbers in the annual report must match the audited financials or 990 for the
  same fiscal year; a mismatch (even from good-faith rounding or a different reporting period) is the
  most common credibility failure reviewers catch.

One-page financial summary skeleton (fill only with figures from the audit/990; leave blanks blank):

```
FINANCIAL SUMMARY — Fiscal year ending [date]          Source: [audited statements / Form 990, FY]
Revenue by source            This year    Prior year    Two years ago
  Contributions & grants     $[  ]        $[  ]         $[  ]
  Government grants          $[  ]        $[  ]         $[  ]
  Earned / program revenue   $[  ]        $[  ]         $[  ]
  Other (incl. one-time gifts, noted)  $[  ]  $[  ]     $[  ]
  Total revenue              $[  ]        $[  ]         $[  ]
Expenses by function         $            % of total
  Program services           $[  ]        [  ]%
  Management & general       $[  ]        [  ]%
  Fundraising                $[  ]        [  ]%
Methodology note: [how shared costs were allocated, e.g., by staff time]
Context line: [plain-language caveat on what the ratio does and does not mean]
Tie-out: totals match [audit / 990 line references] for the same fiscal year — checked by [name]
```

## Step-by-Step: Producing the Report

1. Set the fiscal year scope and confirm audited financials/990 data are finalized before drafting
   the financial section — do not build charts off unaudited estimates that may later shift.
2. Choose the year's theme/narrative thread from the top 2-3 organizational wins or turning points.
3. Draft the section architecture (above) as an outline; assign each section a word/space budget.
4. Commission or select 1-3 finished, consent-cleared stories from `nonprofit-storytelling` matched
   to the theme — do not write new beneficiary narratives inside this skill.
5. Build the at-a-glance stats box from validated KPI data (coordinate with
   `nonprofit-outcomes-measurement`); avoid unverifiable or inflated numbers.
6. Draft the leadership letter last, after other sections are drafted, so it can reference specifics.
7. Compile and cross-check the donor recognition list against the CRM export at least twice,
   including a review pass by the development team for spelling, tier accuracy, and honoring "give
   anonymously" flags.
8. Decide print vs. digital/interactive format based on audience: major donors and board often expect
   a printed piece for stewardship value; general/younger audiences engage more with a scrollable web
   version. Default to one content set; produce both formats only when the donor mix and budget
   justify the added cost.
9. Route to leadership (ED + Board Chair) and at least one non-marketing board member for review
   before final design lock — catches factual and tone issues fresh eyes miss.

## Common Failure Modes

- **Donor list errors** (misspelled names, wrong giving tier, omitted "anonymous" request) — the
  single most damaging mistake because it's visible to the exact audience being stewarded.
- **Financial section that doesn't reconcile** to the audit/990, or invents a "cleaner" number.
- **Overhead-ratio bragging** that undermines future donor understanding of the true cost of
  infrastructure and talent.
- **Generic stock-photo stories** with no connection to actual program data — annual reports lose
  credibility fast when impact claims aren't backed by specific numbers or named (consented) stories.
- **All-narrative, no-data** or **all-data, no-narrative** imbalance — funders and major donors
  typically want both; a report that's 90% donor thank-yous with no program substance reads as a
  purely promotional piece rather than an accountability document.
- **Late financial data** forcing a rushed reconciliation or a "preliminary/unaudited" disclaimer that
  undercuts trust — sequence audit completion before annual report finalization in the planning
  calendar.

## For advisors

- Frame the annual report as an accountability and stewardship instrument for the board, not just a
  marketing artifact; run the "does this reconcile" and "overhead myth" checks as part of a
  governance-quality review.
