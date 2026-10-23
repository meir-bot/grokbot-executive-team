# Setup prompt

Create a bot called Chief Of Staff, paste this into its chat, and answer its question.

```text
Set up my Grok Bot executive team from the grokbot-executive-team repo.

1. Read README.md, guides/rules.md, guides/multi-project-mode.md and every
   file in agents/.
2. Ask me one question, then wait: "One project, or several?"
   (A project can be a product, business unit, or company. If I say several,
   I'll list them, one line each on what they do.)
3. Take on the Chief Of Staff instructions from agents/01-chief-of-staff.md.
   I am the CEO/exec at the top; you are the hub under me.
4. Create every bot below with the instructions block from its file. Keep
   every standing rule exactly as strict as written. All of them are shared
   across projects. Do not copy them per project.
   Department heads, reporting to you: CTO/Product, CFO/Finance, CIO/Ops & IT,
   CMO, CLO (Chief Legal Officer), CSO (Chief Security Officer; security, not
   sales), Hiring Manager.
   Under the CTO: Jevopus (dotted line to the CFO), QA Bot, Prototyper, PM Bot.
   Under the CFO: Spend Negotiator, Expense & Invoice Desk.
   Under the CLO: Contract Desk.
   Under the CMO: SEO/GEO, Social Media, Content, Paid Ads, Marketing Analyst,
   Growth & Partnerships, Email & Lifecycle, Competitor Watch, Clip & Video
   Editor. Creative Director and LinkedIn Outreach on a dotted line to the CMO.
   Under Growth & Partnerships, the Sales Desk: Outbound Prospecting, Signal
   Prospector, Follow-through, Sales Call Coach.
   Personal ops, reporting to you: To Do's, Travel, Save Me Money, Credit Card Max.
   Under you: Bot Org Auditor, Bot Builder, Research Desk, Specialist / Research.
5. If I said several projects, create one "<Project> CEO" bot per project
   from agents/project-ceo.md, replacing <Project> with each name. That is
   the setup for several projects: each Project CEO reports to you, and the
   department heads stay shared. If I said one project, do not create a
   Project CEO.
6. Create these routines, and no others:
   - Chief Of Staff: daily briefing, Sunday-Friday about 8am my time, none
     on Saturday (Shabbat). Decisions at the top, what's going on (by
     department, or by department or project when I run several), what's
     next, 5 growth ideas, combined from each department head and Hiring
     Manager (and from each Project CEO when I run several projects).
   - CFO: monthly expense report on the 1st, per department or project,
     including the coding-seat spend Jevopus logs. QA Bot's daily tests fold
     into the CTO's briefing input. Do not create any other routine.
7. Use the time zone from my account settings; ask only if it isn't set.
8. Show me what you created and anything I must finish in the app.

During setup do not connect tools, send messages or spend money.
```
