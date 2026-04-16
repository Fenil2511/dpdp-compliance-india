# Personal Data Breach Response Checklist
## Rule 7, DPDP Rules 2025 + Section 8(6), DPDP Act 2023

> **How to use**: When a potential personal data breach is detected, activate
> this checklist. Work through each phase in order. Document every action
> with timestamp for Board evidence trail.

---

## ⚡ PHASE 0 — IMMEDIATE TRIAGE (Hour 0–1)

| # | Action | Done | Time | Owner |
|---|--------|------|------|-------|
| 0.1 | Receive alert / report of potential incident | | | IRT |
| 0.2 | Log the incident: date, time, who reported, initial description | | | IRT Lead |
| 0.3 | Activate Incident Response Team (IRT) — assemble core team | | | CISO/DPO |
| 0.4 | Make preliminary determination: **Is this a personal data breach under DPDP?** | | | CISO/Legal |
| 0.5 | Check DPDP definition: Unauthorised processing / disclosure / acquisition / sharing / use / alteration / destruction / loss of access to personal data that compromises CIA | | | Legal |
| 0.6 | If YES or uncertain → activate full breach response protocol | | | IRT Lead |
| 0.7 | Brief CEO/MD and General Counsel immediately | | | CISO |

### ✅ Decision: Is this a DPDP Personal Data Breach?

| Scenario | DPDP Breach? |
|----------|-------------|
| Ransomware encrypts customer database | ✅ YES — loss of access = breach |
| Employee accidentally emails customer list externally | ✅ YES — accidental disclosure |
| Hacker exfiltrates customer records | ✅ YES — unauthorised acquisition |
| Internal staff misuses customer data | ✅ YES — unauthorised use |
| System downtime (no data compromised) | ❌ NO — no personal data compromised |
| Paper records lost (not digitised) | ❌ NO — DPDP covers digital personal data only |
| Test data with no real personal data | ❌ NO — not personal data |

---

## 🚨 PHASE 1 — CONTAINMENT (Hours 1–4)

| # | Action | Done | Time | Owner |
|---|--------|------|------|-------|
| 1.1 | **Isolate affected systems** — take offline if necessary to prevent further exposure | | | IT/CISO |
| 1.2 | **Preserve evidence** — do NOT delete logs, traces, or affected data | | | IT Forensics |
| 1.3 | **Identify the attack vector / root cause** (preliminary) | | | IT/CISO |
| 1.4 | **Determine scope**: What data? How many Data Principals? Which systems? | | | IT + DPO |
| 1.5 | **Stop ongoing breach** — change credentials, revoke tokens, block IP addresses | | | IT |
| 1.6 | **Document containment actions** with exact timestamps | | | IRT Lead |
| 1.7 | **Notify Data Processors** — if breach involves vendor/DP systems, notify them immediately and require their breach report | | | DPO/Legal |

---

## 📊 PHASE 2 — ASSESSMENT (Hours 2–6)

Complete this assessment before notifications:

| Assessment Item | Your Answer |
|----------------|-------------|
| **Nature of breach** | [Unauthorised access / disclosure / encryption / deletion / etc.] |
| **Systems/processes affected** | [List] |
| **Personal data categories compromised** | [Name / email / phone / financial / health / biometric / children's data] |
| **Approximate number of Data Principals affected** | [Number or range] |
| **Geographic spread** | [City / State / Pan-India / International] |
| **Does it involve children's data (under 18)?** | [Yes / No / Unknown] |
| **Does it involve sensitive data (health, financial, biometric)?** | [Yes / No] |
| **Is breach contained?** | [Yes / No / Partially] |
| **Root cause (preliminary)** | [Known / Under investigation] |
| **Estimated date breach began** | [Date/time or "unknown"] |
| **How was breach discovered?** | [Internal detection / external report / third party] |

---

## 📋 PHASE 3 — BOARD NOTIFICATION (As Soon as Reasonably Practicable)

> **Target: Complete within 6 hours of confirming breach** (aligns with RBI/SEBI for financial institutions)

| # | Action | Done | Time | Owner |
|---|--------|------|------|-------|
| 3.1 | **Draft Board notification** using Schedule 3 format | | | DPO/Legal |
| 3.2 | Obtain **DPO and CISO sign-off** on notification content | | | DPO + CISO |
| 3.3 | Obtain **MD/CEO approval** for notification | | | CEO |
| 3.4 | **Submit notification to Data Protection Board of India** via Digital Office portal | | | DPO |
| 3.5 | **Record confirmation** of submission (reference number, timestamp) | | | DPO |
| 3.6 | Designate **single point of contact** for all Board communications | | | DPO |

### Board Notification — Mandatory Content (Schedule 3, DPDP Rules 2025)

Ensure your notification includes:
- [ ] Organisation name, CIN, address, website
- [ ] Date and time breach discovered
- [ ] Date and time breach occurred (if known)
- [ ] **Nature of the breach** (unauthorised access / disclosure / etc.)
- [ ] **Categories of personal data** affected
- [ ] **Approximate number of Data Principals** affected
- [ ] **Likely consequences** of the breach
- [ ] **Measures taken** to address the breach
- [ ] **Measures proposed** for remediation
- [ ] Point of contact for Board communications (name + contact)

---

## 📱 PHASE 4 — DATA PRINCIPAL NOTIFICATION (As Soon as Reasonably Practicable)

> **Target: Send to affected Data Principals within 72 hours of confirming breach**

| # | Action | Done | Time | Owner |
|---|--------|------|------|-------|
| 4.1 | Identify **all affected Data Principals** from breach scope assessment | | | IT/DPO |
| 4.2 | Identify the **communication channel** normally used with each Data Principal | | | CRM/DPO |
| 4.3 | **Draft Data Principal notification** using Template B (Breach Notification Templates) | | | DPO/Comms |
| 4.4 | Ensure notification is in **English and/or relevant Eighth Schedule language** | | | DPO/Comms |
| 4.5 | DPO sign-off on notification content | | | DPO |
| 4.6 | **Send notifications** to all affected Data Principals via normal communication channel | | | IT/CRM |
| 4.7 | **Record delivery confirmation** (email delivery receipts / SMS delivery reports) | | | IT |
| 4.8 | For large-scale breaches: Consider **public notice** (website banner, press release) | | | Comms/Legal |
| 4.9 | **Set up dedicated helpline** / email for Data Principal queries | | | Customer Service |

### Data Principal Notification — Mandatory Content (Rule 7)

Ensure your notification includes:
- [ ] What personal data was compromised (be specific)
- [ ] What happened (in plain language — no jargon)
- [ ] What the organisation is doing
- [ ] What steps the Data Principal should take to protect themselves
- [ ] Contact for further queries

---

## 🔄 PHASE 5 — PARALLEL NOTIFICATIONS (Financial Institutions)

| Regulator | Trigger | Timeline | Form/Channel |
|-----------|---------|----------|-------------|
| **RBI** (if RBI-regulated) | Critical cyber incident | **6 hours** | CIRT-RBI portal |
| **SEBI** (if listed/market participant) | Major cyber incident | **6 hours** | SEBI SCORES portal |
| **CERT-In** | Any cyber incident meeting CERT-In Directions criteria | **6 hours** | incident@cert-in.org.in |
| **DPBI** | Personal data breach | **As soon as reasonably practicable** | DPBI Digital Office |
| **State Police / Cyber Crime** | If criminal offence (hacking, fraud) | Within 24 hours | Cybercrime portal |

---

## 🔍 PHASE 6 — INVESTIGATION AND REMEDIATION (Days 1–30)

| # | Action | Done | Date | Owner |
|---|--------|------|------|-------|
| 6.1 | Engage **external forensic investigator** (if needed) | | | CISO |
| 6.2 | Conduct **full root cause analysis** | | | IT/CISO |
| 6.3 | Document complete **timeline of events** | | | IRT |
| 6.4 | Identify all **security gaps** that enabled the breach | | | CISO |
| 6.5 | Develop **remediation plan** with specific actions and deadlines | | | CISO/DPO |
| 6.6 | Implement **immediate technical fixes** | | | IT |
| 6.7 | Review and update **Data Processor agreements** (if DP was involved) | | | Legal/DPO |
| 6.8 | **Update Board (DPBI)** with investigation findings (supplementary notification) | | | DPO |
| 6.9 | Conduct **affected employee/team debrief** | | | CISO/HR |
| 6.10 | Review and update **Incident Response Plan** based on lessons learned | | | CISO/DPO |

---

## 📝 PHASE 7 — EVIDENCE AND DOCUMENTATION (Ongoing from Day 1)

**Document and preserve the following for potential Board inquiry:**

| Document | Purpose |
|----------|---------|
| Incident log (timestamped) | Timeline of all actions taken |
| Technical forensic report | Evidence of breach scope and root cause |
| Board notification (sent copy + delivery receipt) | Proof of DPBI compliance |
| Data Principal notifications (sent copies + delivery reports) | Proof of Rule 7 compliance |
| Containment actions documentation | Mitigation evidence (penalty reduction) |
| Remediation plan and completion evidence | Mitigation evidence |
| Communication with Data Processors | Chain of accountability |
| Board (DPBI) correspondence | Regulatory cooperation evidence |
| All internal communications about breach | Corporate governance evidence |

> **Retention**: Keep all breach documentation for a minimum of **5 years**
> (aligned with limitation periods for DPBI proceedings).

---

## 📊 BREACH SEVERITY CLASSIFICATION

Use this to determine notification urgency:

| Severity | Criteria | Response Target |
|----------|---------|----------------|
| **Critical** | >1 lakh Data Principals; OR health/biometric/financial data; OR national security implications; OR children's data | Board notification: 4 hours; DP notification: 24 hours |
| **High** | 10,000–1 lakh Data Principals; OR sensitive categories; OR high financial fraud risk | Board notification: 6 hours; DP notification: 48 hours |
| **Medium** | 1,000–10,000 Data Principals; general personal data (name, email, phone) | Board notification: 12 hours; DP notification: 72 hours |
| **Low** | <1,000 Data Principals; low-sensitivity data; no material harm likely | Board notification: 24 hours; DP notification: 7 days |

---

## ⚠️ COMMON MISTAKES TO AVOID

| Mistake | Why It's Critical |
|---------|------------------|
| Delaying notification while "still investigating" | The obligation triggers on "becoming aware" — not when investigation is complete. Notify with best available info, update later |
| Notifying Data Principals before containment | May cause panic without protective benefit if breach is still active. Contain first, then notify |
| Assuming "masked data" means no breach | Masked card numbers + names + emails still = personal data breach |
| Notifying only regulatory bodies, not Data Principals | Both notifications are separate legal obligations; DP notification is mandatory |
| Using legal jargon in Data Principal notification | Must be in plain, simple language + relevant Indian language |
| Not involving Data Processors in response | If a DP was involved, they must report to you AND assist in your investigation |
| Destroying logs to "manage" the narrative | Obstruction of Board inquiry — dramatically worsens outcome |

---

*Document Version 1.0 | Based on DPDP Act 2023 Section 8(6) + DPDP Rules 2025 Rule 7*
*#DataBreach #BreachResponse #DPDPBreach #Rule7 #IncidentResponse #DPBI #DPDPCompliance #IndiaPrivacy*
