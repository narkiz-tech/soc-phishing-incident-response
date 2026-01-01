# Phishing Incident Response Case Study

*(IRONSCALES – Simulated Phishing Incident)*

## Incident Summary

This case study documents the analysis and response to a **simulated phishing incident** detected by **IRONSCALES** within an organisational email environment.

The incident was selected as a **representative example** from a broader threat protection environment and analysed to demonstrate **SOC-style investigation, decision-making, and response actions**.

The phishing email impersonated an internal IT-related message and attempted to harvest user credentials via a malicious link.

> ⚠️ **Note:**
> This analysis is based on a **training / simulation scenario**. All data has been anonymised and no real users or organisations are identified.

---

## Initial Detection

The phishing email was detected by **IRONSCALES automated threat detection**, which flagged the message as **phishing** based on behavioural and content indicators.

The incident was visible in the IRONSCALES dashboard, where it was categorised and prioritised for analyst review.

**Detection highlights:**

* Suspicious sender behaviour
* Social engineering language (urgency)
* Embedded malicious URL
* Campaign identified as phishing simulation

---

## Incident Scope & Impact

* **Incident Type:** Phishing (Credential Harvesting)
* **Attack Vector:** Email
* **Affected Users:** Test users (anonymised)
* **Credential Exposure:** Simulated
* **Business Impact:** High risk (credential compromise scenario)

Although the incident was simulated, the attack technique mirrors **real-world phishing activity** commonly used for initial access.

---

## Evidence Reviewed

The following evidence was reviewed during the investigation:

* Phishing email content (sanitised)
* Campaign metadata and timestamps
* User interaction metrics (open, click, submit)
* Analyst verdict and classification
* Incident activity timeline

All screenshots and supporting artefacts were anonymised prior to documentation.

---

## User Interaction Metrics

The campaign results indicated measurable user interaction:

* **Email Opened:** Yes
* **Malicious Link Clicked:** Yes
* **Credentials Submitted:** Yes (simulation)

These metrics demonstrate how phishing effectiveness is measured and how user behaviour contributes to organisational risk.

---

## Analyst Verdict

After review, the incident was classified as:

* **Verdict:** Phishing
* **Confidence:** High
* **Category:** Credential harvesting simulation

The classification aligned with the observed indicators and confirmed that the email posed a **credential compromise risk** if delivered in a real-world scenario.

---

## Incident Timeline (High-Level)

1. Phishing email delivered to test users
2. User opened the email
3. User clicked the embedded malicious link
4. Credentials submitted via fake login page
5. IRONSCALES detected and classified the incident
6. Analyst reviewed and confirmed phishing verdict

This timeline reflects a standard **SOC investigation flow**.

---

## Response Actions (Recommended)

Based on the incident analysis, the following response actions were recommended:

1. Immediate password reset for affected account(s)
2. Session invalidation
3. Enforcement or verification of MFA
4. User awareness follow-up and training
5. Continued monitoring for related suspicious activity

These actions align with standard **phishing incident response playbooks**.

---

## Lessons Learned

* Phishing remains an effective initial access technique
* User interaction metrics are critical for risk assessment
* Automated detection must be paired with analyst validation
* MFA significantly reduces the impact of credential theft
* Simulated phishing campaigns provide valuable defensive insight

---

## MITRE ATT&CK Mapping

| Technique ID | Technique Name |
| ------------ | -------------- |
| T1566        | Phishing       |
| T1078        | Valid Accounts |

---

## Conclusion

This case study demonstrates a realistic phishing incident analysed from a **defensive, SOC-oriented perspective**.

By reviewing detection indicators, user behaviour, and recommended response actions, this investigation highlights the importance of **early detection, accurate classification, and effective response** in mitigating phishing-related threats.

---

### Why this case study matters

This analysis reflects how **junior SOC analysts** contribute to phishing investigations by:

* Reviewing alerts
* Validating incidents
* Analysing evidence
* Supporting response decisions

It demonstrates practical, real-world security thinking beyond tool usage alone.


