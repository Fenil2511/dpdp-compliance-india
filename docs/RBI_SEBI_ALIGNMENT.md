# DPDP Act 2023 — RBI & SEBI Regulatory Alignment Guide
## For Banks, NBFCs, Payment Aggregators, Brokers & Financial Institutions

> **Purpose**: This document maps DPDP obligations against RBI and SEBI
> requirements, identifies conflicts, and provides practical resolution guidance
> for compliance teams in the Indian financial sector.

---

## OVERVIEW — WHY THIS MATTERS

Financial institutions operating in India face a **triple compliance burden**:

1. **DPDP Act 2023 + Rules 2025** — MeitY/DPBI jurisdiction
2. **RBI Master Directions** — Reserve Bank of India jurisdiction
3. **SEBI Frameworks** — SEBI jurisdiction (for listed entities, market participants)

These frameworks **overlap significantly** — but occasionally **conflict**.
This guide maps the overlaps, flags the conflicts, and tells you how to resolve them.

---

## PART 1 — MASTER ALIGNMENT TABLE

### Section A: Data Security & Cybersecurity

| DPDP Obligation | DPDP Reference | RBI Requirement | SEBI Requirement | Action |
|----------------|---------------|-----------------|------------------|--------|
| Implement security safeguards (encryption, access controls, monitoring, backup, incident response) | Sec 8(5) + Rule 6 | RBI IT Framework (2011); Master Direction – IT (2023); RBI Cyber Security Framework for Banks (2016) | SEBI CSCRF (2023) – Annex A security controls | **Implement once, satisfy all**: ISO 27001:2022 implementation satisfies RBI, SEBI, and DPDP security requirements simultaneously |
| Use "appropriate technology" that is technically sound and current | Rule 2(c) + Rule 6 | RBI mandates regular vulnerability assessments, patch management, technology refresh | SEBI mandates annual VAPT, technology audit | Annual VAPT + patch management = compliant with all three |
| Monitor and log access to personal data | Rule 6 | RBI: Security Operations Centre (SOC) for large banks; log management mandatory | SEBI: SOC requirement for Market Infrastructure Institutions | Unified SIEM/log management satisfies all |
| Implement backup and recovery procedures | Rule 6 | RBI: Business Continuity Planning (BCP) and Disaster Recovery (DR) mandatory | SEBI: Business Continuity Plan mandatory | DR/BCP plan covers DPDP backup requirements |

---

### Section B: Data Breach Notification

| DPDP Requirement | DPDP Timeline | RBI Requirement | SEBI Requirement | Practical Resolution |
|-----------------|--------------|-----------------|------------------|---------------------|
| Notify Data Protection Board | As soon as reasonably practicable | Notify RBI: Critical incidents within 6 hours; Major incidents within 24 hours | Notify SEBI: Major cyber incidents within 6 hours | **Parallel notifications** — trigger all notifications simultaneously on breach discovery. RBI/SEBI timelines are stricter → use those as your internal SLA (6 hours) |
| Notify affected Data Principals | As soon as reasonably practicable | Not explicitly required by RBI | Not explicitly required by SEBI | DPDP adds a new obligation RBI/SEBI don't require. Build DP notification into your IR plan as a 3rd parallel track |
| Notify CERT-In | Not in DPDP | CERT-In Directions 2022: Notify within 6 hours of discovering "certain incidents" | Same — CERT-In directions apply | 4-track notification: DPBI + RBI + SEBI + CERT-In. All within 6 hours target |

**Combined Breach Notification SLA (Financial Institutions):**
```
Hour 0:    Breach detected
Hour 1:    Incident confirmed; IRT activated
Hour 3:    Board/CEO briefed; notifications drafted
Hour 5:    RBI notification sent (critical incident)
Hour 5:    SEBI notification sent (if listed/market participant)
Hour 5:    CERT-In notification sent
Hour 6:    DPBI notification sent
Hours 6–72: Data Principal notifications sent (batch or immediate)
```

---

### Section C: Data Retention vs. DPDP Erasure Rights

**⚠️ KEY CONFLICT AREA — This is the most common conflict for financial institutions**

| Data Type | DPDP Requirement | RBI Retention Requirement | SEBI Retention Requirement | Resolution |
|-----------|-----------------|--------------------------|---------------------------|------------|
| KYC Documents | Erase when purpose served; erase on erasure request | Retain for **10 years** beyond account closure (KYC Master Direction) | Retain as per applicable law | **RBI prevails**: Retain for 10 years. Inform Data Principal of legal retention obligation when responding to erasure request |
| Transaction Records | Erase when purpose served | Retain for **10 years** (PMLA; Banking Regulation Act) | Retain for 5–8 years | **Statutory retention prevails**: Legal obligation to retain overrides DPDP erasure request. Communicate reason to DP |
| Loan Records / Credit History | Erase on request | Retain for **10 years** (or duration of limitation period) | N/A | Retain per RBI; inform DP |
| Employee Personal Data | Erase when employment ends + purpose | Retain per Labour Law / PF / ESIC requirements | N/A | Statutory HR retention prevails |
| Call Recordings (Customer Service) | Erase when purpose served | Retain for **180 days** minimum (RBI guidelines) | N/A | Follow RBI minimum; erase after 180 days unless needed |
| CCTV footage (Branch/ATM) | Erase when purpose served | Retain for **30 days** minimum | N/A | Follow RBI minimum |
| Insurance Policy Data | Erase on request | IRDAI: Retain for **7 years** after policy end | N/A | IRDAI retention prevails |

**How to handle an erasure request where legal retention applies:**

1. Receive erasure request from customer
2. Check if any statutory retention obligation applies (RBI/SEBI/PMLA/Companies Act)
3. If legal retention applies → **Cannot erase** that specific data
4. **Must inform the Data Principal**: "We are unable to erase [specific data] because we are required to retain it under [specific law/regulation] for [specific period]."
5. Erase any data that is NOT subject to legal retention
6. Document the decision and communication

> **Section 38 of DPDP Act**: "The provisions of this Act shall be in addition
> to and not in derogation of any other law for the time being in force." → Legal
> retention obligations under RBI, SEBI, PMLA, etc. continue to apply.

---

### Section D: Consent Management

| DPDP Requirement | DPDP Reference | RBI/SEBI Equivalent | Action |
|-----------------|---------------|---------------------|--------|
| Obtain free, specific, informed consent before processing personal data | Sec 6 | RBI: Customer consent required for sharing data with third parties (Account Aggregator framework) | Align DPDP consent framework with AA consent artefact standards |
| Consent notice must itemise data and purpose | Rule 3 | RBI KYC: Disclose data use to customer | Combine DPDP consent notice with KYC disclosure |
| Consent withdrawal as easy as giving | Sec 6(4) + Rule 4 | Not explicitly in RBI | New obligation for banks — build withdrawal mechanism into mobile app/net banking |
| Separate consents for separate purposes | Sec 6(1) | Not explicit in RBI | Banks must unbundle consents (e.g., core banking vs. marketing vs. third-party sharing) |

---

### Section E: Third-Party / Vendor Management (Data Processors)

| DPDP Requirement | DPDP Reference | RBI Requirement | Action |
|-----------------|---------------|-----------------|--------|
| Written DPA with all Data Processors | Sec 8 | RBI: Written agreements with all outsourcing vendors; Master Direction on Outsourcing | Same agreement can satisfy both — use DPDP DPA template + RBI outsourcing clauses in one agreement |
| DP must implement security safeguards | Rule 6 | RBI: Vendor must meet bank's security standards; right to audit | DPDP Rule 6 + RBI outsourcing security = same outcome |
| DP breach notification SLA to DF | Rule 7 | RBI: Vendor must report security incidents to bank | Unify: require vendors to notify within 4 hours (stricter than both) |
| Sub-processor restrictions | Sec 8 | RBI: Sub-contracting requires bank approval | Align — RBI approval required = DF written consent required |
| DF right to audit vendors | Sec 8 | RBI: Right to audit/inspect outsourcing vendors | Include DPDP + RBI audit rights in vendor contracts |

---

### Section F: Data Principal Rights vs. KYC/AML Requirements

| Scenario | DPDP Position | RBI/AML Position | Resolution |
|----------|--------------|------------------|------------|
| Customer requests erasure of KYC data | DPDP allows erasure | PMLA + KYC Master Direction requires 10-year retention | Retain. Inform customer. Section 17 and 38 of DPDP. |
| Customer requests correction of KYC data | DPDP requires correction | RBI also requires accurate KYC — aligned! | Correct the data. Both DPDP and RBI require this. |
| Customer requests details of who their data was shared with | DPDP Section 11 right | RBI restricts some disclosures (confidentiality obligations) | Provide information on data sharing to the extent not restricted by law. Flag restricted disclosures. |
| Customer requests data in portable format | DPDP Section 11 | Account Aggregator framework supports data portability | For financial data: integrate with AA consent artefact for portability |

---

## PART 2 — SECTOR-SPECIFIC GUIDANCE

### 2.1 Scheduled Commercial Banks & Urban Cooperative Banks

**Key DPDP additions over existing RBI compliance:**

1. **Consent notice upgrade**: Existing customer disclosure at account opening must be upgraded to meet Rule 3 notice standards (itemised data + purpose table)
2. **Consent withdrawal mechanism**: Banks must build a withdrawal mechanism (net banking / mobile app) — this is NEW; not currently required by RBI
3. **Children's accounts (under 18)**: If minors have accounts, parental consent for DPDP purposes needed for digital data processing
4. **Marketing consent**: Many banks use account opening consent for marketing too. This must now be a SEPARATE, OPT-IN consent under DPDP
5. **Third-party data sharing**: Sharing customer data with credit bureaus, insurance companies, AA aggregators — each needs mapped DPDP legal basis

**Practical tip**: Upgrade the account opening form / KYC form to be the DPDP consent notice. One document, dual purpose. Save operational cost.

---

### 2.2 NBFCs

**Same as Banks PLUS:**
- **Credit decisioning**: If using automated credit scoring algorithms → if NBFC becomes SDF, must implement algorithmic accountability
- **Co-lending / BC channels**: Business Correspondent and co-lending partners who access customer data = Data Processors → need DPAs
- **DSA/DST networks**: Loan agents with access to applicant personal data → Data Processors → need DPAs
- **Collection agencies**: Receiving debtor personal data → Data Processors → need DPAs with DPDP clauses

---

### 2.3 Payment Aggregators & Payment Gateways

**High-risk profile**: Large transaction volumes, financial data → likely SDF candidates.

Priority compliance items:
1. **Transaction data**: Each card/UPI transaction = processing of financial personal data. Consent basis = contractual necessity / legitimate use (payment processing)
2. **Merchant data**: Merchants sharing customer data with PA/PG = Data Fiduciary → Data Processor relationship. PA/PG needs DPA with every merchant
3. **Third-party sharing**: Sharing data with banks, NPCI, card networks = must be documented
4. **Tokenisation data**: If storing tokens → still "personal data" (identifiable via token). DPDP applies
5. **Cross-border**: International card transactions involving overseas processors → monitor restriction list

---

### 2.4 Stock Brokers & Depository Participants

**SEBI CSCRF + DPDP:**

1. **KYC/CKYC**: Align DPDP consent notice with SEBI KYC requirements
2. **Trading data**: Order data, portfolio data = personal data. Legitimate use ground (contractual) applies for core trading services
3. **Research recommendations**: Sending personalised research = may require consent (not covered by core service legitimate use)
4. **Sub-brokers / authorised persons**: Act as Data Processors → need DPAs
5. **Algo trading**: If using customer data for algo strategies → DPIA if SDF; document legal basis for all DFs

---

### 2.5 Mutual Fund Houses / AMCs

1. **Investor data**: NAV statements, redemption data, SIP data = personal financial data
2. **Distributor network**: MFDs/IFAs accessing investor data = Data Processors → need DPAs
3. **CAMS/KFintech**: RTAs accessing investor data = Data Processors → existing agreements need DPDP clauses
4. **Target-based advertising**: Marketing based on investor profile → needs separate consent
5. **Nominee data**: Nominee information = third-party personal data → use minimisation required

---

## PART 3 — UNIFIED COMPLIANCE PROGRAMME FOR FINANCIAL INSTITUTIONS

### The "One Compliance, Three Regulators" Approach

**Goal**: Build one compliance programme that simultaneously satisfies DPDP, RBI, and SEBI — avoiding duplication.

**Framework:**

```
LEVEL 1 — FOUNDATION (Satisfies all three)
├── Security: ISO 27001:2022 implementation
│   → Satisfies: DPDP Rule 6 + RBI IT Framework + SEBI CSCRF
├── Incident Response: Unified IR Plan with 4-track notification
│   → Satisfies: DPDP Rule 7 + RBI 6-hour reporting + SEBI reporting + CERT-In
├── Vendor Management: Single DPA template
│   → Satisfies: DPDP Sec 8 + RBI Outsourcing MD + SEBI Guidelines
└── Training: Annual privacy + cybersecurity training
    → Satisfies: DPDP best practice + RBI + SEBI requirements

LEVEL 2 — DPDP-SPECIFIC ADDITIONS
├── Consent Management: Rule 3 notice + withdrawal mechanism
├── Data Principal Rights: Information, Correction, Erasure, Grievance portal
├── Children's Data: Age verification + parental consent workflow
├── Consent Records: Maintain who consented, when, for what
└── Retention Map: Document what is retained per legal obligation (RBI/PMLA/SEBI)

LEVEL 3 — SDF-SPECIFIC (if notified)
├── DPO: Appoint India-based DPO; report to Board
├── Independent Auditor: Empanel qualified DPDP auditor
├── DPIA: Conduct for all high-risk processing
└── Algorithmic Accountability: Document and disclose automated decisions
```

---

## PART 4 — SAMPLE CONFLICT RESOLUTION MATRIX

| Conflict | DPDP Says | RBI/SEBI Says | Resolution | DPDP Section |
|----------|-----------|--------------|------------|-------------|
| Erase KYC data | Erase on request | Retain 10 years | Retain; inform DP | Sec 38 + Sec 17 |
| Marketing consent | Separate, opt-in | No specific rule | DPDP stricter; follow DPDP | Sec 6 |
| Breach notification timeline | ASAP | 6 hours | Follow 6 hours (stricter) | Rule 7 |
| Right to data portability | Right to information (Sec 11) | Account Aggregator framework | Use AA for portability | Sec 11 |
| Credit bureau data sharing | Needs consent/legitimate use | Mandated by RBI Credit Info Direction | Legitimate use (legal obligation) under Sec 7(c) | Sec 7(c) |
| Employee data processing | Consent or legitimate use | Employment law record-keeping | Legitimate use (employment - Sec 7(h)) | Sec 7(h) |
| Fraud investigation | Data Principal rights may be restricted | Banks mandated to investigate fraud | Section 17(1)(a) exemption applies | Sec 17(1)(a) |

---

*Document Version 1.0 | Based on DPDP Act 2023 + DPDP Rules 2025 + RBI Master Directions + SEBI CSCRF*
*#DPDPBanking #RBICompliance #SEBICompliance #FinancialSector #DPDPAct2023 #DataProtectionIndia #NBFC #FinTech #PaymentAggregator*
