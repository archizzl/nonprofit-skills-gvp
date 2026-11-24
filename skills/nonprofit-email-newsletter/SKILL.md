---
name: nonprofit-email-newsletter
description: "Plans a nonprofit's recurring e-newsletter (non-ask supporter updates): cadence, segment content strategy, template sections, content calendar, subject lines, and deliverability. Use when asked to \"design our monthly e-newsletter template,\" \"segment our newsletter list,\" \"improve our newsletter open rates,\" or \"should this go in the newsletter or the appeal email.\" Not for fundraising appeal emails (use nonprofit-annual-appeals), CRM or list tooling setup (use nonprofit-donor-crm), social content (use nonprofit-social-media), or donation page copy (use nonprofit-donation-page-copy)."
license: MIT
metadata:
  supervision: "unsupervised"
  supervision_note: "Recurring supporter updates, no ask and no filing."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Email Newsletter

## Boundaries

- **Newsletter vs. appeal test (apply every time):** if the email's primary CTA is "donate now," it
  belongs to `nonprofit-annual-appeals`, even when sent to the same list. A newsletter may carry only
  a soft, secondary giving mention (e.g., a small "support this work" link).
- Segmentation tooling and CRM/ESP setup: `nonprofit-donor-crm` (this skill defines what each
  segment should see).
- Social content: `nonprofit-social-media`. Donation page copy: `nonprofit-donation-page-copy`.

## Standard Deliverable: Newsletter Template Structure

A reliable recurring structure (readers learn to expect and scan it, improving engagement over time):

1. **Subject line + preview text** — see subject-line guidance below.
2. **Opening note** (2-4 sentences from the ED or a rotating staff voice) — sets the theme for this
   issue, not a generic "hello."
3. **Lead story** — one program update, milestone, or outcome, with a photo and a short pull-quote if
   available (source finished narratives from `nonprofit-storytelling` when featuring a beneficiary).
4. **Quick-hit updates section** — 2-4 short items (upcoming events, a new hire, a media mention, a
   volunteer need) as a scannable bulleted or card list, not full paragraphs.
5. **Spotlight** — rotate between volunteer, donor, staff, or partner spotlights issue to issue so no
   single audience type is neglected.
6. **Upcoming dates/CTA block** — event registrations, volunteer sign-ups; a small "ways to give"
   link, kept secondary in visual weight to informational content.
7. **Footer** — standard boilerplate (from `nonprofit-brand-messaging`), social links, unsubscribe/
   preference-center link (required for CAN-SPAM compliance).

Worked issue outline (illustrative; replace with real program content):

```
Subject:   3 kids, 1 summer, 1 big win
Preview:   What happened when our reading camp doubled in size
Opening:   ED note (3 sentences) — theme: summer learning
Lead:      Camp recap + photo + one consented participant quote
Quick hits: • Fall volunteer orientation 9/12  • New program director  • Local radio mention
Spotlight: Volunteer — a tutor's first season (rotate to donor next issue)
Dates/CTA: Register for the open house (primary)  ·  Ways to give (small text link)
Footer:    Boilerplate · social links · unsubscribe / preferences
```

## Segmentation Strategy (Content Logic, Not Tooling)

Decide *what each segment should see*, then hand the technical list-building to `nonprofit-donor-crm`:

- **General subscribers** (signed up via website, no gift/volunteer history): broadest program-update
  content, low ask frequency, focus on building affinity before conversion.
- **Active donors:** can include slightly more outcome/ROI-of-your-gift framing ("here's what your
  support funded this quarter") without becoming a full appeal.
- **Volunteers:** prioritize volunteer opportunity content and volunteer spotlights; deprioritize
  financial asks, which can feel redundant to their time-based contribution.
- **Board/major stakeholders:** may warrant a distinct, higher-frequency or more detailed version
  (sometimes a separate "board update" is more appropriate than folding them into the general list).
- **Lapsed/inactive subscribers:** consider a distinct re-engagement newsletter track or sunset
  policy rather than lowering overall list deliverability by continuing to mail unengaged addresses.

## Subject Line and Deliverability Practices

- Default: keep subject lines under ~50 characters and specific ("3 kids, 1 summer, 1 big win" beats "Our
  July Newsletter") — specificity consistently outperforms generic labels on open rate.
- Avoid spam-trigger patterns (excessive punctuation/caps, "free," multiple dollar signs).
- Maintain list hygiene: remove or suppress hard bounces and long-term non-openers (e.g., no opens in
  12+ months as a default; adjust against the org's own ESP engagement data) periodically — a bloated, unengaged list drags down sender reputation and can push
  future sends (including appeal emails) into spam folders for everyone.
- Send consistently on the same day/time pattern (e.g., first Thursday monthly) — consistency builds
  subscriber expectation and modestly improves open rates over erratic scheduling.
- Always include a working unsubscribe link and honor opt-outs promptly — a legal requirement (CAN-SPAM)
  and a deliverability factor (spam complaints from ignored unsubscribes damage sender reputation).

## Step-by-Step: Building or Running the Newsletter Program

1. Set cadence based on real content supply, not aspiration — a promised weekly newsletter with only
   monthly program updates worth sharing produces filler content and declining engagement; monthly or
   biweekly is realistic for most small-to-mid nonprofits.
2. Define the segment list and what differs per segment (per the strategy above); confirm the CRM/
   ESP can actually execute the planned segmentation before committing to it editorially.
3. Build the template structure once as a reusable layout; resist redesigning it every issue.
4. Maintain a rolling content calendar 4-8 weeks out, pulling from the same content pipeline as
   social media and the annual report so stories are captured once and reused across channels.
5. Draft using the org's messaging house voice; keep the CTA block visually secondary to information.
6. QA every issue: test links, check personalization tags render correctly, and preview on mobile
   (most nonprofit email opens are on mobile devices).
7. Send, then review open rate, click rate, and unsubscribe rate by segment; watch for a rising
   unsubscribe rate as an early signal of ask-creep or declining relevance.
8. Periodically clean the list (bounce and long-term non-opener suppression) on a set schedule (e.g.,
   twice yearly) rather than only reactively after a deliverability problem appears.

## Common Failure Modes

- **Ask creep:** the "newsletter" slowly becomes another appeal channel, fatiguing the list and
  blurring the metric picture for both channels — if this is happening, split into two distinct
  sends/tracks.
- **One-size-fits-all content** sent identically to donors, volunteers, and cold subscribers, missing
  relevance gains from minimal segmentation effort.
- **Irregular cadence** that trains subscribers not to expect (or open) the email.
- **No content pipeline coordination** with social/annual report teams, causing duplicated effort or,
  worse, stale content because "someone else already covered that story."
- **Ignoring list hygiene**, letting deliverability quietly degrade until even appeal emails
  (a much higher-stakes send) land in spam.
- **Overloading each issue** with too many CTAs (donate, volunteer, register, follow us, read this) —
  newsletters with a single primary CTA per issue outperform multi-ask emails on click-through.

## For advisors

- When a client says "our newsletter isn't working," first check whether it has quietly become an
  appeal channel (a strategy problem) before recommending template or subject-line fixes (tactical
  problems); the two need different recommendations.
