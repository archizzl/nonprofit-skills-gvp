---
name: nonprofit-annual-appeals
description: "Plans and writes annual fund direct-mail and email appeals: donor segmentation for a drop, ask-string ladders, appeal letter and reply-device copy, year-end and giving-season calendars, and response-rate and average-gift analysis. Use when a user says 'plan our year-end appeal', 'write the appeal letter and reply card', 'build an ask string for this segment' or 'why did this appeal underperform?'. Not for CRM or segmentation tooling setup (use nonprofit-donor-crm), lapsed-donor win-back campaigns (use nonprofit-donor-retention), team or walk campaigns (use nonprofit-peer-to-peer-fundraising), or non-ask newsletters (use nonprofit-email-newsletter)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Solicitation copy goes to your whole donor file at once."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Annual Fund Appeals

## Boundaries

- CRM and segmentation tooling setup: `nonprofit-donor-crm`. This skill uses those segments to drive
  messaging and ask amounts.
- Lapsed-donor win-back campaign design: `nonprofit-donor-retention`. This skill covers what to send
  an active or recently lapsed segment as part of the regular appeal calendar.
- Team, walk and run campaigns: `nonprofit-peer-to-peer-fundraising`.
- Non-ask newsletter content: `nonprofit-email-newsletter`.
- Online donation page conversion copy: `nonprofit-donation-page-copy` (keep its ask amounts and
  framing consistent with the appeal).

## Core Rules

- **Ask string** — anchor suggested amounts to the donor's own giving history, not a generic
  ladder: center the ask string around 1.1x-1.5x the donor's last or highest gift, with the top
  option meaningfully higher to invite an upgrade.
- **Segments** — new donors (first-year), renewing donors, lapsing donors, mid-level donors, and
  non-donor prospects or lapsed inquirers each get a distinct messaging angle and ask level.
- **Appeal calendar** — typically: spring/mid-year appeal, summer sustainer push, fall/pre-year-end
  appeal, December year-end appeal (often 30-40%+ of annual-fund dollars for many orgs), and a
  January thank-you/tax-receipt touch. Avoid stacking two full-file asks within 2-3 weeks of each
  other.

## Standard Deliverables

1. **Segmentation plan** — segments with distinct messaging angle and ask-string logic per segment.
2. **Appeal letter** — direct-response structure: a compelling opening (specific person/moment, not
   a mission-statement restate), the problem, the specific ask amount(s), what the gift accomplishes
   in concrete terms ("$75 provides X"), a deadline or urgency device, a single call to action, and
   a P.S. (direct-mail P.S. lines are read almost as often as the opening and should restate the
   ask/urgency).
3. **Reply device / donation page** — matches the letter's ask string exactly across mail, email,
   and the landing page.
4. **Appeal calendar** — dated plan across the fiscal year with channel, segment, and theme per drop.
5. **Performance scorecard** — per appeal: response rate (gifts / pieces sent), average gift,
   cost-to-raise-a-dollar, and year-over-year comparison by segment.

### Output template: segment plan and letter skeleton

| Segment | Definition | Count | Messaging angle | Ask string | Channel | Drop date |
|---|---|---|---|---|---|---|
| New | First gift in last 12 months | [n] | [angle] | [1.1x-1.5x last gift ladder] | [mail/email] | [date] |
| Renewing | [definition] | [n] | [angle] | [ladder] | [channel] | [date] |
| Lapsing | 1-2 years since last gift | [n] | [angle] | [ladder] | [channel] | [date] |
| Mid-level | [org threshold] | [n] | [angle] | [ladder] | [channel] | [date] |

```
Opening: [specific person or moment]
Problem: [what is at stake, in one short paragraph]
Ask: [ask amount from this segment's string] by [deadline]
Impact: [$X provides Y — finance-verified]
Urgency: [deadline / match / challenge, if real]
Call to action: [one action: reply card, URL, phone]
Signature: [name, title]
P.S. [restate ask amount and deadline]
```

## Concrete Steps

1. Pull and segment the donor file: new, renewing, lapsing (1-2 years since last gift; test
   messaging here vs. handing fully lapsed 2+ year donors to a dedicated win-back track), mid-level,
   and prospects.
2. Set ask strings per segment anchored to giving history (1.1x-1.5x last/highest gift, escalating
   top anchor) rather than one flat ask string for the whole file.
3. Draft the letter using direct-response structure; lead with a specific story or moment, state
   the ask early and again in the P.S., and quantify gift impact in concrete terms.
4. Build the reply device/donation page to mirror the letter's exact ask amounts and any matching
   gift or challenge grant mentioned.
5. Slot the appeal into the calendar with adequate spacing from other mass appeals and from
   any peer-to-peer or event solicitation touching the same file.
6. Send a testable variant where feasible (subject line, ask amount, or opening story) if volume
   supports statistically meaningful comparison.
7. After the appeal closes, calculate response rate and average gift by segment; compare to prior
   year and to sector benchmarks (annual fund response rates commonly run low-single-digit
   percentages for cold mail and higher for warm/renewal segments — treat any specific external
   benchmark figure as a rough reference, not a guarantee, and prioritize the org's own
   year-over-year trend).
8. Feed underperforming segments back into the segmentation plan for the next cycle rather than
   repeating the same ask unchanged.

## Verify Before Acting

- [ ] Ask amounts are identical across the letter, reply device, email and landing page for each segment.
- [ ] Every segment maps to exactly one ask string, and the string is based on that donor's giving history.
- [ ] Deadline, match or challenge language is real, consistent across channels, and approved by whoever holds the match.
- [ ] Impact statements ("$75 provides X") are confirmed with finance or program staff.
- [ ] Merge fields, salutations and suppressions (recent donors, do-not-solicit, deceased) are tested on a seed list.
- [ ] No other full-file ask lands within 2-3 weeks of this drop.
- [ ] Copy has been reviewed by a second person before it goes to the whole file.

## Common Failure Modes

- **One ask string for everyone**: ignoring giving history produces both under-asks (frustrating
  loyal donors) and over-asks (alienating new/small donors).
- **Mission-statement opening**: burying the ask and the human story under organizational
  boilerplate in the first paragraph, where response-rate impact is highest.
- **Mismatched channels**: letter and online donation page showing different suggested amounts or
  different campaign framing, confusing the donor and depressing conversion.
- **Appeal stacking**: sending a full-file mail appeal and a full-file email appeal with the same
  ask within days of each other, spiking unsubscribes/opt-outs.
- **No P.S. or weak P.S.**: skipping the highest-read line of a direct-mail letter.
- **Ignoring cost-to-raise-a-dollar**: chasing response rate alone without factoring mail/print
  costs against a lower-cost email-only push for marginal segments.
- **Rewriting creative to fix a data problem**: a declining-response problem is often a
  segmentation or list-hygiene issue (routed partly to `nonprofit-donor-crm`), not a copywriting
  one. Request the last 2-3 years of appeal-level response rate and average gift by donor type
  before recommending new creative.

## For advisors

- Push clients toward a documented appeal calendar with explicit spacing rules; ad hoc scheduling
  driven by whoever has bandwidth that month is the most common root cause of donor fatigue and
  inconsistent year-over-year comparisons.
- Frame the December appeal's outsized share of annual results to the board explicitly so cash-flow
  and staffing decisions account for that concentration.
