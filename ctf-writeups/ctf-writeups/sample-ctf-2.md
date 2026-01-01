# CTF Write-up: Suspicious Login & Privilege Escalation Analysis

## Overview

This write-up documents the investigation of a **CTF challenge focused on suspicious authentication activity and privilege escalation** on a Linux system.

The objective was to analyse provided logs, identify abnormal behaviour, and determine whether unauthorised access or misuse of privileges had occurred.

This challenge reflects **common SOC investigations involving compromised accounts**.

---

## Challenge Description

The challenge provided system and authentication logs from a Linux host.  
The task was to:

- Identify suspicious login activity
- Detect potential privilege escalation
- Determine whether the behaviour indicated compromise
- Explain findings clearly and logically

---

## Investigation Approach

The investigation followed a structured SOC-style workflow:

1. Review authentication activity  
2. Identify anomalies and failed login patterns  
3. Analyse privilege escalation events  
4. Correlate actions across logs  
5. Assess risk and conclude based on evidence  

---

## Tools Used

- Linux authentication logs (`auth.log`)
- Basic log filtering and analysis
- Understanding of Linux user and privilege management

---

## Analysis Process

### 1. Authentication Review
- Reviewed login attempts in the authentication logs
- Identified repeated failed login attempts for a single user
- Observed a successful login following multiple failures

This pattern raised suspicion of **brute-force or credential guessing activity**.

---

### 2. Source & Timing Analysis
- Login attempts occurred within a short time window
- Frequency suggested automation rather than human error
- Activity did not align with normal user behaviour patterns

---

### 3. Privilege Escalation Review
- Shortly after login, `sudo` commands were executed
- Commands accessed sensitive system areas
- Behaviour was inconsistent with standard user activity

---

### 4. Correlation
- Failed logins → successful login → privileged commands
- Sequence strongly indicated **unauthorised access followed by escalation**

---

## Findings

Based on log evidence:

- Authentication activity was abnormal
- Privilege escalation occurred soon after access
- Behaviour aligned with common post-compromise actions

The activity was assessed as **likely malicious**.

---

## Outcome

The challenge objective was completed by:

- Identifying suspicious login behaviour
- Detecting privilege escalation
- Explaining the attack sequence clearly
- Supporting conclusions with log evidence

---

## Lessons Learned

- Authentication logs are critical for early compromise detection
- Context and timing are essential when analysing login events
- Privilege escalation often follows credential compromise
- Log correlation is a key SOC analyst skill

---

## Analyst Reflection

This challenge reinforced the importance of:

- Reviewing login activity holistically
- Correlating events across multiple log sources
- Avoiding assumptions and relying on evidence
- Communicating findings clearly in incident documentation

These skills directly translate to **real-world SOC and incident response operations**.
