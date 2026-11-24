# Nonprofit Skills (GVP subset)

57 agent skills for nonprofit work, selected from
[sector-skills/nonprofit-skills](https://github.com/sector-skills/nonprofit-skills) (MIT license,
commit `9a7f196`). Each skill is a folder in `skills/` with one `SKILL.md`. Your agent loads a
skill automatically when a request matches its description.

The skills are unchanged from the original. They are general nonprofit guidance, not specific to
gun violence prevention. The housing, arts, faith-based, retail and community-finance collections
were left out, so a few skills mention sibling skills that aren't here.

## Install

### Easiest: ask your agent
Paste this into Gemini / Antigravity:

> Install the agent skills from https://github.com/archizzl/nonprofit-skills-gvp. Clone the repo and
> copy every folder inside its `skills/` directory into my global skills folder
> (`~/.gemini/config/skills/` for Antigravity, `~/.gemini/skills/` for Gemini CLI or Antigravity
> CLI). Then confirm the skills are listed.

### Antigravity CLI (as a plugin)
```bash
agy plugin install https://github.com/archizzl/nonprofit-skills-gvp
```
Skills install as `nonprofit-skills-gvp:<skill-name>`. Check with `agy plugin list`.

### Manual
```bash
git clone https://github.com/archizzl/nonprofit-skills-gvp.git
mkdir -p ~/.gemini/config/skills
cp -R nonprofit-skills-gvp/skills/* ~/.gemini/config/skills/
```
For Gemini CLI, copy to `~/.gemini/skills/` instead. For Claude Code, copy to `~/.claude/skills/`.

## Skills

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

## License

MIT. See [LICENSE](LICENSE). Original work by the
[Nonprofit Skills](https://github.com/sector-skills/nonprofit-skills) contributors.
