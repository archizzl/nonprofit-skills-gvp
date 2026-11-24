---
name: nonprofit-bylaws-policy
description: "Drafts and reviews nonprofit bylaws (membership, board size and terms, quorum, voting, amendment) and core governance policies: conflict-of-interest, whistleblower/non-retaliation, and document retention and destruction. Use when asked 'draft bylaws for a new 501(c)(3),' 'our bylaws say 15 seats but we have 7,' 'write a conflict-of-interest policy and disclosure form,' or 'create a document retention schedule.' Not for running meetings or committees under existing bylaws (use nonprofit-board-governance), Form 990 filing (use nonprofit-form-990), or state charitable solicitation registration (use nonprofit-charitable-registration)."
license: MIT
metadata:
  supervision: "expert-required"
  supervision_note: "Bylaws are legally binding on the organization and controlled by state law."
  last_reviewed: "2026-11-09"
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Bylaws & Core Policy Drafting

## Boundaries

This skill produces the documents, including the policies IRS Form 990 asks whether an organization has adopted.

- Operating within them day-to-day (meetings, committees, the ED relationship): `nonprofit-board-governance`.
- Annual filing mechanics and public disclosure of the 990: `nonprofit-form-990`.
- State-by-state charitable solicitation registration filings: `nonprofit-charitable-registration`.

## Bylaws: Required and Recommended Provisions

Bylaws are the organization's internal operating rulebook and generally control over informal
practice — if actual practice conflicts with written bylaws, the bylaws (or state law) govern until
formally amended. Core sections to include:

1. **Name, purpose, and mission reference** — should track the Articles of Incorporation, not
   contradict it; contradictions between Articles and bylaws are a common cause of IRS/state
   follow-up.
2. **Membership structure** (if any) — nonprofits are not required to have a legal "membership" class
   with voting rights distinct from the board; decide deliberately, since a formal membership
   structure adds real governance obligations (member meetings, member voting rights on certain
   actions) that most service-delivery nonprofits should not take on without a specific reason
   (e.g., associations, some advocacy coalitions).
3. **Board composition** — size (a fixed number or a range, e.g., "no fewer than 5 nor more than 15"
   avoids repeated bylaws amendments as the board changes size), qualifications, and any required
   seats (e.g., board chair of a fiscal sponsor, specific stakeholder seats).
4. **Terms and term limits** — length of term (commonly 2-3 years), maximum consecutive terms
   (commonly 2-3 terms before a mandatory one-year gap), and staggered terms so the whole board
   doesn't turn over in the same year.
5. **Officer roles** — Chair/President, Vice Chair, Secretary, Treasurer at minimum, with duties
   defined (the Treasurer works with staff on statements per `nonprofit-financial-statements`).
6. **Meetings** — frequency of required board meetings (many states set a statutory minimum, often
   annual at minimum), notice requirements, quorum (commonly a majority of seated directors, not
   "authorized" seats if there are vacancies — specify which), and whether virtual/electronic
   meetings and written consent-in-lieu-of-meeting are permitted.
7. **Voting** — simple majority default; name which actions require a supermajority (commonly bylaws
   amendments, removal of a director, dissolution, mergers) — check
   `nonprofit-mergers-fiscal-sponsorship` for merger process itself.
8. **Committees** — authorize the board to create committees and distinguish board committees
   (composed of directors, can hold delegated authority) from advisory councils (non-directors, no
   binding authority) if the organization uses both.
9. **Indemnification** — protects directors/officers acting in good faith from personal liability,
   generally paired with D&O insurance (see `nonprofit-risk-management`).
10. **Amendment procedure** — who can propose amendments, notice period, and vote threshold required.
11. **Dissolution clause** — required for 501(c)(3) status: on dissolution, remaining assets must go
    to another 501(c)(3)/governmental entity, never to private individuals. The IRS looks for this
    dedication of assets in the organizing document (Articles of Incorporation for a corporation) or
    in state law, so confirm the Articles carry it; restating it in the bylaws is fine but does not
    substitute for a missing Articles clause.

### Common Bylaws Failure Modes

- Bylaws say one board size, actual practice is another (unamended after growth/shrinkage) —
  reconcile before any funder or auditor governance review.
- No stated quorum, or a quorum defined against "board seats" without clarifying vacant seats count
  against or are excluded from the total — ambiguity that stalls a vote's validity when challenged.
- No conflict-of-interest or indemnification clause cross-referenced, leaving the two documents
  inconsistent.
- Amendment procedure so burdensome (e.g., requires unanimous consent) that the bylaws become
  functionally unamendable and organizations start operating in violation of their own document.

## Conflict-of-Interest (COI) Policy

The IRS Form 1023 application and Form 990 (Part VI, Line 12) both ask whether the organization has
a written COI policy — adopt one even though it is not strictly statutorily mandated everywhere,
since its absence is treated as a governance red flag by funders, charity raters, and the IRS
itself.

1. **Definition section**: define "interested person" (directors, officers, key employees, and their
   family members/business entities) and "financial interest" broadly enough to catch indirect
   benefit (e.g., a vendor contract with a director's company).
2. **Disclosure duty**: require annual written disclosure from every director/officer/key employee,
   plus an ad hoc disclosure obligation the moment a new conflict arises (not just annually).
3. **Recusal procedure**: the interested person discloses, leaves the room for discussion and vote,
   and is not counted toward quorum for that vote — minute the recusal explicitly.
4. **Determination of fair/reasonable transaction**: the disinterested board members must
   affirmatively determine the transaction is fair and in the organization's best interest, using
   comparability data where relevant (ties directly to the IRS **rebuttable presumption of
   reasonableness** process for compensation — see `nonprofit-board-governance`'s ED evaluation
   section for that specific application).
5. **Annual disclosure form** — a standard one-page form every board/staff member covered signs
   yearly listing known financial interests, board/employment affiliations, and family relationships
   with vendors or grantees. Skeleton:

```
[Organization] Annual Conflict-of-Interest Disclosure — [year]
Name / role (director, officer, key employee): ______
I have received and read the COI policy adopted [date].   [ ] Yes
1. Financial interests in any vendor, grantee or partner of [Org]: [none | list entity, nature of interest]
2. Board, officer or employment roles with other organizations: [list]
3. Family members employed by, or doing business with, [Org]: [none | list]
4. Transactions with [Org] in the past 12 months in which I or a family member had an interest: [none | list]
I will disclose any new conflict promptly, before the related discussion or vote.
Signature / date: ______    Reviewed by (secretary or governance chair): ______
```

## Whistleblower / Non-Retaliation Policy

Not universally state-mandated for nonprofits, but required in some states (e.g., New York for
nonprofits with 20 or more employees and more than $1 million in prior-year annual revenue; verify the
current threshold in the state's nonprofit corporation law or attorney general guidance) and treated as a
Form 990 governance-disclosure question elsewhere — adopt regardless of jurisdiction as standard practice.

1. State the organization's commitment to legal/ethical conduct and prohibits retaliation against
   anyone reporting suspected fraud, financial impropriety, or legal/policy violations in good
   faith.
2. Provide at least one reporting channel *outside* the normal chain of command (e.g., board audit
   committee chair or an anonymous hotline/email) so a report about the ED or CFO has somewhere safe
   to go.
3. Name who investigates (audit committee is common) and commit to a defined timeline for
   acknowledgment and resolution.
4. Explicitly state that knowingly false reports are not protected, to prevent misuse, while making
   clear good-faith reports made without full certainty are protected.

## Document Retention and Destruction Policy

Required-in-substance because the federal Sarbanes-Oxley Act's document-destruction provision
(18 U.S.C. § 1519) applies to nonprofits too — knowingly destroying documents relevant to a federal
investigation is a criminal offense regardless of entity type; a written policy demonstrates
good-faith routine practice rather than post-hoc destruction.

1. Build a retention schedule table by document category with a specific retention period, e.g.:
   corporate records/bylaws/minutes/Articles (permanent); IRS exemption determination letter
   (permanent); financial statements and audits (permanent or 7+ years); tax/990 filings (permanent
   or per state, commonly 7 years minimum); employment/personnel records (7 years post-termination as
   a conservative default; federal minimums are shorter — I-9s for 3 years after hire or 1 year after
   employment ends, whichever is later, and employment tax records for at least 4 years); grant agreements and related records
   (per the grant's own retention clause, often 3-7 years post-award-closeout — check individual
   agreements; federal awards under 2 CFR 200.334 generally require 3 years from submission of the
   final financial report); donor records and gift agreements
   (permanent for named/restricted gifts, per `nonprofit-planned-giving` for legacy commitments);
   insurance policies (permanent while any related claim is possible). Verify the current federal
   minimums at the source (USCIS for I-9s, IRS for employment tax records, 2 CFR 200.334 on eCFR) and
   check state law, which may be longer.
2. Include an explicit **litigation/investigation hold** clause: normal destruction schedules are
   immediately suspended for any document relevant to pending or reasonably anticipated litigation,
   audit, or investigation — this clause is what makes the routine-destruction defense credible.
3. Name a records custodian/owner and specify both physical and electronic records (including email
   and cloud storage), plus secure destruction methods (shredding, secure wipe) rather than simple
   deletion.

## Standard Deliverables

- Full bylaws draft or redline of existing bylaws against current practice
- Conflict-of-interest policy + annual disclosure form
- Whistleblower/non-retaliation policy with named reporting channel
- Document retention and destruction schedule (table by document category)

## For advisors

- Run a practice-vs-bylaws reconciliation pass first (actual board size, actual quorum practice, actual
  committee structure) before drafting amendments; the most common project is fixing drift, not writing
  from scratch.
- Get every COI disclosure form signed annually with a hard deadline, not "as time allows."
- Treat missing COI, whistleblower and document retention policies as the fastest, lowest-cost governance
  wins: they weigh heavily in funder due diligence and 990 Part VI relative to the effort, and should
  usually come before a full bylaws rewrite unless a specific defect (quorum ambiguity, term limit drift)
  is blocking a live decision.

## Verify Before Acting

- [ ] Purpose and dissolution language matches the Articles of Incorporation; the Articles carry the
      501(c)(3) dedication-of-assets clause.
- [ ] Board size, terms, quorum, notice and supermajority thresholds are checked against the current state
      nonprofit corporation statute and against actual practice.
- [ ] Bylaws, COI policy and indemnification clause cross-reference each other consistently.
- [ ] Whistleblower thresholds and retention periods are confirmed at the current official source for the
      organization's state and funders.
- [ ] The amendment procedure in the existing bylaws is followed for adoption (notice, vote threshold),
      and the vote is minuted.
- [ ] The draft is marked for review by the organization's legal counsel before adoption; bylaws are
      legally binding and controlled by state law.
