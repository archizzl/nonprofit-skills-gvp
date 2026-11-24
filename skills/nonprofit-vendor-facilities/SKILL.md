---
name: nonprofit-vendor-facilities
description: "Covers two linked operations jobs: procurement and vendor contracts (tiered purchasing policy, 2 CFR 200 procurement for federal grant funds, competitive bids, contract clause review) and facilities (lease negotiation and renewal, total occupancy cost, shared space, build-out and maintenance planning). Use when asked to 'review this vendor contract before we sign,' 'write a procurement policy for our federal grants,' 'negotiate our office lease renewal,' or 'plan a build-out budget.' Not for event venue logistics (use nonprofit-fundraising-events), approval thresholds and signing authority (use nonprofit-financial-controls), or sponsorship deals (use nonprofit-corporate-sponsorships)."
license: MIT
metadata:
  supervision: "expert-required"
  supervision_note: "Leases and contracts legally bind the organization; federal procurement rules apply to grant funds."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Vendor & Facilities Management

## Boundaries

- Venue booking and logistics for a specific fundraising event: `nonprofit-fundraising-events`.
- Approval-threshold and signing-authority mechanics for vendor payments: `nonprofit-financial-controls`.
- Corporate sponsorship deal structuring: `nonprofit-corporate-sponsorships`.

## Procurement Policy Design

1. **Set a tiered purchasing policy** by dollar amount — e.g., under $1,000: any authorized staff
   with manager approval; $1,000-$10,000: 2-3 informal quotes required; over $10,000: formal
   competitive bid/RFP process; over a board-set capital threshold: board approval required. Tie
   these thresholds to the approval mechanics designed in `nonprofit-financial-controls` rather than
   duplicating a separate, conflicting threshold table.
2. **If the organization receives federal funds** (directly or as a pass-through subrecipient), the
   procurement policy must satisfy **2 CFR 200.317-327 (Uniform Guidance procurement standards)** for
   any purchases charged to those awards: full and open competition, documented cost/price analysis,
   a written conflict-of-interest policy covering procurement staff, and specific micro-purchase and
   simplified acquisition thresholds (dollar figures are set/updated by OMB — verify the current
   thresholds rather than assuming a fixed number). Purchases funded by federal awards without a
   compliant procurement process are a common Single Audit finding (see
   `nonprofit-financial-controls` for the audit-response side).
3. **Require a written conflict-of-interest disclosure** from any staff/board member involved in
   vendor selection before the process starts, not after a vendor is chosen — recuse anyone with a
   financial or family relationship to a bidder.
4. **Document the selection decision** even for below-threshold purchases where feasible — a short
   memo naming who was considered and why the choice was made protects the organization in a funder
   review or audit far better than an undocumented "we've always used them."

## Vendor Contract Negotiation

- **Read for these clauses every time**: term length and auto-renewal (many vendor contracts
  auto-renew with a narrow cancellation window — calendar the cancellation deadline, don't rely on
  memory), termination for convenience vs. termination for cause only, indemnification (make sure the
  nonprofit isn't accepting liability disproportionate to the contract's size), insurance/certificate
  of insurance requirements, data ownership and data deletion on termination (critical for CRM,
  payment processor, and cloud software vendors — see `nonprofit-data-privacy` for the data-handling
  policy side), and price escalation terms (capped annual increase vs. open-ended).
- **Ask explicitly for nonprofit pricing, extended payment terms, or reduced licensing**; it's rarely
  offered proactively.
- **Right-size the contract to actual usage** — long multi-year commitments to lock in a price can
  become a liability if the organization's size, program mix, or software needs change; weigh
  discount-for-commitment against flexibility, especially for a growing or recently-downsized
  organization.
- **Maintain a vendor contract calendar** — renewal dates, auto-renewal cancellation windows, and
  insurance certificate expirations in one tracked place; a lapsed insurance certificate or a
  missed cancellation window are the most common avoidable vendor-management failures.

## Facilities and Lease Management

1. **Before signing or renewing a lease**, model total occupancy cost (base rent, common area
   maintenance/CAM charges, utilities, insurance, property tax pass-throughs if triple-net) against
   the budget's occupancy line (`nonprofit-budgeting`) — a lease quoted as "$X/sq ft" without CAM and
   pass-throughs understates true cost.
2. **Negotiate nonprofit-favorable lease terms where possible**: below-market or donated space from a
   mission-aligned landlord (common for faith-based or community-foundation-affiliated space),
   renewal options with a capped escalation, tenant improvement (TI) allowances for build-out, and
   early termination rights tied to funding contingencies (valuable for a growing or funding-uncertain
   organization).
3. **Evaluate shared space / co-location arrangements** as an alternative to a standalone lease —
   nonprofit "shared services" or co-location hubs (multiple nonprofits sharing one facility, often
   with shared reception, conference rooms, and sometimes shared back-office services) can cut
   occupancy cost meaningfully; weigh against loss of dedicated program space control and brand
   visibility.
4. **Plan build-out and capital repair separately from operating budget** — a build-out or major
   capital repair (new roof, ADA-compliance renovation, program space fit-out) is a capital
   expenditure, not an operating expense; fund it from a capital campaign, a designated capital
   reserve, or a specific grant, and keep it out of the annual operating budget's expense
   line so a one-time cost doesn't distort the ongoing operating picture (coordinate with
   `nonprofit-capital-campaigns` if the amount requires a dedicated fundraising effort, and with
   `nonprofit-reserves-cash-flow` if funded from reserves).
5. **Check ADA and local code compliance** before any program space is opened to the public/clients,
   including physical accessibility and, for many program types, occupancy/fire-code limits — this is
   both a legal requirement and, functionally, a risk-management issue (coordinate with
   `nonprofit-risk-management` for the insurance/liability side).
6. **Maintain a facilities condition and maintenance schedule** (HVAC service intervals, roof
   inspection cycle, fire-safety inspection dates) — deferred maintenance is a frequent hidden cost
   that resurfaces as an emergency capital expense when ignored.

## Total Occupancy Cost Template

| Cost line (annual)               | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 | Source / lease clause |
|----------------------------------|--------|--------|--------|--------|--------|-----------------------|
| Base rent (sq ft x rate)         |        |        |        |        |        |                       |
| Escalation (% or fixed per year) |        |        |        |        |        |                       |
| CAM charges                      |        |        |        |        |        |                       |
| Property tax pass-through        |        |        |        |        |        |                       |
| Building insurance pass-through  |        |        |        |        |        |                       |
| Utilities (if not included)      |        |        |        |        |        |                       |
| Tenant's own insurance           |        |        |        |        |        |                       |
| Build-out cost net of TI allowance |      |        |        |        |        |                       |
| Total occupancy cost             |        |        |        |        |        |                       |
| Budget occupancy line            |        |        |        |        |        |                       |
| Variance                         |        |        |        |        |        |                       |

## Verify Before Acting

- [ ] For federally funded purchases, the procurement policy covers each 2 CFR 200.317-327 element:
      full and open competition, documented cost/price analysis, written conflict-of-interest rules for
      procurement staff, micro-purchase and simplified acquisition thresholds (verify the current
      figures in 2 CFR 200 / OMB guidance), and retained selection documentation.
- [ ] Purchasing tiers match the approval thresholds in `nonprofit-financial-controls`; no second,
      conflicting table.
- [ ] Every contract reviewed has its auto-renewal cancellation deadline and insurance certificate
      expiration entered on the vendor contract calendar.
- [ ] The occupancy model includes CAM and pass-throughs and is compared to the budget occupancy line.
- [ ] Leases, binding vendor contracts, and the federal procurement policy go to qualified counsel
      before signing or adoption.

## Common Failure Modes

- Federal-grant-funded purchases made without following 2 CFR 200 procurement standards, surfacing as
  a Single Audit finding months or years later.
- Missing a lease or vendor contract auto-renewal cancellation window and getting locked into another
  term unintentionally.
- Signing a lease based on quoted base rent without modeling CAM/pass-through charges, causing a
  budget variance every year the lease is in effect.
- No written conflict-of-interest check before vendor selection, especially for a board member's or
  staff member's own company/relative's business.
- Funding a capital build-out or major repair out of the operating budget, distorting that year's
  program-vs-admin ratios and possibly triggering a reserve or cash-flow crisis.

## Standard Deliverables

- Written procurement policy with dollar-tiered approval/bid requirements
- 2 CFR 200-compliant procurement procedure (for federally funded organizations)
- Vendor contract calendar (renewal/cancellation/insurance dates)
- Lease total-occupancy-cost model
- Facilities maintenance and capital repair schedule

## For advisors

- When a client receives or is pursuing federal funding, check the procurement policy against 2 CFR
  200 standards proactively rather than waiting for a Single Audit finding to surface the gap.
