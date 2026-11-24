---
name: nonprofit-risk-management
description: "Runs nonprofit risk assessment and mitigation: risk register, insurance coverage review (GL, D&O, E&O, abuse/molestation, cyber, property), safeguarding and incident policy for programs serving minors or vulnerable adults, crisis response and business continuity. Use when asked 'do a risk assessment for our organization,' 'are we covered for this under our insurance,' 'we run programs for kids, what safeguarding policy do we need,' or 'build a business continuity plan.' Not for financial controls or fraud prevention (use nonprofit-financial-controls), donor data privacy (use nonprofit-data-privacy), or volunteer recruitment and onboarding (use nonprofit-volunteer-management)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Insurance and risk decisions need an informed owner, not a filing authority."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Risk Management

## Boundaries

This skill covers physical, reputational, program-safety and insurable risk.

- Internal financial controls, fraud and segregation-of-duties design: `nonprofit-financial-controls`.
- Donor data privacy, PCI compliance and data-sharing policy: `nonprofit-data-privacy`.
- Volunteer recruitment and general onboarding: `nonprofit-volunteer-management` (this skill's screening
  protocols feed into, but don't replace, that onboarding process).
- Executing media statements: `nonprofit-media-relations`. Full leadership pipeline planning:
  `nonprofit-succession-planning`.

## Core Framework: Enterprise Risk Management (ERM) for Nonprofits

Move beyond ad hoc "what could go wrong" brainstorming to a structured **risk register**:

1. **Identify** risks across categories: programmatic (harm to a client/beneficiary), financial
   (fraud, loss of major funding), operational (loss of facility, key-person dependency), reputational
   (media/PR crisis, social media incident), compliance/legal (regulatory violation, employment
   claim), and governance (board dysfunction, ED departure without succession plan — see
   `nonprofit-succession-planning`).
2. **Assess** each risk on likelihood and impact (a 5x5 heat map is the default) to prioritize, rather
   than treating every risk as equally urgent.
3. **Mitigate** each high-priority risk with a named strategy (avoid, reduce, transfer via insurance or
   contractual indemnification/waivers, or accept); document any decision to accept, usually for
   low-impact/low-likelihood items only.
4. **Assign ownership and review cadence** — a risk register with no named owner per risk and no
   review schedule (recommended: at least annually, presented to the board or a risk/audit committee)
   becomes a static document nobody revisits until after an incident occurs.
5. **Standard deliverable**: a risk register (spreadsheet or table) with columns for risk
   description, category, likelihood, impact, mitigation strategy, owner, status, and last-reviewed
   date.

## Insurance Coverage Review

Map coverage against the risk register rather than reviewing policies in isolation. What each policy
type misses is where the gaps hide:

- **General Liability (GL)** — baseline third-party injury/property damage; does not cover professional
  errors or abuse claims.
- **Directors & Officers (D&O)** — governance claims (e.g., wrongful termination allegations against the ED,
  a removed board member suing); pairs with the bylaws indemnification clause (`nonprofit-bylaws-policy`) —
  indemnification without D&O insurance behind it is hollow if the organization lacks funds to cover a claim.
- **Professional Liability / E&O** — claims from the service itself (clinical advice, legal-aid
  representation); essential for licensed or quasi-professional services, not covered by GL.
- **Abuse/Molestation Coverage** — a distinct rider or policy, NOT automatically included in GL or even
  umbrella policies; confirm explicitly for any organization serving minors, elderly or vulnerable adults
  (youth programs, camps, mentoring, disability services, some faith-based programs).
- **Property** — confirm replacement cost vs. actual cash value, and fit for owned vs. leased space (see
  `nonprofit-vendor-facilities` for lease-side obligations).
- **Cyber liability** — breach response, ransomware, cyber business interruption (coordinate with
  `nonprofit-data-privacy` on the underlying data practices).
- **Umbrella/excess** — raises limits above GL/auto/D&O more cheaply than buying up each underlying limit.
- **Volunteers and workers' comp** — confirm whether volunteers are covered under GL, a separate volunteer
  accident policy, or excluded; paid staff need workers' compensation per state law regardless of
  nonprofit status.

### Insurance Review Checklist

1. Pull the full list of current policies and their declarations pages (coverage limits,
   deductibles, exclusions).
2. Cross-walk against the risk register — for every "transfer via insurance" mitigation, confirm an
   actual policy covers it (not assumed).
3. Check named-insured accuracy — related entities (a supporting 501(c)(4), a fiscal-sponsored
   project) may not be automatically covered under the parent's policy unless specifically named
   (see `nonprofit-c3-c4-structure` and `nonprofit-mergers-fiscal-sponsorship`).
4. Review exclusions closely, especially abuse/molestation carve-outs and any communicable-disease
   or pandemic exclusions added since 2020.
5. Benchmark limits against peer organizations of similar size/activity via a broker who specializes
   in nonprofit coverage, not a generalist commercial broker.
6. Set an annual renewal review on the calendar, not just an auto-renewal default.

## Safeguarding and Incident Policy (Programs Serving Minors/Vulnerable Adults)

1. **Screening protocol**: criminal background checks (and, where relevant, sex-offender registry
   checks and reference checks) for every staff member and volunteer with unsupervised access to
   minors/vulnerable adults, re-run on a periodic cycle (commonly every 1-3 years), not just at hire.
2. **Two-adult rule / no-unsupervised-contact policy**: require two screened adults present for
   activities with minors, and prohibit one-on-one unsupervised contact (including electronic/social
   media contact) as a structural control, not a trust-based one.
3. **Mandatory reporting training**: train all staff/volunteers on state mandatory-reporter
   obligations for suspected abuse/neglect, including exact reporting channel and timeline (varies by
   state — confirm current law rather than assuming a uniform national rule).
4. **Incident reporting procedure**: a written, simple process any staff/volunteer/participant can use
   to report a concern, naming who receives reports (should include a channel outside the normal
   chain of command, mirroring the whistleblower channel design in `nonprofit-bylaws-policy`), the
   required response timeline, and escalation to law enforcement/child protective services where
   legally required.
5. **Board/ED notification protocol**: define which incident severities require immediate ED
   notification vs. board notification vs. legal counsel engagement — a common failure mode is an
   incident that should have reached the board getting stuck at the program-manager level.

Safeguarding policy skeleton:

```
[Organization] Safeguarding Policy — adopted [date], next review [date]
1. Scope: programs, roles and settings covered; who counts as a minor or vulnerable adult
2. Screening: checks required by role (background, registry, references); re-screen every [n] years
3. Conduct: two-adult rule; no one-on-one unsupervised contact, including electronic/social media
4. Training: mandatory-reporter obligations under [state] law; frequency; sign-off record
5. Reporting a concern: channels (including one outside the chain of command); who receives reports
6. Response: timeline; when law enforcement/child protective services is contacted (per [state] law)
7. Escalation: severity levels -> ED / board / legal counsel notification
8. Records: where incident records are kept, who can access them, retention period
9. Insurance: abuse/molestation coverage confirmed (policy, limit, date checked)
```

## Crisis Response and Business Continuity

1. **Crisis response plan** structure: activation trigger (what counts as a crisis), a named crisis
   team with backup designees (not just one person who might be unreachable), a communications
   protocol (internal staff/board notification before external statements), designated spokesperson,
   and a decision log kept during the event.
2. **Draft holding statements in advance** for foreseeable scenarios (safety incident, financial
   scandal, natural disaster affecting facility/clients) so the first public response doesn't have to
   be composed from scratch under pressure — coordinate with `nonprofit-media-relations` for
   execution mechanics once a statement is needed.
3. **Business continuity/disaster recovery plan**: identify single points of failure (one person who
   knows the payroll system, one physical location for all records) and mitigate — offsite/cloud
   backup of critical records, a documented emergency operating procedure if the primary facility is
   unusable, and a named line of authority succession if the ED is suddenly unavailable (full
   leadership pipeline planning is `nonprofit-succession-planning`; this skill covers the emergency-
   authority stopgap specifically).
4. **Test the plan** — a tabletop exercise annually with the crisis team walking through a realistic
   scenario surfaces gaps a written plan alone won't reveal.

## Standard Deliverables

- Risk register (categorized, scored, mitigation-assigned, owned)
- Insurance coverage cross-walk against the risk register with gap list
- Safeguarding policy (screening protocol, two-adult rule, mandatory reporting training plan)
- Incident reporting procedure with escalation thresholds
- Crisis response plan with holding statements
- Business continuity/disaster recovery plan

## For advisors

- Start from the risk register, not the insurance policy; buying more coverage first wastes budget on the
  wrong lines and leaves real gaps (most commonly abuse/molestation) unaddressed.
- Use the insurance cross-walk as a fast, concrete diagnostic to open a broader risk conversation with a
  client board; a missing abuse/molestation rider or an unnamed related entity on a D&O policy are specific,
  credible findings.

## Common Failure Modes

- **Assuming GL covers abuse claims** when the policy explicitly excludes them; this is a shockingly common gap.
- **Related entity not named** — a supporting 501(c)(4) or fiscal-sponsored project left off the parent's
  policies.
- **Incident stuck at program level** — an incident that should have reached the ED or board never leaves
  the program manager.
- **Single-person crisis team** with no backup designees, so the plan fails when that person is unreachable.
- **Risk register with no owner or review date**, so nobody revisits it until after an incident.
- **Screening only at hire**, with no periodic re-screen for staff and volunteers with unsupervised access.
- **Untested crisis plan** — no tabletop exercise before an actual crisis.
