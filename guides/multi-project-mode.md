# Multi-project mode (optional)

The default team runs **one company or team**. Use this mode if you run several projects or business units and want each one tracked on its own.

## What changes

- Add one **Project CEO** bot per project from [agents/optional-project-ceo.md](../agents/optional-project-ceo.md), replacing `<Project>` with its name.
- Each Project CEO reports to **Chief Of Staff**. The department heads (CTO/Product, CFO/Finance, CIO/Ops & IT, CMO and the marketing team) stay shared across all projects.
- Each Project CEO sends a daily report (Sun-Fri, before ~8am, none on Shabbat): decisions needed, what's going on, what's next, 5 growth ideas.
- Chief Of Staff's **daily digest** combines the Project CEO reports with the department heads' input: decisions from every project at the top, a short status per project, then the best 5 growth ideas overall.
- The CFO already splits costs per department or project, so the monthly expense report shows spend per project with no extra setup.

```text
You (CEO/exec)
  |
Chief Of Staff            daily digest: decisions on top, status per project, 5 growth ideas
  |
  +-- <Project> CEO bots  one per project or business unit; daily report to Chief Of Staff
  +-- Department heads    CTO/Product · CFO/Finance · CIO/Ops & IT · CMO (+ marketing team), shared
  +-- Supporting bots     Creative Director · LinkedIn Outreach · Specialist/research
```

## Turning it on

Answer "several projects" to the question in the [setup prompt](../setup-prompt.md), or ask Chief Of Staff later to add a Project CEO for each project. Remove a Project CEO bot when its project ends.
