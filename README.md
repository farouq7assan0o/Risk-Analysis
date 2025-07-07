# Risk Analysis and FAIR Modeling – DPSR Phishing Incident

## **Overview**

This project analyzes a phishing-based security incident at the **Department of Public Safety and Regulation (DPSR)** using the **FAIR (Factor Analysis of Information Risk)** model. It combines both qualitative and quantitative risk analysis methods, including **STRIDE/DREAD threat modeling**, **FAIR-U simulation**, and the application of Jordanian cybersecurity regulations.

## **Objectives**

- Identify and prioritize cyber risks using STRIDE and DREAD scoring
- Quantify the impact of a phishing attack using the FAIR methodology
- Model risk reduction through control implementation in FAIR-U
- Align the analysis with Jordan’s cybersecurity laws and frameworks

---

## **Incident Summary**

- **Attack Type:** Spear-phishing (email impersonation of a senior officer)
- **Duration:** Undetected for 6 days
- **Consequences:**
  - Exfiltration of sensitive documents (licensing and audits)
  - Spoofed emails sent with malware
  - Attempted internal privilege escalation

---

## **Threat Modeling (STRIDE + DREAD)**

Top Risks Identified:

| Threat                  | DREAD Score | Priority       |
|-------------------------|-------------|----------------|
| Information Disclosure  | 7.8         | Top Priority   |
| Elevation of Privilege  | 7.8         | Top Priority   |
| Spoofing                | 7.0         | High           |
| Tampering               | 5.8         | Medium         |
| Denial of Service       | 5.6         | Medium         |
| Repudiation             | 5.0         | Low            |

---

## **Quantitative FAIR Risk Model**

**Before Controls:**

- **Annualized Loss Expectancy (ALE):** $1.38M  
- **Top Drivers of Risk:**
  - Weak multi-factor authentication (MFA)
  - Legacy email systems
  - Delayed breach detection
  - High user susceptibility (~25% click rate)
  - Incomplete incident response readiness

**After Controls:**

- **New ALE:** $177K  
- **Estimated Risk Reduction:** ~$1.2M/year  
- **Controls Implemented:**
  - Mandatory MFA
  - Email system upgrade and SIEM
  - Executive phishing training
  - Real-time alerting and IR tabletop drills

---

## **FAIR Inputs & Assumptions**

- **Contact Frequency (CF):** 18 (avg) → 14 after controls
- **Probability of Action (PoA):** 25% (avg) → 12%
- **Resistance Strength (RS):** 50% → 65%
- **Loss Magnitude (LM):** $310K avg → $120K after controls
- **TEF, LEF, SLEF, PL modeled with Monte Carlo simulations**

---

## **Regulatory Alignment**

Aligned the risk findings with:

- **Jordanian Cybersecurity Law No. 16 (2019)**
- **Personal Data Protection Law No. 24 (2023)**
- **Jordan National Cybersecurity Framework (JNCSF)**

**Findings:**

- DPSR breached regulatory expectations by delaying breach disclosure by over 72 hours
- Failure to enforce MFA and implement real-time detection violated compliance requirements

---

## **Recommendations**

- **Enforce Mandatory MFA** for all staff
- **Upgrade email clients** and implement SIEM with real-time monitoring
- **Develop a formal IRP** and conduct tabletop incident simulations
- **Ensure breach disclosures** comply with PDPL timelines (within 72 hours)
- **Engage with NCSC** for threat coordination and reporting

---

## **Tools Used**

- FAIR-U (FAIR Institute Risk Modeling Tool)
- DREAD + STRIDE Risk Scoring Framework
- Microsoft Excel (Monte Carlo support)
- Risk Register and Executive Dashboards
- PowerPoint (DPSR Executive Summary Presentation)

---

## **Author**

**Farouq Hassan**  
Spring 2023–2024  
HTU – Risk Management & Governance  
Supervisor: Dr. Safaa Hriez
