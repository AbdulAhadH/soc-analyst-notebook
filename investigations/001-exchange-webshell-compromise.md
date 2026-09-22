# Investigation 001 — Spike of Domain Discovery Commands 

**Date:** 2026-09-21
**Source:** TryHackMe SOC Dashboard — SOC L1 Alert Reporting 
**Status:** Escalated to L2

## Summary

A spike of AD domain discovery commands executed under `NT AUTHORITY\SYSTEM`. The process chain shows the `revshell.exe`, which points to the server being compromised rather than this being legitimate system activity. I escalated it as a true positive.

## Alert Details

| Field | Value |
|---|---|
| Alert Name | AD Domain Discovery Command Spike |
| Time Detected | [pull from dashboard] |
| Host Name | DMZ-MSEXCHANGE-2013 |
| Host OS | Windows Server 2012 R2 |
| User | NT AUTHORITY\SYSTEM |
| Source Process | C:\Windows\System32\cmd.exe |
| Parent Process | C:\Users\Public\revshell.exe |
| Grandparent Process | C:\Windows\System32\inetsrv\w3wp.exe |
| Invoked Commands | `dir`, `hostname`, `whoami /priv`, `net group "Domain Admins" /domain`, `nltest /dclist:tryhackme.thm` |

## Investigation

`NT AUTHORITY\SYSTEM` is the identity as by default, so seeing it here doesn't mean an admin did something.
Looks like a program .exe started in a shared public folder, cmd was opened and ran commands


**Classification:** True Positive
**Confidence:** High
**Escalated:** Yes

## What I Communicated


Who - NT AUTHORITY\SYSTEM |  Code/command execution with the server
What - commands whoami/priv, dir, hostname, net group "Domain Admins" 
When - March 27th 2025 | 19:56
Where- Host Name: DMZ-MSEXCHANGE-2013
Why - Compromising the server, domain discovery

## Questions / What I'd Ask a L2

- I believe this host should be isolated, but I don't know the real process for that
