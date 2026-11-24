# Nonprofit Skills (GVP subset)

57 skills for Gemini covering nonprofit advocacy, fundraising, governance, finance, communications,
programs and volunteers. Once you add a skill, Gemini uses it on its own when your request matches,
or you can pick it by typing `/` in a chat.

Selected from [sector-skills/nonprofit-skills](https://github.com/sector-skills/nonprofit-skills)
(MIT license, commit `9a7f196`) and unchanged from the original. They are general nonprofit
guidance, not specific to gun violence prevention.

## Add skills to Gemini

Gemini adds skills one at a time, so start with the ones you'll actually use (see the starter set
below).

1. **Download this repo once.** Click the green **Code** button at the top of this page, then
   **Download ZIP**, and unzip it. Each skill is a folder inside `skills/`.
2. **Open Gemini** at [gemini.google.com](https://gemini.google.com) and click **Customize** in
   the left sidebar, then the **Skills** tab.
3. Click **Create**, then **Upload**.
4. Select the `SKILL.md` file inside the skill's folder (for example
   `skills/nonprofit-grant-writing/SKILL.md`).
5. Click **Upload** (skip the optional extra files), check that the name and description filled
   in, then click **Create**. You'll see "Skill created" and the skill under **Installed**.

Repeat steps 3–5 for each skill you want. You can have up to 100 active skills. To remove one, use
the **⋯** menu next to it on the Skills page.

## Starter set

The 10 most useful for advocacy work:

| Skill | Use it for |
|---|---|
| [nonprofit-grassroots-mobilization](skills/nonprofit-grassroots-mobilization/SKILL.md) | Action alerts, petitions, click-to-call, rapid response |
| [nonprofit-legislative-advocacy](skills/nonprofit-legislative-advocacy/SKILL.md) | Legislator meetings, lobby days, testimony |
| [nonprofit-policy-analysis](skills/nonprofit-policy-analysis/SKILL.md) | Issue briefs, bill analysis, position papers |
| [nonprofit-coalition-building](skills/nonprofit-coalition-building/SKILL.md) | Multi-org coalitions and MOUs |
| [nonprofit-voter-engagement](skills/nonprofit-voter-engagement/SKILL.md) | Nonpartisan voter registration, GOTV, candidate forums |
| [nonprofit-c3-c4-structure](skills/nonprofit-c3-c4-structure/SKILL.md) | c3/c4 rules, 501(h) lobbying limits, shared-staff allocation |
| [nonprofit-media-relations](skills/nonprofit-media-relations/SKILL.md) | Press releases, pitching, spokesperson prep |
| [nonprofit-storytelling](skills/nonprofit-storytelling/SKILL.md) | Ethical stories, consent and interview protocols |
| [nonprofit-social-media](skills/nonprofit-social-media/SKILL.md) | Content calendars and platform strategy |
| [nonprofit-grant-writing](skills/nonprofit-grant-writing/SKILL.md) | LOIs and full grant proposals |

## All skills

Folder names start with `nonprofit-` (for example `nonprofit-grant-writing`).

- **Advocacy & Policy:** coalition-building, grassroots-mobilization, legislative-advocacy, policy-analysis, voter-engagement
- **Governance & Compliance:** board-governance, bylaws-policy, c3-c4-structure, charitable-registration, form-990, risk-management
- **Communications:** annual-report, brand-messaging, donation-page-copy, email-newsletter, media-relations, social-media, storytelling
- **Fundraising:** annual-appeals, capital-campaigns, corporate-sponsorships, donor-pipeline, donor-retention, fundraising-events, grant-research, grant-writing, major-gifts, peer-to-peer-fundraising, planned-giving
- **Finance & Operations:** budgeting, cost-allocation, financial-controls, financial-statements, hr, reserves-cash-flow, vendor-facilities
- **Programs & Impact:** needs-assessment, outcomes-measurement, program-design, program-scaling
- **Volunteers & People:** board-recruitment, staff-retention, succession-planning, volunteer-management
- **Strategy:** change-management, eos-traction, mergers-fiscal-sponsorship, revenue-diversification, strategic-planning
- **Technology & Data:** data-privacy, digital-fundraising-tools, donor-crm
- **Executive Leadership:** ceo-board-partnership, executive-communications, executive-dashboard, executive-search, executive-transitions

The housing, arts, faith-based, retail and community-finance collections from the original library
were left out, so a few skills mention sibling skills that aren't here.

## Other tools

The same `skills/` folders work in Claude Code (copy them to `~/.claude/skills/`) and other agents
that read `SKILL.md` files. `plugin.json` lets Antigravity install the whole set as a plugin.

## License

MIT. See [LICENSE](LICENSE). Original work by the
[Nonprofit Skills](https://github.com/sector-skills/nonprofit-skills) contributors.
