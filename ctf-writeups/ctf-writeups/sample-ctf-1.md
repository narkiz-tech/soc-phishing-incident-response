# CTF Write-up: Suspicious Network Traffic Analysis

## Overview

This write-up documents the investigation of a **capture-the-flag (CTF) challenge** focused on identifying malicious activity within network traffic.  
The objective was to analyse provided artefacts, determine whether suspicious behaviour was present, and explain the findings clearly.

This exercise demonstrates **incident analysis, problem-solving, and analytical reasoning** rather than exploitation.

---

## Challenge Description

The challenge provided a network capture file containing normal and abnormal traffic.  
The task was to:

- Identify indicators of malicious activity
- Determine the nature of the suspicious behaviour
- Explain how the conclusion was reached
- Document the investigation process

---

## Investigation Approach

I approached the challenge using a structured incident response mindset:

1. Understand the scope of the artefact  
2. Identify unusual patterns or anomalies  
3. Validate findings using multiple indicators  
4. Draw conclusions based on evidence, not assumptions  

This mirrors how alerts are investigated in a SOC environment.

---

## Tools Used

- Wireshark  
- Basic TCP/IP and protocol analysis  
- Filtering and packet inspection techniques  

---

## Analysis Process

### 1. Initial Review
- Opened the capture file in Wireshark
- Reviewed overall traffic volume and protocol distribution
- Identified traffic types that appeared inconsistent with normal behaviour

### 2. Filtering & Inspection
- Applied protocol and IP-based filters
- Inspected suspicious packets for:
  - Unusual destination ports
  - Repeated connection attempts
  - Encoded or abnormal payloads

### 3. Pattern Identification
- Observed repeated communication to an external IP
- Traffic timing suggested automation rather than user activity
- Packet structure indicated potential command-and-control behaviour

---

## Findings

Based on the analysis:

- Traffic patterns were **not consistent with normal user behaviour**
- Repeated outbound connections suggested **malicious automation**
- The activity aligned with indicators commonly seen in malware callbacks or beaconing

The evidence supported the conclusion that the traffic was **suspicious and malicious in nature**.

---

## Outcome

The challenge objective was successfully completed by:

- Identifying the malicious traffic
- Explaining why it was suspicious
- Supporting conclusions with observable evidence

No exploitation was required; the focus was on **analysis and reasoning**.

---

## Lessons Learned

- Network traffic analysis is a critical detection skill in SOC roles
- Context and patterns matter more than single indicators
- Clear documentation is as important as technical findings
- Not all incidents require exploitation to reach valid conclusions

---

## Analyst Reflection

This challenge reinforced the importance of:
- Methodical investigation
- Avoiding assumptions
- Explaining findings clearly for non-technical stakeholders

These skills directly translate to real-world incident response and SOC operations.
