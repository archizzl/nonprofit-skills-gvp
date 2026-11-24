---
name: nonprofit-needs-assessment
description: "Plans and conducts community needs assessments and landscape/gap scans to justify launching, continuing, or sunsetting a nonprofit program: secondary data, surveys, focus groups and key informant interviews, asset mapping, and gap analysis against existing providers. Use when asked \"is there actually demand for this program,\" \"the funder wants evidence of need,\" \"who else serves this population,\" or \"should we sunset this program.\" Not for designing the program once need is established (use nonprofit-program-design) or measuring a running program's outcomes (use nonprofit-outcomes-measurement)."
license: MIT
metadata:
  supervision: "review"
  supervision_note: "Primary data collection involves human participants and consent."
  date_added: "2026-09-07"
  date_added_source: "git:1860ed47a83901ff5e6d45abc4a2ef05be8fd4cd"
---

# Nonprofit Needs Assessment

## Boundaries

- This skill stops at "here is the documented need and the gap." Building the logic model/theory of
  change for the response is `nonprofit-program-design`; hand off a continue-and-redesign finding there.
- Tracking whether a running program achieves outcomes is `nonprofit-outcomes-measurement`; a needs
  assessment is a point-in-time (or periodic, e.g., every 3–5 years) study, not ongoing monitoring.
- Assessing a funder's or partner's fit rather than a community's need is `nonprofit-grant-research`.

## Core Frameworks

### 1. Needs Assessment Triangulation Model

Credible needs assessments triangulate three data types — do not rely on only one:

1. **Secondary/quantitative data**: existing public data (default starting set: Census/ACS, county
   and state health department data, school district data, 211 call data, and existing needs
   assessments from hospitals/United Ways/community foundations that may already cover the geography;
   add domain sources such as HUD point-in-time counts as relevant).
2. **Primary quantitative data**: surveys of the target population or service providers, structured
   to produce comparable numbers (Likert-scale need ratings, service utilization/barriers surveys).
3. **Primary qualitative data**: key informant interviews (service providers, government officials,
   faith/community leaders), focus groups, and community listening sessions/town halls with the
   population itself — essential for capturing lived experience that administrative data misses, and
   for avoiding a needs assessment that speaks *about* a community rather than *with* it.

A needs assessment built on secondary data alone is the most common quality shortfall funders and
evaluators flag — it documents that a problem exists in the abstract but not that this specific
population, in this specific service area, experiences it in a way this organization is positioned
to address.

### 2. Asset Mapping / Landscape Scan

Before concluding a gap exists, map what already serves the population:
- **Provider inventory**: who else offers this or an adjacent service in the geography (name,
  capacity/slots, eligibility criteria, waitlist status, funding source).
- **Community assets, not just deficits**: existing informal supports, cultural/faith institutions,
  natural helpers — use an assets-based (vs. purely deficit-based) framing; many funders expect it,
  and it avoids a report that only catalogs problems.
- **Capacity vs. demand gap**: the actual gap is rarely "no service exists" — more often it's
  insufficient capacity, wrong eligibility criteria, wrong hours/location/language access, or long
  waitlists. Name the *specific* gap type; "duplicative service" is a common and damaging finding if
  the scan is skipped.

### 3. Gap Analysis Structure

State findings as: **Need (documented) → Current capacity (mapped) → Gap (the delta) → Implication
for this organization** (fill gap directly, partner/refer instead of duplicating, or no organizational
role). A needs assessment that stops at documenting need without this last step gives leadership
nothing decision-ready.

## Instructions

1. **Define the population and geography precisely** before collecting anything — "youth in our
   city" is not scoped enough to find or design data collection against; specify age range,
   neighborhood/zip codes, and the specific condition/need domain.
2. **Start with secondary data** to build a baseline picture and identify what's already known —
   check county/city health departments, Census/ACS, school districts, United Way/community
   foundation reports, and 211 data before commissioning any primary research.
3. **Identify the secondary-data gaps** — what the existing data can't tell you (usually: lived
   experience, specific barriers, why people don't access existing services) — and design primary
   data collection specifically to fill those gaps, not to re-confirm what secondary data already
   shows.
4. **Run the landscape/asset scan** in parallel: inventory other providers, their capacity, and
   eligibility/access barriers (cost, hours, language, transportation, documentation status, waitlists).
5. **Design primary data collection instruments** matched to the audience: short structured surveys
   for broad reach/quantifiable ratings; key informant interviews for providers and community
   leaders; focus groups or listening sessions for the population itself, held in accessible
   locations/languages/times and, where appropriate, with compensation for participants' time.
6. **Recruit for representativeness**, not convenience — flag and mitigate selection bias (e.g., only
   surveying people already engaged with the organization systematically overstates satisfaction and
   understates unmet need among the unserved).
7. **Synthesize with the triangulation model**: look for convergence and divergence across secondary
   data, primary quantitative data, and qualitative input — divergence is often the most important
   finding (e.g., data shows a service exists, but the community reports it's inaccessible).
8. **Run the gap analysis**: need → current capacity → the specific gap → organizational implication
   (fill it, refer/partner, or stand down).
9. **Write the needs assessment report** with the standard structure: executive summary, methodology
   (data sources, sample sizes, response rates, limitations), findings by data source, landscape/asset
   map, gap analysis, and recommendations.
10. **Set a revisit cadence** — needs assessments go stale; recommend refreshing every 3–5 years or
    on a major demographic/funding/policy shift, and say so in the report so it isn't treated as a
    one-time artifact.

## Verify Before Acting

- [ ] Population, age range, and geography (zip codes/neighborhoods) are stated precisely in the report.
- [ ] Every finding cites its data source and year; secondary figures are pulled from the current
      release at the named agency (e.g., Census/ACS, county health department), not copied from an
      older report.
- [ ] Methodology states sample sizes, response rates, recruitment method, and limitations,
      including selection bias.
- [ ] All three data types are present (secondary, primary quantitative, primary qualitative), and
      divergences are reported rather than smoothed over.
- [ ] Participant consent, privacy, and compensation were handled as planned before data collection.
- [ ] The landscape scan was completed and each gap ends in an organizational implication (fill,
      refer/partner, or stand down).

## Common Failure Modes

- **Secondary-data-only assessments** presented as if they establish local, specific need — always
  include primary data and community voice; funders commonly probe for both.
- **Skipping the landscape scan**, leading to a program proposal that duplicates an existing,
  underused service instead of addressing the real gap (access, capacity, or eligibility).
- **Deficit-only framing** that ignores existing community assets and reads as extractive rather than
  collaborative — a weakness with funders committed to community-centered/equity-based grantmaking.
- **Non-representative sampling** — surveying only people already in the organization's database,
  systematically missing the unserved population the assessment is supposed to reach.
- **No compensation or accessibility planning** for community participants (transportation, child
  care, language, timing), which suppresses turnout from exactly the population most affected.
- **Stopping at "need exists"** without a gap analysis or organizational-implication statement,
  leaving the board/funder with a diagnosis but no decision.
- **Treating the assessment as one-and-done** rather than setting a refresh cadence, so program
  decisions rest on years-stale data.

## For Advisors/Consultants

- Scope the engagement explicitly around the triangulation model — clients often request "a needs
  assessment" meaning only a secondary-data literature review; clarify budget/timeline needed to add
  primary qualitative and quantitative components, since this is where most of the client's credibility
  with funders and community stakeholders is actually built.
- When facilitating listening sessions/focus groups for a client, build in a debrief step with the
  client's staff or board on findings that challenge existing assumptions — needs assessments that
  surface uncomfortable findings (e.g., "your flagship program isn't reaching the population with
  greatest need") are the ones most likely to be quietly shelved without a structured decision
  conversation attached.
- Where the client's real question is "should we keep funding this program," reframe the assessment
  around an explicit sunset/continue/redesign decision; the board memo should translate the gap
  analysis into 2–3 concrete organizational options.

## Standard Deliverables

- Needs assessment report: executive summary, methodology, findings, landscape/asset map, gap
  analysis, recommendations, limitations
- Data collection instruments (survey, interview guide, focus group protocol)
- Provider/asset inventory table
- Gap analysis summary (need → capacity → gap → implication)
- Board/funder-facing summary memo with a recommended organizational response
