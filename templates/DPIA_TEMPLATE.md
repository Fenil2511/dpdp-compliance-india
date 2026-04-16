# Data Protection Impact Assessment (DPIA) Template
## Section 10(2)(c), DPDP Act 2023 + Rule 9, DPDP Rules 2025

> **Mandatory for**: Significant Data Fiduciaries (SDFs) — for every new or
> materially changed processing activity.
> **Best practice for**: All Data Fiduciaries processing sensitive or large-scale data.

---

## DPIA METADATA

| Field | Details |
|-------|---------|
| **DPIA Reference Number** | DPIA-[YEAR]-[SEQUENCE] |
| **Processing Activity Name** | [e.g., "Customer credit scoring using AI"] |
| **Business Unit / Product** | [Name] |
| **DPIA Lead** | [Name, Designation] |
| **DPO Review** | [DPO Name, Date] |
| **Business Owner Approval** | [Name, Date] |
| **Version** | [1.0] |
| **Date Initiated** | [DD/MM/YYYY] |
| **Date Completed** | [DD/MM/YYYY] |
| **Next Review Date** | [DD/MM/YYYY] |
| **Status** | [Draft / Under Review / Approved / Closed] |

---

## SECTION 1 — PROCESSING ACTIVITY DESCRIPTION

### 1.1 What Personal Data is Being Processed?

| # | Personal Data Type | Data Source | Format |
|---|-------------------|------------|--------|
| 1 | [e.g., Name, date of birth] | [e.g., Customer registration] | Digital |
| 2 | [e.g., Transaction history] | [e.g., Banking core system] | Digital |
| 3 | [Continue for each type] | | |

### 1.2 Who Are the Data Principals?

| Category | Approximate Number | Special Category? |
|----------|-------------------|------------------|
| [e.g., Individual loan applicants] | [e.g., 50,000/month] | [e.g., No] |
| [e.g., Minors (under 18)] | [Number] | YES — children's data |
| [e.g., Health condition disclosed] | [Number] | YES — health data |

### 1.3 What is the Purpose of Processing?

**Primary purpose**: [One clear sentence — e.g., "To assess creditworthiness of loan applicants using automated AI scoring to determine loan eligibility and interest rate."]

**Is the purpose clearly defined?** [ ] Yes [ ] No — if No, stop and define before proceeding

**Is the purpose specific?** [ ] Yes [ ] No — if No, the processing may not have valid consent/legal basis

### 1.4 What is the Legal Basis for Processing?

| Processing Activity | Legal Basis | DPDP Reference |
|--------------------|------------|----------------|
| [Activity 1] | [ ] Consent [ ] Sec 7(a) voluntary [ ] Sec 7(b) State function [ ] Sec 7(c) Legal obligation [ ] Sec 7(h) Employment | Sec 4 |
| [Activity 2] | [Select] | Sec 4 |

### 1.5 How Will Data Be Processed?

Describe the processing workflow:

```
[Step 1]: Data collected from [source] via [method]
[Step 2]: Data stored in [system] with [security controls]
[Step 3]: Data processed by [system/team] for [purpose]
[Step 4]: Output/decision: [describe]
[Step 5]: Data shared with [parties] if applicable
[Step 6]: Data retained for [period] then deleted via [method]
```

### 1.6 Who Processes the Data?

| Party | Role | Location | DPA in Place? |
|-------|------|----------|--------------|
| [Own team/system] | Data Fiduciary | India | N/A (internal) |
| [Vendor name] | Data Processor | [India/Country] | [ ] Yes [ ] No |
| [Other DF sharing with] | Data Fiduciary | [Country] | [ ] Yes [ ] No |

### 1.7 Where is Data Stored and Transferred?

| Storage Location | Country | Security Standard |
|----------------|---------|------------------|
| [Primary database] | India | [ISO 27001 / other] |
| [Backup location] | India | [Standard] |
| [Offshore location if any] | [Country] | [Standard — check against restriction list] |

---

## SECTION 2 — NECESSITY AND PROPORTIONALITY

### 2.1 Is the Processing Necessary?

| Question | Answer |
|----------|--------|
| Is the processing necessary to achieve the stated purpose? | [ ] Yes [ ] No |
| Could the purpose be achieved with less personal data? | [ ] Yes — describe how: | [ ] No |
| Could the purpose be achieved without personal data at all? | [ ] Yes | [ ] No |
| Is the processing proportionate to the purpose? | [ ] Yes [ ] No |

**Data minimisation check:**
- List every data element: Is each one strictly necessary for the purpose?
- Remove or do not collect elements that are not strictly necessary

| Data Element | Necessary? | If No — Action |
|-------------|-----------|----------------|
| [Element 1] | [ ] Yes [ ] No | [Remove / anonymise / aggregate] |
| [Element 2] | [ ] Yes [ ] No | |

### 2.2 Retention Period Assessment

| Data Type | Retention Period | Justification | Legal Basis for Retention |
|-----------|-----------------|---------------|--------------------------|
| [Type 1] | [Period] | [Why this long?] | [Purpose / Legal obligation] |

---

## SECTION 3 — RISK ASSESSMENT TO DATA PRINCIPALS' RIGHTS

### 3.1 Risk Identification

For each risk, assess likelihood (1–5) and impact (1–5). Risk Score = Likelihood × Impact.

| # | Risk | Likelihood (1–5) | Impact (1–5) | Risk Score | Risk Level |
|---|------|-----------------|-------------|------------|------------|
| R1 | Unauthorised access to personal data (external breach) | | | | |
| R2 | Unauthorised access by internal staff | | | | |
| R3 | Data shared with wrong third party | | | | |
| R4 | Data used beyond stated purpose | | | | |
| R5 | Inaccurate data leading to wrong decision affecting Data Principal | | | | |
| R6 | Data retained beyond necessary period | | | | |
| R7 | Data Principal unable to exercise rights (correction, erasure) | | | | |
| R8 | Children's data processed without parental consent (if applicable) | | | | |
| R9 | Cross-border transfer to restricted country | | | | |
| R10 | Algorithmic bias leading to discriminatory outcomes | | | | |
| R11 | [Add processing-specific risks] | | | | |

**Risk Level Key:**
- 1–4: Low | 5–9: Medium | 10–15: High | 16–25: Critical

### 3.2 Rights Impact Assessment

| Data Principal Right | Impact of this Processing Activity |
|---------------------|-----------------------------------|
| Right to information (Sec 11) | [ ] No impact [ ] Potential difficulty — describe: |
| Right to correction (Sec 12) | [ ] No impact [ ] Potential difficulty — describe: |
| Right to erasure (Sec 12) | [ ] No impact [ ] Conflict with legal retention — describe: |
| Right to grievance (Sec 13) | [ ] No impact [ ] Potential difficulty — describe: |
| Right to withdraw consent (Sec 6) | [ ] No impact [ ] Business impact of withdrawal — describe: |

---

## SECTION 4 — RISK MITIGATION MEASURES

For each identified risk (Risk Score ≥ 5), document mitigation:

| Risk Ref | Risk | Mitigation Measure | Control Type | Owner | Target Date | Residual Risk |
|----------|------|-------------------|-------------|-------|-------------|---------------|
| R1 | Unauthorised external access | Encryption + WAF + SIEM | Technical | CISO | [Date] | Low |
| R2 | Internal staff misuse | RBAC + PAM + audit logs | Technical + Process | CISO | [Date] | Low |
| R5 | Inaccurate data → wrong decision | Data quality controls + human review mechanism | Process | Business Owner | [Date] | Medium |
| R10 | Algorithmic bias | Regular bias testing + diverse training data | Technical + Process | Data Science | [Date] | Medium |
| [Rx] | [Risk] | [Measure] | | | | |

### 4.1 Residual Risk Acceptance

| # | Residual Risk | Residual Risk Level | Acceptance Decision | Approver |
|---|--------------|--------------------|--------------------|----------|
| 1 | [Risk after mitigation] | Low / Medium / High | [ ] Accepted [ ] Escalate [ ] Processing not approved | [DPO/Board] |

**If any residual risk is HIGH or CRITICAL**: Processing should NOT commence without Board approval and documented risk acceptance.

---

## SECTION 5 — CONSULTATION

### 5.1 Internal Stakeholders Consulted

| Stakeholder | Role | Date Consulted | Input Provided |
|-------------|------|---------------|----------------|
| DPO | Privacy oversight | | |
| Legal | Legal basis review | | |
| CISO | Security assessment | | |
| Business Owner | Purpose validation | | |
| IT Architecture | Technical feasibility | | |
| Compliance | Regulatory alignment | | |

### 5.2 External Consultation (Where Feasible)

| Party | Method | Date | Outcome |
|-------|--------|------|---------|
| Sample of Data Principals (focus group) | [Survey / Interview] | | |
| Industry body / Privacy association | [Consultation] | | |
| External legal counsel | [Opinion] | | |

---

## SECTION 6 — DPO REVIEW AND OPINION

**DPO Name**: ___________________
**Date of Review**: ___________________

**DPO Opinion**:
[ ] **Approve**: Processing can proceed as described. Mitigation measures are adequate.
[ ] **Approve with conditions**: Processing can proceed subject to the following conditions being met first: [List conditions]
[ ] **Reject**: Processing should not proceed. Reasons: [Explain]

**DPO Comments**:
[DPO writes their assessment here — independence of opinion must be maintained]

---

## SECTION 7 — FINAL APPROVAL

| Approver | Name | Signature | Date | Decision |
|----------|------|-----------|------|----------|
| Business Owner | | | | |
| DPO | | | | |
| CISO | | | | |
| Legal | | | | |
| **Management / Board** (for HIGH/CRITICAL residual risk) | | | | |

---

## SECTION 8 — IMPLEMENTATION AND MONITORING

### 8.1 Pre-Commencement Checklist

Before this processing activity commences:
- [ ] All HIGH and CRITICAL risks mitigated
- [ ] DPO approval obtained
- [ ] All consent notices updated to include this processing
- [ ] Data Processor agreements updated if new vendor involved
- [ ] Staff trained on new processing activity
- [ ] Technical security controls tested and verified
- [ ] Rights request mechanism updated to handle requests for this data

### 8.2 Ongoing Monitoring

| Monitoring Activity | Frequency | Owner |
|--------------------|-----------|-------|
| Security controls review | Quarterly | CISO |
| Data Principal rights compliance check | Monthly | DPO |
| Data retention adherence check | Quarterly | IT/DPO |
| Algorithm performance/bias review | Semi-annually | Data Science/DPO |
| DPIA review (material changes or annually) | Annual / on change | DPO |

---

## SECTION 9 — DPIA REGISTER ENTRY

Once completed, add this DPIA to the organisational DPIA Register:

| Field | Entry |
|-------|-------|
| DPIA Reference | |
| Processing Activity | |
| Date Approved | |
| DPO Approval Status | |
| Next Review Date | |
| High/Critical Risks Identified | [Yes/No — count] |
| Board Escalated | [Yes/No] |
| Status | [Active / Modified / Closed] |

---

*Template Version 1.0 | Based on DPDP Act 2023 Section 10(2)(c) + DPDP Rules 2025 Rule 9*
*#DPIA #DataProtectionImpactAssessment #DPDPSDF #SignificantDataFiduciary #PrivacyByDesign #DPDPCompliance #IndiaPrivacy*
