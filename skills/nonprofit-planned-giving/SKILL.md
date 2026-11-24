---
name: nonprofit-planned-giving
description: "Builds bequest and legacy society programs: planned-gift vehicles (bequests, beneficiary designations, charitable gift annuities, charitable remainder trusts), legacy conversation scripts, sample bequest language, legacy society marketing, and stewardship of documented estate commitments. Use when a user says 'help us launch a legacy society', 'script a bequest conversation', 'explain a charitable remainder trust to our board' or 'how do we steward donors who put us in their will?'. Not for outright major gifts made today (use nonprofit-major-gifts) or pipeline stage tracking (use nonprofit-donor-pipeline)."
license: MIT
metadata:
  supervision: "expert-required"
  supervision_note: "Gift annuities, remainder trusts and bequests are legal instruments with state registration rules."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Planned & Legacy Giving

## Boundaries

- Outright current major gifts, including large QCD gifts: `nonprofit-major-gifts`.
- Pipeline stage mechanics: `nonprofit-donor-pipeline`. Planned-giving prospects still move through
  those stages before a legacy conversation.

## Planned-Gift Vehicles: Org-Side Rules

Always direct donors to their own attorney/financial advisor for execution; the org's role is to
describe options and provide sample bequest language, not give individualized legal/tax advice.

1. **Bequest** — via will or living trust: specific amount, specific asset, percentage/residuary
   (often preferred since it doesn't need updating when the estate's total value changes), or
   contingent. Provide exact sample bequest language naming the organization's full legal name,
   EIN, and location.
2. **Beneficiary designation** — retirement account (401(k)/IRA), life insurance, or donor-advised
   fund succession. Retirement-account gifts are tax-efficient because the charity, unlike an
   individual heir, pays no income tax on the distribution — a genuinely useful talking point.
3. **Charitable Gift Annuity (CGA)** — requires state-specific registration/regulatory compliance
   and actuarial rate-setting (commonly referencing American Council on Gift Annuities suggested
   rates; verify the current suggested rates with ACGA and the current registration rules with each
   relevant state insurance regulator). Most small/mid nonprofits need a specialized gift-annuity
   administrator or reinsurance arrangement rather than running this in-house from scratch.
4. **Charitable Remainder Trust (CRT)** — requires the donor's own estate attorney to draft; the
   org's role is cultivation and stewardship, not drafting the trust.
5. **IRA Qualified Charitable Distribution (QCD)** — a current (not deferred) gift, often promoted
   alongside planned giving since it targets the same donor segment (70½+; verify the current QCD
   age and annual limit in IRS guidance before citing them). Note it if a donor conversation
   surfaces it, and route large current gifts to `nonprofit-major-gifts`.

## Legacy Society Design

1. Name the society (often tied to a founder, a meaningful year, or mission imagery) and set a
   simple qualification standard: any documented planned gift of any vehicle/amount typically
   qualifies — do not set a minimum dollar threshold, since most bequest amounts are unknown until
   the estate settles.
2. Define membership benefits: recognition (annual listing, unless the donor requests anonymity),
   an annual legacy-society event or gathering, a dedicated staff point of contact, and regular
   impact updates.
3. Build a simple documentation process: a one-page "notification of intent" form the donor can
   voluntarily complete (not legally binding, just informational) so the org can plan and steward
   even without seeing the will itself.

## Standard Deliverables

- **Legacy-gift marketing materials** — website page, newsletter inserts, and a dedicated brochure
  explaining vehicles in plain language with the org's legal name/EIN/sample bequest language
  included.
- **Donor conversation script/talking points** — for gift officers and board members, covering how
  to raise the topic naturally (often tied to stewardship visits with older, loyal donors) without
  it feeling transactional or morbid.
- **Sample bequest language sheet** — exact legal wording for specific-amount, percentage, and
  residuary bequests, reviewed by the org's legal counsel.
- **Legacy society roster and stewardship plan** — tracks documented intents, vehicle type (if
  known), estimated/unknown value, and a stewardship touch cadence distinct from the annual-fund
  cycle.

### Output template: sample bequest language sheet

Structure only. Final wording must come from the org's legal counsel; do not present this skeleton
as approved language.

```
Our legal name: [FULL LEGAL NAME]   EIN: [00-0000000]   Address: [ADDRESS]

Specific bequest:
  "I give [dollar amount / description of property] to [FULL LEGAL NAME], [EIN], [ADDRESS],
  for its general charitable purposes." [counsel-approved wording]

Percentage bequest:
  "I give [percentage]% of my estate to [FULL LEGAL NAME] ..." [counsel-approved wording]

Residuary bequest:
  "I give [all / percentage] of the residue of my estate to [FULL LEGAL NAME] ..." [counsel-approved wording]

Contingent bequest: [counsel-approved wording for gifts that take effect only if named heirs predecease]

Restricted purpose (optional): [counsel-approved wording, with a clause allowing redirection if the purpose becomes impossible]

Please share your plans with us: [contact name, phone, email] | Notification of intent form: [link]
We recommend reviewing your plans with your own attorney or financial advisor.
```

## Concrete Steps

1. Identify planned-giving prospects from existing pipeline data: long-tenured donors (typically
   10+ years of consistent giving), donors aged 60+, donors with no children or stated estate
   planning interest, and volunteers/board alumni with deep affinity but modest current giving
   capacity — planned giving frequently reaches donors who could never make an equivalent outright
   major gift.
2. Introduce the topic in existing stewardship conversations rather than a cold ask — legacy
   conversations work best embedded in an ongoing relationship.
3. Provide vehicle options and sample language; refer the donor to their own advisor for execution.
4. When a donor confirms intent, document it (with the donor's permission) in the legacy society
   roster; invite them to the legacy society if not already a member.
5. Steward documented legacy donors on a distinct cadence — typically lighter-touch financial asks,
   heavier relationship/recognition touches (invitations, updates, personal notes) since no further
   solicitation is usually needed.
6. Report legacy society growth (new documented intents per year, total membership) to the board
   annually as a distinct metric from current-year fundraising totals, since realized value often
   lags by years or decades.
7. When an estate gift is actually received, route it through finance/gift-acceptance policy review
   (especially for non-cash or restricted bequests) before recognition and acknowledgment.

## Verify Before Acting

Before any legacy marketing material, bequest language sheet or donor script goes out:

- [ ] The org's full legal name, EIN and address match its IRS determination letter and state
  records.
- [ ] Sample bequest language has been reviewed by the org's legal counsel.
- [ ] No material or script gives individualized tax or legal advice, and each refers donors to
  their own advisors.
- [ ] Any QCD age or limit, ACGA rate, or tax statement has been checked against the current
  official source (IRS, ACGA, state insurance regulator).
- [ ] If CGAs are offered, state registration and administration (in-house or outsourced) are
  confirmed for every state where annuitants live.
- [ ] A gift acceptance policy covering vehicle types, minimums and complex assets is in place.

## Common Failure Modes

- **Treating legacy giving as a numbers-only youth-to-death funnel**: legacy conversations require
  relationship trust; a cold mailer alone rarely converts without an existing warm relationship.
- **No sample bequest language provided**: donors abandon the idea when required to draft legal
  language themselves — always hand them exact, attorney-reviewed wording.
- **Setting a dollar minimum for legacy society membership**: discourages participation since most
  donors don't know or won't disclose the amount.
- **Giving individualized tax/legal advice**: exposes the org and the donor to risk — always refer
  to the donor's own professional advisors.
- **Under-resourcing gift-annuity administration**: attempting to run CGAs without proper state
  registration or actuarial/reinsurance support creates real regulatory and financial risk.
- **Marketing before a gift acceptance policy**: accepting an unanticipated complex estate asset
  without a policy (vehicle types accepted, minimums, complex-asset handling) is a recurring
  operational and legal headache; put the policy in place before actively marketing planned gifts.

## For advisors

- Start a launch or revival by segmenting the existing donor file for tenure and age signals; most
  orgs already have a viable legacy prospect pool sitting unused.
- Set board expectations (and KPI design, with `nonprofit-outcomes-measurement`) around
  documented-intent counts and pipeline growth rather than short-term realized-dollar targets.
