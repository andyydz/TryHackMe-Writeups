# SOC Fundamentals — TryHackMe Writeup



![Status](https://img.shields.io/badge/Status-Completed-success)
![Platform](https://img.shields.io/badge/Platform-TryHackMe-red)
![Difficulty](https://img.shields.io/badge/Difficulty-Easy-brightgreen)
![Category](https://img.shields.io/badge/Category-SOC%20%2F%20Blue%20Team-blue)



> 🔑 **Key Finding:** A SOC isn't just a SIEM dashboard — it's the combination of **People, Process, and Technology**, and every alert investigation comes down to answering five core questions: **Who, What, When, Where, Why**.

## Overview

This room introduces the foundational structure of a Security Operations Center (SOC) and walks through the core framework analysts use to triage and investigate alerts. It closes with a hands-on scenario simulating a real Tier 1 analyst workflow: investigating a port scan alert inside a SIEM using the 5W methodology.


## What I Actually Found

| Pillar | Component | Key Detail |
|---|---|---|
| People | SOC Team Roles | CISO, SOC Manager, Security Analyst (L1/L2/L3), Security Engineer, Detection Engineer — each with distinct responsibilities in the escalation chain |
| Process | Alert Triage (5W) | Who, What, When, Where, Why — the standard framework for structuring an investigation |
| Process | IR Lifecycle | Incident reporting, response, and forensics as the output of a triaged alert |
| Technology | SIEM | Security Information and Event Management — centralizes and correlates logs from network devices for detection |
| Technology | EDR | Endpoint Detection & Response — visibility and response at the host/endpoint level |
| Technology | Firewall | Perimeter control and traffic filtering, feeds log data into the SIEM |

## Hands-On Activities

### The Three Pillars of a SOC
Learned that SOC effectiveness rests on three interlocking pillars: **People** (analysts and their defined roles), **Process** (standardized workflows like alert triage and incident response), and **Technology** (SIEM, EDR, firewall — the tools that generate and centralize visibility). No single pillar functions well without the other two.

### People — SOC Team Structure
Covered the role hierarchy and responsibilities:
- **CISO** — overall security strategy and ownership
- **SOC Manager** — runs day-to-day SOC operations and team management
- **Security Analyst (L1/L2/L3)** — tiered escalation: L1 triages and filters alerts, L2 investigates deeper, L3 handles complex/advanced threats
- **Security Engineer** — builds and maintains the security infrastructure
- **Detection Engineer** — writes and tunes detection rules/use cases

### Process — The 5W Alert Triage Framework
Broke down the questions every analyst should answer when triaging an alert:
- **What** — what activity triggered the alert
- **When** — timestamp of the activity
- **Where** — source/destination involved
- **Who** — the host or user associated with the activity
- **Why** — whether the activity is malicious or benign/intended

This feeds directly into incident reporting, response, and forensic follow-up.

### Technology — SIEM, EDR, Firewall
- **SIEM** (Security Information and Event Management) — aggregates logs across the network for correlation and detection
- **EDR** (Endpoint Detection and Response) — endpoint-level visibility and containment
- **Firewall** — network perimeter filtering and an additional log source for the SIEM

### Practical Exercise: Port Scan Alert Investigation
Took on the role of a Tier 1 SOC Analyst investigating an alert for port scanning activity, using SIEM access to review raw logs and answer the 5W framework:

| Question | Finding |
|---|---|
| What | Port scanning activity detected |
| When | 12 June 2024, 17:24 |
| Where | Destination host IP — `[REDACTED]` |
| Who | Source hostname — `[REDACTED]` |
| Why | Assessed intent — malicious vs. intended/authorized |

Also reviewed whether any response was sent back to the scanning source, and concluded the investigation by documenting findings against the alert.

**Flag:** `[REDACTED]`

## SOC Analyst Relevance

| Skill Practiced | SOC Application |
|---|---|
| 5W Alert Triage | Core methodology used in every real-world SOC ticket/alert investigation |
| SOC Role Awareness | Understanding escalation paths (L1 → L2 → L3) for when/how to hand off an incident |
| SIEM Log Review | Foundational skill for reading and correlating raw logs to a single alert |
| People/Process/Technology Framework | Common interview talking point — shows understanding of SOC as an operational system, not just tooling |
| Port Scan Recognition | One of the most common Tier 1 alert types — recognizing scan patterns is a baseline skill |

## Key Takeaways

- A SOC runs on three pillars — People, Process, Technology — and weakness in any one undermines the others.
- The 5W framework is a transferable mental model I can apply to any alert, not just port scans.
- L1 analysts are triage-focused: the job is to answer the 5Ws quickly and accurately, then escalate or close.
- SIEM, EDR, and firewall logs all feed the same investigation — knowing what each contributes is foundational before going deeper into tools like Splunk.

---
📂 Part of my [TryHackMe Writeups series](https://github.com/andyydz/TryHackMe-Writeups)
