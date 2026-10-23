# Routines

Setup creates two routines: the morning briefing and the monthly expense report. Every other routine in this repo is a suggestion. They are **off by default**. Enable one only after you have run it by hand and it still earns its place.

Per-bot schedules are in each file under **Suggested routines**.

## Shabbat-aware default

This is the default, and you can change it.

- Nothing on Saturday.
- Nothing on Friday after 14:00 local time. Friday morning is fine.
- Sunday morning is fine.
- If a monthly date falls on Saturday, run it Sunday morning.

Cron in the bot files is local time: `min hour dom mon dow`. `0` is Sunday. `5` is Friday. `6` is Saturday. A source that said "Friday afternoon" is already moved to Friday morning or Thursday in the bot file.

## Most-recommended routines online

Public posts, ranked by likes and bookmarks. The ranking will go stale. These are patterns, not routines this template turns on.

| # | Routine | Cadence | Link |
|---|---|---|---|
| 1 | Weekday pre-market brief: filings, analysts, insiders, public sentiment | Weekday, before the open | [@SPCX100T](https://x.com/SPCX100T/status/2110145512020279726) |
| 2 | Self-updating pages: revenue vs plan, a morning brief, competitor changes, a monthly memo that is never sent | Monday 8:00, daily 7:00, monthly | [@distortgeekin](https://x.com/distortgeekin/status/2113261664694894731) |
| 3 | Backup of the whole bot setup, saved outside the account, with no secrets | Recurring; this template suggests Sunday 10:00 | [@Michael_Fenech_](https://x.com/Michael_Fenech_/status/2112204877971821055) |
| 4 | Plus-alias email triggers: a routine runs only when mail arrives at one address | Event | [@bot](https://x.com/bot/status/2111184278377857410) |
| 5 | Sunday week plan, a short weekday evening review, Monday "5 people to check in with" | Weekly and weekday. Move any Friday evening pass to Friday morning | [@coreyganim](https://x.com/coreyganim/status/2112663410043470281) |
| 6 | Weekly "release notes vs my setup" | Monday 8:00 | [@Michael_Fenech_](https://x.com/Michael_Fenech_/status/2108145378323542306) |
| 7 | Script this routine: turn a rule-based routine into a plain script | Periodic. This template puts it on the CIO on the 1st at 13:00, after the other month-open jobs | [@Kevin_Logan](https://x.com/Kevin_Logan/status/2112505666942407076) |
| 8 | Usage fixes: slow the fastest routine, working hours only, move routines off the chat bot | One pass, then sometimes | [@GrokBotRadar](https://x.com/GrokBotRadar/status/2111513393538732162) |
| 9 | Routine audit: KEEP / SLOW DOWN / EVENT TRIGGER / CHANGE CHECK / RETIRE | Monday, or monthly. One owner | [@Michael_Fenech_](https://x.com/Michael_Fenech_/status/2111478843202818102), [@GrokBotRadar](https://x.com/GrokBotRadar/status/2112010598276030605) |
| 10 | Content system: daily public-post scout, a weekly metrics log, a Monday plan | Daily and weekly | [@AIGuide_](https://x.com/AIGuide_/status/2111645720050651605) |
| 11 | Cut mailbox scans from every 15–30 minutes to twice a day | Twice a day | [@GrokBotRadar](https://x.com/GrokBotRadar/status/2110086951500169474) |
| 12 | Read-only social routines: creator scout, shoutouts, mention radar, a rare follower audit | Mixed. Mention radar in this template skips Friday afternoon | [@GlennHasABeard](https://x.com/GlennHasABeard/status/2111935110929174714) |
| 13 | Weekday inbox triage with a "done when" line | Weekday 7:15 | [@GrokBotRadar](https://x.com/GrokBotRadar/status/2107188270669148319) |

## General advice

- **Keep routines few.** A public GTM team went from 10 routines to 1 ([their rules](https://github.com/timscheuerai/grokbot-gtm-team/blob/main/guides/rules.md)). This repo's [standing rules](rules.md) say the same. A new routine must produce something the exec reads every time.
- **Prefer event triggers to polling.** A schedule every 5 minutes is about 8,640 runs a month ([@fleyta88](https://x.com/fleyta88/status/2111522091316990308)).
- **Stay silent when nothing changed.**
- **Run by hand, then save it as a skill, then schedule it** ([field notes](https://github.com/unicodef1wn/grokbot-field-notes/blob/main/agents/SKILLS-AND-ROUTINES.md), [@GrokBotRadar](https://x.com/GrokBotRadar/status/2110423210886111472)).
- **Hiding a bot does not stop its routines** ([@GrokBotRadar](https://x.com/GrokBotRadar/status/2105513032915038493)). Turn the routine off.
- **Stagger the 1st-of-month jobs.** Do not run them in one pile. If the 1st is Saturday, run the set Sunday morning, same order:

  | Local time | Job | Owner |
  |---|---|---|
  | 7:00 | Bot portfolio review, only if this bot owns that audit | Bot Org Auditor |
  | 8:00 | Card perk rollup, not a budget review | Credit Card Max |
  | 9:00 | Monthly expense report. Setup creates this one | CFO |
  | 10:00 | Marketing monthly | Marketing Analyst |
  | 11:00 | Company vendor refresh | Spend Negotiator |
  | 12:00 | Personal subscription inventory | Save Me Money |
  | 13:00 | Script-this-routine review | CIO |

- **Fold daily inputs into the one morning briefing.** Department heads, Hiring Manager, Project CEOs, the PM attention list, QA results, and the daily task readback go into that briefing. They do not each message the exec.
- **One owner per overlapping job.** Leave the others off.
  - Routine audits: Chief Of Staff weekly usage audit. Not also Bot Org Auditor's weekly review, Bot Builder's routine healthcheck, and the CIO script review.
  - Contract intake: Contract Desk does the first pass. The CLO owns the legal judgment and the notice-date watch. One "a contract arrived" trigger.
  - Receipts: Expense & Invoice Desk. The CFO does not also log them.
  - Vendor lists: Spend Negotiator for company tools, Save Me Money for personal subscriptions, CFO for the monthly expense report.
  - Script-this-routine: CIO. Not Jevopus.
  - First-touch drafts: Outbound Prospecting for the prospect list. LinkedIn Outreach for LinkedIn replies.
  - Renewal dates: CLO for notice and auto-renew terms. Spend Negotiator for a price talk inside 120 days.
  - Search and AI-answer reports: SEO/GEO. The CMO only passes the morning briefing input.
