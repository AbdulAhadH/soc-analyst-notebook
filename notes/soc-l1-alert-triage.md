# SOC L1 Alert Triage

Source: TryHackMe — SOC Level 1, SOC L1 Alert Triage
Date: 2026-09-20

## Why this matters

Learning about SOC alers, how they are categorized, and the effective methods of triaging these alerts.

## What an L1 analyst actually does in a shift

- Views and recieves multiple alerts on a daily basis
- Review alerts, view on a categories basis distinguish the bad from the good
- If malcicious the alert will be True Positive, if not a False Positive
- Alerts are assigned to me and the status is updated
  - Read alert's name and description (Understand who is under threat, and note the action described in the alert)
  - Note the alert fields: (IP, host, user) 
  - Check if a workbook or SOP is in place
  - Follow the steps if a workbook exists, if not invesitgate the activity
  - Make the final decision to escalate or comment and move the alert to closed
- Triage attacks and pass complex ones to L2
- Protect the company systems

## Alert prirotisation

- Filter the alerts for those not assigned to someonelse
- Sort the alerts by severity; critical, high, medium, low
- Sort by time: oldest first to newest (same severity the newcomer would have just started compared to an older alert)

## What I got wrong or didn't know

- Initially missed that for the Potential Data Exfiltration, large amount of data was due to *.zoom.us as destination

## Questions I still have

- Interested in seeing more types of alerts
- How workbook looks, or the detailed process when the workbook does not exist
- How detailed comments are expected to look
