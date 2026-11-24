---
name: nonprofit-digital-fundraising-tools
description: "Evaluates and sets up the tools that process online gifts: giving platforms, peer-to-peer and crowdfunding platforms, payment processors and gateways, recurring-gift billing with card updater and dunning, donation form technical setup, and fee and total-cost modeling. Use for 'which online giving platform should we use,' 'compare payment processor fees,' 'set up monthly giving with failed-card retries,' or 'should we cover fees or pass them to donors.' Not for CRM selection or data hygiene (use nonprofit-donor-crm), PCI scope or privacy (use nonprofit-data-privacy), donation page copy (use nonprofit-donation-page-copy), or peer-to-peer campaign strategy (use nonprofit-peer-to-peer-fundraising)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Payment and gateway choices move donor money."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Digital Fundraising Tools

## Boundaries

This skill covers the technology stack that processes and moves online gifts, not the database that
stores donor history or the words on the page. Hand off instead of answering here:

- Which CRM stores the donor record, dedup, and segmentation → `nonprofit-donor-crm` (most giving
  platforms integrate with a CRM; this skill covers the giving/payment tool, the CRM skill covers
  the system of record).
- PCI-DSS scope, data-sharing policy, privacy disclosures → `nonprofit-data-privacy`.
- The persuasive copy, ask amounts, and page layout content itself → `nonprofit-donation-page-copy`.
- Broad peer-to-peer *campaign strategy* (participant recruitment, team captain toolkits) →
  `nonprofit-peer-to-peer-fundraising`; this skill covers the platform/technology selection for
  running it.

## For Practitioners: Selecting and Configuring the Stack

### 1. Separate three decisions that get conflated

1. **Giving platform** (the donation page/checkout experience and campaign tools): Classy,
   Donorbox, GiveButter, Qgiv, Network for Good, Bloomerang Giving Tools, Kindful. Product names and
   ownership change often; verify the current lineup on vendor sites before naming options.
2. **Payment processor/gateway** (who actually moves the money): Stripe, PayPal, Authorize.Net,
   often bundled inside the giving platform's contract but sometimes a separate merchant account.
3. **CRM/system of record** (`nonprofit-donor-crm`): where the gift and constituent history live
   after the transaction completes.

Many platforms bundle #1 and #2; almost none replace #3. Confirm what syncs automatically to the
CRM (real-time API, nightly batch, or manual CSV export) before assuming integration exists.

**Default shortlist heuristic** (instead of a flat vendor list):
- Start with the giving tools native to, or natively integrated with, the org's current CRM; a
  platform without a native sync must justify the reconciliation work it adds.
- Low or irregular online volume: favor no-monthly-fee platforms (percentage or donor-tip models).
- Steady, higher volume: compare flat SaaS fees against percentage fees at the org's actual volume;
  a flat fee wins once annual online volume x the percentage platform fee exceeds the flat fee.
- Large recurring share: weight card updater, dunning, and processor token portability above
  campaign features.
- Peer-to-peer or event-heavy: shortlist platforms with combined registration-plus-donation checkout.

### 2. Compare platforms on fee structure, not just sticker price

Standard deliverable: a **fee and feature comparison table** covering:

- **Platform fee**: flat monthly/annual SaaS fee vs. percentage-of-transaction vs. "free" platform
  monetized through an optional donor-paid tip/cover-fee prompt (Classy, GiveButter, and Donorbox
  all use variants of this "donor covers fees" model).
- **Payment processing fee**: typically 2.2%-2.9% + $0.30/transaction for card payments; ACH/bank
  transfer is usually cheaper (often under 1%) and worth offering for larger gifts. Verify current
  published pricing on each vendor's nonprofit pricing page before quoting any fee.
- **Peer-to-peer/event fees**: often a separate, higher fee tier layered on top of standard giving
  fees.
- **Nonprofit discount rates**: PayPal, Stripe, and several platforms offer reduced nonprofit
  pricing — confirm the org is registered for it (usually requires 501(c)(3) verification).
- **True effective cost**: model total fees against actual gift volume and average gift size, not
  the advertised headline rate — a platform with a higher percentage but donor-covered fees can
  net the org more than a "cheaper" one where the org absorbs all fees.

**Comparison table skeleton** (worked numbers are illustrative only; replace with the org's gift data
and each vendor's current published rates):

| Line | Platform A | Platform B |
|------|------------|------------|
| Annual online volume / gift count | $100,000 / 1,000 | $100,000 / 1,000 |
| Platform fee | $0 (donor tip model) | $1,200/yr flat |
| Card processing (illustrative 2.9% + $0.30) | $3,200 | $3,200 |
| Donor-covered fee opt-in (org's assumption) | 60% | 0% (org absorbs) |
| Fees absorbed by org | $1,280 | $4,400 |
| Net to mission | $98,720 | $95,600 |
| CRM sync (native / middleware / CSV) | | |
| Recurring: card updater, dunning, token export | | |
| Peer-to-peer / event fee tier | | |

### 3. Recurring giving setup

Configure recurring giving deliberately:

1. Set the default recurring cadence prominently (monthly) with one-time as the secondary option,
   not the reverse — form design measurably shifts donors toward whichever option is emphasized.
2. Enable **account updater / card-updater services** (most major processors offer this) so
   expiring or reissued cards update automatically instead of silently failing.
3. Configure **dunning management**: automatic retry logic and donor email notification on failed
   recurring charges, with a grace period before canceling the recurring gift.
4. Track and report a **recurring-gift attrition/churn rate** separate from overall donor
   retention — this is the metric that reveals whether card-updater and dunning setup is actually
   working.

### 4. Peer-to-peer and crowdfunding platform setup

- Common platforms: Classy, GiveButter, Qgiv, RunSignUp (endurance events), Funraise. Evaluate on:
  team/individual page customization, leaderboard and gamification features, participant
  fundraising minimums enforcement, and registration-plus-fundraising combined checkout (for
  walk/run events with a registration fee *and* a fundraising ask).
- Configure the **default page template** participants receive so a majority of fundraising pages
  aren't blank — blank personal pages are the top driver of low participant fundraising totals.
- Confirm how participant-raised funds and any registration fees reconcile back to the CRM as
  separate, correctly-attributed gift records (registration fee vs. donation should not be
  conflated in reporting).

### 5. Technical form setup checklist

1. Mobile-responsive checkout with Apple Pay/Google Pay enabled; wallet payment options reduce
   checkout abandonment.
2. Automatic tax-receipt email on completion, correctly formatted per IRS substantiation rules for
   gifts (statement that no goods/services were provided, or fair market value of any provided).
3. Redirect/thank-you page and confirmation email configured — don't leave donors on a generic
   processor confirmation screen.
4. Source tracking on campaign links so gifts tie back to the specific appeal, and confirm the source
   field carries through to the CRM gift record.
5. Test the full donor path (new card, recurring setup, Apple Pay, failed-card scenario) before
   launch — a broken checkout on a high-traffic day (year-end, Giving Tuesday) is the most common
   and costly technical failure mode.

## For Advisors: Running a Platform Selection or Fee-Optimization Engagement

1. **Volume and gift-profile analysis first**: pull the last 12-24 months of online gift data
   (count, average size, one-time vs. recurring split) before recommending a platform — fee
   structures favor different platforms at different volumes.
2. **Total cost of ownership model**: build a simple spreadsheet projecting annual fees under each
   candidate platform against the client's actual gift volume, including any implementation or
   contract minimums.
3. **Integration audit**: confirm exactly how gifts flow into the client's CRM (native
   integration, Zapier/middleware, manual import) — a beautiful giving platform that requires
   manual monthly CSV reconciliation into the CRM creates ongoing staff burden the client will
   feel long after the selection project ends.
4. **Migration/cutover plan**: if replacing an existing processor, plan for recurring donors'
   payment methods — some platforms support token migration between processors (avoiding
   re-asking every recurring donor for a new card), others require re-enrollment, which causes
   real attrition. Confirm this before recommending a switch.
5. **Deliverable**: a short recommendation memo with the comparison table, TCO projection, and an
   implementation timeline — present fee tradeoffs in terms of net dollars to mission, not just
   percentage rates.

## Common Failure Modes

- Choosing a platform on advertised "0% platform fee" without modeling the donor-covered-fee
  opt-in rate, which is never 100% and shifts real cost back to the org.
- No card-updater/dunning setup, causing silent recurring-gift attrition that looks like a
  retention problem but is actually a technical one.
- Assuming CRM sync is automatic and real-time without verifying it — leads to gift records
  "missing" for days or requiring manual reconciliation.
- Skipping a full checkout test before a high-traffic giving day.
- Not enabling ACH/bank transfer as an option for larger gifts, leaving unnecessary card
  processing fees on the table.
