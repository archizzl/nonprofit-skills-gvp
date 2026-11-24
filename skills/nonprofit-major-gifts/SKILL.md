---
name: nonprofit-major-gifts
description: "Sets major and principal gift strategy for one prospect: capacity, affinity and readiness rating, a specific ask amount and structure, proposals and one-page cases, solicitation briefings, and gift agreements including multi-year pledges and naming terms. Use when a user says 'how much should we ask this donor for?', 'help me structure a $500K proposal', 'draft a gift agreement for a named fund' or 'prep me for a solicitation meeting'. Not for moving prospects through pipeline stages (use nonprofit-donor-pipeline), bequests and legacy gifts (use nonprofit-planned-giving), or campaign-wide gift tables (use nonprofit-capital-campaigns)."
license: MIT
metadata:
  supervision: "expert-required"
  supervision_note: "Gift agreements, multi-year pledges and naming rights are enforceable commitments."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Major & Principal Gift Strategy

## Boundaries

- Tracking where a prospect sits in the general pipeline: `nonprofit-donor-pipeline`.
- Bequests and legacy society gifts: `nonprofit-planned-giving`.
- A capital campaign's overall gift table and leadership: `nonprofit-capital-campaigns`, which
  calls this skill for each individual ask.
- Proposals to foundation or institutional funders: `nonprofit-grant-writing`.
- Pledge reminders and stewardship after the gift: `nonprofit-donor-retention`.

Most organizations define "major gift" as a threshold relative to their own median gift (commonly
the top 1-10% of donors or a fixed floor like $10K-$25K+); "principal gift" typically denotes the
top tier within major gifts (often $1M+ or the organization's own defined ceiling tier). Confirm
the org's own threshold before applying generic figures.

## Capacity & Readiness Rating

Score each prospect on three independent axes before setting an ask:

1. **Capacity** — estimated financial ability to give, from wealth indicators (real estate,
   business ownership, stock holdings/SEC filings, past gift sizes to peer organizations, art/
   foundation affiliations). Express as a *range*, not a point estimate (e.g., "$50K-$150K
   capacity over 3-5 years").
2. **Affinity** — strength of connection to the mission and to an inside champion (board
   member, staff, peer donor) who can open or accompany the ask.
3. **Readiness** — timing signals: recent liquidity event, life stage, past response to
   cultivation moves, explicitly stated interest. A high-capacity, high-affinity prospect with low
   readiness should not be solicited yet — return to cultivation.

A common failure mode is setting the ask from capacity alone; always multiply the capacity/affinity/
readiness signals together, not add them — a weak score on any one axis should sharply reduce
confidence in a near-term ask.

## Setting the Ask Amount

1. Anchor to actual data: largest prior gift to your org, largest known gift to any peer
   organization, and stated or inferred capacity range.
2. Apply a stretch multiplier appropriate to relationship depth — typically 1.5x-3x the donor's
   largest previous gift for a well-cultivated relationship; higher stretch requires higher
   confidence in capacity and cultivation depth.
3. Set a specific number, not a range, in the internal strategy — asking "for a gift between $25K
   and $50K" externally is acceptable, but the internal team must agree on a real target and a
   walk-away minimum before the meeting.
4. Decide the ask structure: outright cash, multi-year pledge (typically 3-5 years), or a
   blended cash + appreciated stock/DAF gift. Multi-year pledges let you propose a materially
   larger total commitment at a comfortable annual cash-flow level for the donor.
5. Identify the right asker (peer-to-peer solicitation by a board member or major donor
   consistently outperforms staff-only asks) and confirm they are briefed and rehearsed.

## Standard Deliverables

- **One-page case/proposal summary** — problem, solution, specific funding need tied to a concrete
  budget line or project, requested amount, naming/recognition offered, timeline.
- **Formal proposal document** (for $100K+ or campaign gifts) — narrative case, budget detail,
  organizational credibility section, gift structure options, next steps (individual/family
  donors; institutional funders go to `nonprofit-grant-writing`).
- **Gift agreement** — legally reviewable document specifying: gift amount and payment schedule,
  restriction/designation of funds, naming rights and duration, reporting commitments back to the
  donor, and a variance/redirection clause if the named purpose becomes impossible to fulfill
  (essential — its absence is a recurring legal and PR risk for named endowments and building
  gifts).
- **Solicitation briefing memo** — for the asker: relationship history, ask amount and rationale,
  anticipated objections, and a fallback ask if the primary number is declined.

## Concrete Steps

1. Confirm the prospect has cleared Cultivation and is marked ready in the pipeline system
   (`nonprofit-donor-pipeline` handoff point).
2. Complete the capacity/affinity/readiness rating; do not proceed to ask-setting on capacity
   alone.
3. Set the specific ask number and structure (outright vs. multi-year vs. blended) using the
   anchoring method above.
4. Draft the proposal or one-pager matched to the ask size and the donor's stated interest area.
5. Identify and brief the asker; rehearse the ask, including handling a "no," a "not now," and a
   counter-offer.
6. Conduct the solicitation; record the outcome, amount, and any conditions immediately.
7. On a "yes," draft the gift agreement within 5-10 business days while intent is fresh; route
   through legal/finance review before signature for any gift with naming rights or restrictions.
8. On a multi-year pledge, set up pledge reminder and payment tracking (a stewardship handoff to
   `nonprofit-donor-retention`).

### Output template: solicitation briefing memo

```
Prospect: [name]          Asker(s): [peer asker + staff partner]     Meeting: [date, place]
Ratings: Capacity [range over N years] | Affinity [high/med/low + champion] | Readiness [signal]
Relationship history: [prior gifts with dates and amounts; key cultivation moves]
Donor's interest area: [what they have said they care about]
Ask: [specific amount] for [purpose / budget line], structure [outright / N-year pledge / blended]
Rationale: [largest prior gift, peer gifts, stretch multiple used]
Walk-away minimum: [amount]          Fallback ask: [amount or structure]
Recognition offered: [naming / recognition, subject to gift acceptance policy]
Anticipated objections and responses: [objection -> response]
Next step if yes: [gift agreement within 5-10 business days; legal/finance review]
Next step if "not now": [return-to-cultivation move and date]
```

## Verify Before Acting

Before the ask, and again before any gift agreement is signed:

- [ ] The prospect is marked ready in the pipeline and has a rating on all three axes, not
  capacity alone.
- [ ] The internal team has agreed a specific ask number and a walk-away minimum, and the asker is
  briefed.
- [ ] Gift agreement amount, payment schedule, restriction, naming term and duration, reporting
  commitments and variance clause match the proposal and the donor's verbal yes.
- [ ] The org can deliver any restricted purpose long term, and naming terms fit its gift
  acceptance and naming policies.
- [ ] Legal and finance have reviewed any agreement with naming rights, restrictions or a
  multi-year pledge before signature.

## Common Failure Modes

- **Underasking**: staff self-censor and ask well below true capacity out of discomfort — counter
  with the anchoring formula and peer-comparison data, not intuition.
- **No walk-away number**: going into a solicitation without an agreed minimum acceptable gift
  leads to accepting a token amount that undervalues the relationship.
- **Undefined restrictions**: accepting a highly restricted gift without confirming the org can
  actually deliver the restricted purpose long-term — always negotiate a variance clause.
- **Wrong asker**: sending a junior staffer to ask a peer-level relationship a board member should
  be asking.
- **Proposal-agreement mismatch**: gift agreement terms that drift from what was actually proposed
  and verbally agreed — reconcile documents before signature.
- **Training before diagnosis**: when proposal-to-close is low, diagnose whether the failure is the
  ask amount (asking wrong), the asker (wrong messenger) or readiness (asking too soon) before
  recommending training; each has a different fix.

## For advisors

- Bring an outside, dispassionate capacity read; clients routinely underestimate their top donors'
  capacity because staff proximity breeds caution. Use documented peer-gift comparisons to justify a
  stretch ask to a skittish ED or board.
- Insist on a written gift agreement template with a variance clause as a standard deliverable; its
  absence is a governance red flag worth raising with the board directly.
