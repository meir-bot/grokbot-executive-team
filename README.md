# Grok Bot Lev Group team

**A multi-company AI org in Grok Bot: one Chief Of Staff hub, a CEO bot per company, a shared exec team, and the rules they all work by.**

![Org chart](assets/org-chart.png)

Inspired by [Tim Scheuer's grokbot-gtm-team](https://github.com/timscheuerai/grokbot-gtm-team). Same idea and layout, rebuilt for running several companies at once.

**[Create the team in 1 prompt](setup-prompt.md)** · [The team](#the-team) · [The rules](guides/rules.md)

## Set up the team

1. Create a new bot in Grok Bot and call it **Chief Of Staff**.
2. Paste the prompt from [setup-prompt.md](setup-prompt.md) into its chat.
3. Answer its questions (your companies, which bots you want, your time zone). It creates the rest and the routines.
4. Connect tools in settings. Each bot's file lists the connectors it may use.

Nothing is sent or spent during setup. Every file in [agents/](agents/) also has the block to paste by hand.

## The team

| Bot | Job | Reports to |
|---|---|---|
| Owner (human) | Sets goals, approves anything irreversible | |
| [Chief Of Staff](agents/01-chief-of-staff.md) | The hub. Routes work, combines the daily CEO digest, sends everything as drafts. | Owner |
| [<Company> CEO](agents/02-company-ceo.md) | One per company. Daily report: what's going on, what's next, 5 growth ideas. | Chief Of Staff |
| [CTO](agents/03-cto.md) | Code via cloud agents, staging first. | Chief Of Staff |
| [CFO](agents/04-cfo.md) | Tool costs split per project; monthly expense report on the 1st. | Chief Of Staff |
| [CIO](agents/05-cio.md) | Infra, domains and DNS on Vercel, keys, vendors. | Chief Of Staff |
| [CMO](agents/06-cmo.md) | Leads the marketing team across all companies. | Chief Of Staff |
| [SEO/GEO](agents/07-seo-geo.md) | Search ranking and visibility in AI answers. | CMO |
| [Social Media](agents/08-social-media.md) | Social channels, post drafts, calendar. | CMO |
| [Content](agents/09-content.md) | Blog, landing page and long-form copy. | CMO |
| [Paid Ads](agents/10-paid-ads.md) | Ad campaigns and budgets, drafts only. | CMO |
| [Marketing Analyst](agents/11-marketing-analyst.md) | Funnel and campaign metrics, mostly from PostHog. | CMO |
| [Growth & Partnerships](agents/12-growth-partnerships.md) | Partnerships, referrals, growth experiments. | CMO |
| [Email & Lifecycle](agents/13-email-lifecycle.md) | Onboarding, newsletters and lifecycle sequences. | CMO |
| [Creative Director](agents/14-creative-director.md) | Visual identity, design assets, brand consistency. | CMO (dotted line) |
| [LinkedIn Outreach](agents/15-linkedin-outreach.md) | LinkedIn prospecting and message drafts. | CMO (dotted line) |
| [Directory Research (specialist)](agents/16-directory-research.md) | Builds and enriches a directory from public sources. | Chief Of Staff |

## How the work flows

```text
Owner (human)        goals and approvals; sends what bots draft
  |
Chief Of Staff       routes every request to one owner; daily digest, decisions on top
  |
  +-- <Company> CEO bots   one per company; daily report: status, next, 5 growth ideas
  +-- Shared execs         CTO (code, staging first) · CFO (costs) · CIO (infra, DNS) · CMO
  |     +-- CMO team       SEO/GEO · Social · Content · Paid Ads · Analyst · Growth · Email
  |     :.. dotted line    Creative Director · LinkedIn Outreach
  +-- Specialist bots      one narrow job, e.g. directory research / enrichment
  |
Drafts back to the owner  nothing irreversible happens without an explicit OK
```

## Routines

| Routine | When | Who |
|---|---|---|
| Daily CEO report | Sun-Fri ~8am, skipping Shabbat | Each Company CEO bot, combined by Chief Of Staff |
| Monthly expense report | 1st of each month | CFO |

## License

[MIT](LICENSE).
