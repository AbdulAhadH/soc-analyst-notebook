# Alert Triage Log

Every alert I've triaged, in order. 
This is a working log,not a one-time writeup — new rows get added as I go through the path.

| Date | Room / Source | Alert | My Verdict | Why | Priority |
|---|---|---|---|---|---|
| 2026-09-20 | SOC L1 Alert Triage | "Double-Extension File Creation" | True Positive | Double extension ".exe" is present after the .mp4, phishing attack to trick the user to run the executable | Default Assigned: High |
| 2026-09-20 | SOC L1 Alert Triage | "Potential Data Exfiltration" | False Positive | Flagged for +5GB of data sent from one device, this case was due to zoom call| Default Assigned: Critical |
| 2026-09-20 | SOC L1 Alert Triage | "Download from GitHub Repository" | False Positive | Github download from developer from verified source: github.com/facebook/react | Default Assigned: Low |
| 2026-09-21 | SOC L1 Alert Reporting | "Spike of Domain Discovery Commands" | True Positive | Compromising the server, domain discovery | Default Assigned: Medium |
| 2026-09-21 | SOC L1 Alert Reporting | "Email Marked as Phishing after Delivery" | True Positive | Phishing attempt to gain access to data | Default Assigned: Medium |
