# Introduction to EDR

**Source:** TryHackMe, SOC Level 1, Core SOC Solutions
**Date:** October 12

## What EDR is

It collects information from endpoints.
It provides visibility into what’s happening on a system.
It helps security teams detect, investigate, and respond to threats.

## How it's different from antivirus

Antivirus (AV) is like the immigration check at the airport. It scans your bags against a list of known forbidden items.

EDR is like an airport CCTV and security team. Even if something slips past immigration, EDR can still notice unusual behavior and investigate further.


## How it works

The agent (sensor) is the “data collector” on the endpoint. It gathers logs, processes, network activity, and system changes, then sends it back to the central EDR system for analysis.

## What data it collects

Telemetry is basically the “raw data” that the EDR collects.

Networks connections help in detecting C2 communications

C2 (Command & Control) traffic often looks like suspicious outbound connections to unusual IPs or domains. By monitoring network connections, EDR can spot this.

IOC = Indicator of Compromise (hash, IP, domain, filename, etc.)

EDR can flag threats by matching endpoint activity with a database of known IOCs.
This is similar to AV, but EDR adds extra context like process trees and network data.

