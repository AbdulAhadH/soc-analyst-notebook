# SOC Analyst Notebook

Notes and investigation writeups from my progress the SOC Level 1 analyst path.
Each investigation is written the way an analyst would hand a case to their team lead:
what happened, how I found it, and what should change so it doesn't happen again.

Currently working through: TryHackMe SOC Level 1

## Investigations

Root-cause writeups from hands-on rooms. (First one lands at the alert triage module.)


## Notes

| Topic | What it covers |
|---|---|
| [SOC Role in Blue Team](notes/soc-role-in-blue-team.md) | How a SOC is structured and where an L1 analyst sits in it |
| [SOC L1 Alert Triage](notes/soc-l1-alert-triage.md) | Alert lifecycle, fields, and how priority gets decided |
| [SOC L1 Alert Reporting](notes/soc-l1-alert-reporting.md) | How and when to escalate, and what makes a good case report |

## Alert Triage Log

[Running log](triage-log/alert-log.md) of every alert I've triaged

## Investigations

Write-ups for more complex alerts 

| ID | Title | Verdict | Link |
|---|---|---|---|
| 001 | Web Shell Compromise | True Positive — Escalated | [View](investigations/001-exchange-webshell-compromise.md) |
