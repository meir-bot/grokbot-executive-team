# Running several projects

How to run several projects with shared department heads. Each project gets a Project CEO. A project can be a product, a business unit, or a company.

One project needs nothing extra: Chief Of Staff and the department heads are the whole team. Several projects keep that same team and add a Project CEO for each project.

## What you set up

- Add one **Project CEO** bot per project from [agents/project-ceo.md](../agents/project-ceo.md), replacing `<Project>` with its name.
- Each Project CEO reports to **Chief Of Staff**. Department heads stay shared across every project: CTO/Product, CFO/Finance, CIO/Ops & IT, CMO, CLO, CSO, Hiring Manager, and the teams under them (marketing, Sales Desk, product build, finance desk, Contract Desk). Do not copy them per project. Personal ops (To Do's, Travel, Save Me Money, Credit Card Max) and the Chief Of Staff specialists stay shared too.
- Each Project CEO sends a daily report (Sun-Fri, before ~8am, none on Shabbat): decisions needed, what's going on, what's next, 5 growth ideas.
- Chief Of Staff's **daily briefing** combines the Project CEO reports with the department heads' and Hiring Manager's input: decisions from every project at the top, a short status per project, then the best 5 growth ideas overall. Group status by department or by project.
- The CFO already splits costs per department or project, so the monthly expense report shows spend per project with no extra setup. Jevopus's coding-seat log is part of that report.

```text
You (CEO/exec)
  |
Chief Of Staff            daily briefing: decisions on top, status per project, 5 growth ideas
  |
  +-- <Project> CEO       one per project (product, business unit, or company)
  +-- Department heads    CTO/Product · CFO/Finance · CIO/Ops & IT · CMO · CLO · CSO · Hiring Manager, shared
  |     +-- their teams   product build, finance desk, Contract Desk, marketing, Sales Desk
  +-- Personal ops        To Do's · Travel · Save Me Money · Credit Card Max, shared
  +-- Under Chief Of Staff   Bot Org Auditor · Bot Builder · Research Desk · Specialist/research
  +-- Dotted line         Creative Director · LinkedIn Outreach (CMO) · Jevopus to CFO
```

## How to turn it on

Answer "several" to **"One project, or several?"** in the [setup prompt](../setup-prompt.md), and list each project. Or ask Chief Of Staff later to add a Project CEO for a project. Remove a Project CEO bot when that project ends.
