---
name: nonprofit-charitable-registration
description: "Manages state charitable solicitation registration: which states require registration given the fundraising footprint, initial filings, the Unified Registration Statement (URS), registered agents, exemptions, renewal tracking, and paid-solicitor and fundraising-counsel triggers. Use when asked 'we're doing a national online campaign, which states do we register in,' 'file our charitable registration in New York,' 'build a renewal calendar across our states,' or 'are we exempt because we're small.' Not for the federal Form 990 (use nonprofit-form-990) or corporate foreign qualification to do business in a state."
license: MIT
metadata:
  supervision: "expert-required"
  supervision_note: "State filings with statutory deadlines and fees; requirements vary by state."
  last_reviewed: "2026-11-09"
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Charitable Solicitation Registration

## Boundaries

- Federal Form 990: `nonprofit-form-990` (most states require attaching a copy to the state registration).
- Foreign qualification to transact business in a state is a corporate-law filing, often bundled with
  registration; this skill flags it but does not execute it.

## Core Concept: Solicitation-Based, Not Incorporation-Based Trigger

The single most important thing to get right: registration obligations are triggered by **soliciting
donations from residents of a state**, not by where the organization is incorporated or
headquartered. A nonprofit incorporated in one state that runs a nationwide email appeal, a donation
button visible to all US visitors, or an out-of-state peer-to-peer fundraising event has potentially
triggered registration obligations in every state that received a solicitation — this is the most
commonly missed compliance gap for growing organizations that started local and scaled online
without revisiting registration.

1. **~40 states plus DC** require charitable solicitation registration in some form before a
   nonprofit may solicit contributions from their residents — the exact list and each state's
   specific exemptions changes periodically, so confirm current requirements against a current
   source (e.g., the National Association of State Charity Officials' state survey map at
   https://www.nasconet.org/survey-map, each state regulator's own site, or a compliance service)
   rather than relying on a static memorized list.
2. **Charleston Principles**: advisory guidelines on internet solicitation approved by the NASCO
   Board in 2001 — not binding law, and states apply them differently. For an organization based
   outside the state, registration is generally triggered if its non-internet activity there (direct
   mail, phone, in-person events) would require it on its own; or if it solicits through an
   interactive website (one that can take a donation online, such as a donate button — even via a
   linked or third-party processor) and either specifically targets that state's residents or
   receives "repeated and ongoing" or "substantial" contributions from the state through the site.
   Email solicitation into a state is treated like direct mail or phone solicitation. A website that
   offers information but does not solicit is not by itself a trigger, even if unsolicited donations
   arrive — but organizations that actively fundraise nationally (email campaigns, national
   peer-to-peer events, national grant/major donor prospecting) should assume broad multi-state
   exposure rather than lean on the passive-website exception.
3. **Common exemptions** (vary by state — verify per state, do not assume uniformity): religious
   organizations, all-volunteer organizations with no paid staff, organizations below a small annual
   contribution threshold (commonly in the low five figures, some states set a low-revenue exemption
   with its own registration-lite filing), and educational institutions in some states. Exemption
   does not mean "no filing at all" in every state — several states require an annual exemption
   claim/renewal even for exempt organizations.

## Registration Process

1. **Build the solicitation footprint map first**: list every state where the organization actively
   solicits — direct mail lists, email campaign recipient geography, event locations, peer-to-peer
   participant/donor geography (`nonprofit-peer-to-peer-fundraising`), grant funders headquartered
   in-state, and donation-page traffic by state if available. This map, not a guess, should drive the
   registration list.
2. **Check whether the Unified Registration Statement (URS) still helps** — it was designed as a
   single multi-state paper application, but its publisher (the Multi-State Filer Project) now
   describes it as having "limited utility today since most states require online filing," and its
   June 2025 state list names only seven states that accept it (AR, GA, IL, KS, MN, OR, VA). Major
   solicitation states such as California, New York and Florida are not on that list and use their
   own state forms (California and Florida also offer online filing). Even where the URS is accepted, some states still require a
   state-specific supplemental form/fee, so plan on per-state filings and confirm each state's
   current method with its regulator.
3. **File initial registration before the first solicitation** in a new state, not after — most
   states technically require registration prior to solicitation, and enforcement (though
   inconsistently applied) can include fines and, in serious cases, being barred from soliciting.
4. **Registered agent**: some states require a resident/registered agent (or a consent to service of
   process) as part of charitable registration; most do not, so check each state's form rather than
   assuming. National compliance-filing services commonly bundle this. Decide whether to use a
   commercial registered agent service (scales cleanly across many states) versus a named individual
   (creates a single point of failure if that person leaves the organization).
5. **Attach required supporting documents**: IRS determination letter, most recent Form 990 (see
   `nonprofit-form-990` — most states require the same version filed federally, so keep the two
   processes' timelines synchronized), audited financials above certain revenue thresholds in some
   states, and a list of officers/directors.
6. **Track renewal deadlines per state** — renewal cycles are NOT uniformly annual-on-the-same-date;
   many states set renewal relative to the organization's own fiscal year-end, not a fixed calendar
   date, which is the most common cause of missed renewals in multi-state portfolios.

## Professional Fundraiser and Fundraising Counsel Triggers

Separate registration regimes apply to **paid solicitors** (third parties who solicit on the
nonprofit's behalf, e.g., a telemarketing firm) and **fundraising counsel** (consultants who plan/
manage but don't directly solicit) in many states — if the organization engages an outside firm for
telemarketing, a professional grant-writing/campaign firm, or an event production company that also
solicits sponsors, confirm whether that vendor itself must be separately registered in-state, and
whether the contract must be filed with the state (common in several states for paid-solicitor
contracts specifically). This is a common miss when hiring outside fundraising help for a capital
campaign (`nonprofit-capital-campaigns`) or fundraising event (`nonprofit-fundraising-events`).

## Registration Tracker

| State | Trigger (channel) | Status | Form (state / URS + supplement) | Fee (confirmed on regulator site, date) | Renewal basis (calendar / FYE-relative) | Next due | 990 version attached | Owner |
|---|---|---|---|---|---|---|---|---|
| [State] | [email, events, P2P, mail] | [registered / exempt-filed / not yet needed] | [form name] | [$, date checked] | [rule] | [date] | [tax year] | [name] |

## Verify Before Acting

Run this per state before each filing or renewal:

- [ ] Registration requirement, exemption and threshold confirmed on the state regulator's current site
      (or the NASCO survey map), not a memorized list.
- [ ] Current form, filing method (online or paper) and fee confirmed on the regulator's site; any
      state-specific supplement to the URS is attached.
- [ ] The Form 990 attached is the same version filed federally; audited financials attached where the
      state's revenue threshold requires them.
- [ ] Renewal date is set from that state's rule (calendar date or fiscal-year-relative), not a single
      annual reminder.
- [ ] Any paid solicitor or fundraising counsel is registered in-state and any required contract filing
      is done before the vendor starts work.
- [ ] Filings are reviewed by the compliance owner or counsel before submission; deadlines and fees are
      statutory and vary by state.

## Common Failure Modes

- Registering only in the home state and assuming a nationwide email list or online giving page
  doesn't count as multi-state solicitation.
- Missing a renewal because the state's cycle is tied to fiscal year-end rather than a calendar
  date, and the tracking calendar was built assuming uniform annual dates.
- Filing the URS but skipping a state-specific supplemental form/fee that state still requires on top
  of it.
- Assuming an all-volunteer or small-revenue exemption applies without confirming it against the
  specific state's current threshold and filing requirement (an exemption claim itself is sometimes
  still a required annual filing).
- Not registering the paid-solicitor contract when a state requires the contract itself (not just the
  organization) to be filed before a telemarketing or event-solicitation vendor begins work.

## Standard Deliverables

- Solicitation footprint map (states with active solicitation activity, by channel)
- State-by-state registration tracker (see the table above)
- Registered agent decision memo
- Paid-solicitor/fundraising-counsel vendor compliance checklist

## For advisors

- Build the footprint map before touching any application form; most registration gaps come from
  underestimating footprint, not from filing errors.
- Treat multi-state registration as a standing compliance program with an owner and a tracked calendar;
  recommend a commercial multi-state filing service once an organization solicits in roughly 10+ states.
