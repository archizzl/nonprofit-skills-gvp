---
name: nonprofit-board-governance
description: "Designs how a seated nonprofit board works: meeting structure and consent agendas, committee charters, board self-assessment, board-vs-staff decision lines, board job descriptions and the board side of ED evaluation. Use when asked 'our board meetings run long and nothing gets decided,' 'what committees should our board have,' 'run a board self-assessment,' or 'the board keeps micromanaging staff.' Not for recruiting or onboarding new members (use nonprofit-board-recruitment), bylaws or COI/whistleblower/retention policy text (use nonprofit-bylaws-policy), Form 990 governance disclosures (use nonprofit-form-990), or the CEO's own board reports, self-eval and chair 1:1s (use nonprofit-ceo-board-partnership)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Internal process design; consequential but not externally filed."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Board Governance

## Boundaries

This skill assumes the board already exists.

- Recruitment matrix, cultivating and onboarding new members: `nonprofit-board-recruitment`.
- Legal text of bylaws, conflict-of-interest, whistleblower and document retention policies:
  `nonprofit-bylaws-policy` (this skill references those policies operationally but does not draft them).
- Form 990 Part VI governance disclosures: `nonprofit-form-990`.
- The CEO/ED's own side of the relationship (board report, self-evaluation memo, chair 1:1 agendas,
  exec-session prep): `nonprofit-ceo-board-partnership`. This skill designs the board's evaluation process.

## Core Framework: Governance vs. Management

Use the governance/management line to diagnose almost every board complaint. A board that debates which
vendor to use for the office copier is doing management, not governance; redirect it. Conversely, an ED
who sets strategic direction without board sign-off has flipped the line the other way. Two named models
operationalize the split:

- **Policy Governance / "Carver model"** (John Carver): the board writes **Executive Limitations**
  policies (what the ED may *not* do — e.g., "the ED shall not allow financial conditions that
  jeopardize solvency") and **Ends policies** (what results the organization exists to produce for
  whom, at what cost), then monitors the ED's compliance against those written limits rather than
  approving each operational decision.
- **Consensus/traditional model**: board approves budgets, major contracts, and policies directly by
  vote at meetings — more common in smaller and mid-size nonprofits than full Carver adoption.

Name which model (or hybrid) a client/organization is using before recommending agenda structure or
delegation language — the advice differs materially between them. Default: if the board has not adopted
written Ends and Executive Limitations policies, treat it as the traditional model.

## Meeting Structure and Agendas

1. **Consent agenda** — bundle routine, non-controversial items (prior minutes, standard reports,
   routine policy renewals) into a single motion voted on without discussion, freeing meeting time
   for strategic topics. Any board member can pull an item off the consent agenda for discussion
   before the vote.
2. **Agenda design principle**: order items by decision importance, not chronology — put the highest
   -stakes strategic discussion when the board is freshest (early-to-mid meeting), not last after
   attention has degraded.
3. **Standard agenda skeleton**: call to order/quorum check → consent agenda → ED report (narrative,
   not just numbers) → committee reports (by exception — only flag items needing board action) →
   old business → new business/strategic discussion → executive session (if needed) → adjourn.
4. **Timeboxing**: assign a minute allocation to every agenda item in advance and appoint a
   timekeeper; a board packet sent 5-7 days ahead (not at the meeting) is the single biggest lever for
   shortening meetings, since members arrive prepared instead of reading materials live.
5. **Executive session**: reserve time without staff present for sensitive topics (ED evaluation,
   legal matters, compensation) — minute only that a session occurred and its general subject, not
   full discussion detail, unless legally required otherwise.
6. **Quorum and voting**: confirm the bylaws-defined quorum and any supermajority requirements (e.g.,
   removing a director, amending bylaws) before convening a vote — check `nonprofit-bylaws-policy` or
   the organization's actual bylaws for the exact figures, since this skill does not draft them.

## Committee Design

Common standing committees and what each actually owns:

- **Executive Committee** — acts with delegated authority between meetings on time-sensitive matters
  only; should not become a shadow board that pre-decides everything before the full board sees it.
- **Finance Committee** — budget development oversight, financial statement review, recommends
  reserve levels; distinct from the Audit Committee where org size allows separation (small boards
  often combine Finance + Audit, which creates an independence tension worth flagging to a client).
- **Audit Committee** — auditor selection, oversight of the audit process, and receiving the
  management letter directly, ideally with no staff (including the ED/CFO) as voting members, to
  preserve independence (see `nonprofit-financial-controls` for the audit process itself).
- **Governance/Nominating Committee** — board self-assessment administration, board matrix
  maintenance, slate development for new members (recruitment details in
  `nonprofit-board-recruitment`), and orientation.
- **Development/Fundraising Committee** — board fundraising participation and accountability, not
  execution of the annual fund itself.
- **Program/Impact Committee** — deeper-dive oversight of outcomes and evaluation data feeding board
  monitoring, without taking over program management decisions.

Every committee needs a **written charter**: purpose, authority (recommends to full board vs. can
act independently), membership/chair term, and reporting cadence — an unwritten charter is why
committees drift into duplicating or contradicting each other.

```
[Committee name] Charter — adopted [date] by board vote
Purpose: [one sentence on what this committee oversees]
Authority: [recommends to full board | may act on: ___ (cite bylaws section)]
Membership: [number] directors; [non-director members allowed? voting?]
Chair: appointed by [board chair | board]; term [length]; renewable [yes/no]
Staff liaison: [title] (non-voting)
Meetings: [frequency]; quorum [per bylaws or majority of members]
Responsibilities:
- [annual task 1, with month due]
- [annual task 2]
Reporting: to full board [each meeting | by exception]; minutes filed with [secretary]
Annual review: charter reviewed by Governance Committee each [month]
```

## Board Self-Assessment

Run annually or every 2 years, separate from individual board member performance review:

1. Distribute a confidential written self-assessment survey covering: understanding of mission/
   fiduciary duty, meeting effectiveness, committee functioning, ED-board relationship quality,
   fundraising participation, and board composition/diversity gaps.
2. Aggregate anonymously; never attribute individual responses in the full-board readout.
3. Present findings to the Governance Committee first, then a summary with an action plan to the
   full board — a self-assessment with no resulting action item is a wasted cycle and a common
   funder/rating-agency red flag (e.g., in due diligence questionnaires).
4. Feed composition gaps identified (skills, sector experience, lived experience, demographics)
   directly into `nonprofit-board-recruitment`'s recruitment matrix.

## ED-Board Relationship and ED Evaluation

- **Fiduciary duties** (care, loyalty, obedience) apply regardless of governance model; the duty of
  loyalty is operationalized via the conflict-of-interest policy drafted under `nonprofit-bylaws-policy`.
- **ED evaluation**: run annually, tied to written goals set jointly at the start of the review
  period (not invented retroactively), gathering input via a structured tool (self-assessment +
  board chair/committee input, optionally 360-degree staff/peer input) and delivered in executive
  session by the board chair (or a designated committee), never as a surprise.
- **Compensation setting**: for the ED's pay, apply the IRS **rebuttable presumption of
  reasonableness** process — independent body approval (no one with a conflict of interest voting),
  use of comparability data (peer nonprofit compensation surveys), and contemporaneous documentation
  of the decision and rationale — this protects both the ED and board from an excess-benefit-
  transaction finding.

## Standard Deliverables

- Board meeting agenda template with consent agenda and timeboxes
- Committee charter template (purpose, authority, membership, reporting cadence)
- Board self-assessment survey and action-plan summary
- ED annual evaluation tool and goal-setting worksheet
- Board member job description / code of conduct one-pager

## For advisors

- As the ED or board chair, redesign the agenda and packet cadence first — most "board dysfunction"
  complaints are solved by better meeting mechanics before any personnel or bylaws change is needed.
- Frame committee-charter gaps and self-assessment results as a specific action plan with owners and
  dates for the Governance Committee — not just a diagnostic memo.

## Verify Before Acting

- [ ] Governance model (Carver, traditional or hybrid) is named and the agenda and delegation language match it.
- [ ] Quorum, supermajority votes and committee authority match the organization's actual bylaws, not a template.
- [ ] Each committee charter states whether it recommends or acts, and any power to act is permitted by the bylaws.
- [ ] Executive-session and ED-evaluation steps keep the evaluation in executive session, against goals set at the start of the period.
- [ ] ED compensation steps follow the rebuttable-presumption process (independent approval, comparability data, contemporaneous documentation).
- [ ] CEO-side work (board report, self-eval) is handed to `nonprofit-ceo-board-partnership`.

## Common Failure Modes

- **ED reporting informally to individual directors** instead of the board as a whole, creating rogue
  direction-setting — fix by channeling all ED direction through the board chair and full board votes,
  never a single director acting unilaterally.
- **Executive Committee as a shadow board** that pre-decides everything before the full board sees it.
- **Combined Finance + Audit Committee** on a small board without flagging the independence tension.
- **Self-assessment with no action item**, which wastes the cycle and shows up as a red flag in funder
  due diligence questionnaires.
- **Unwritten committee charters**, so committees drift into duplicating or contradicting each other.
