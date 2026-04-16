# DPDP Act 2023 — ISO 27001:2022 & ISO 27701:2019 Mapping
## For Organisations Pursuing Integrated Compliance

> **Purpose**: If your organisation has ISO 27001 or is pursuing it, this mapping
> shows exactly which DPDP obligations are covered by ISO controls and which are
> NEW obligations requiring additional work.

---

## KEY INSIGHT UPFRONT

> **ISO 27001:2022 covers ~60% of DPDP security and governance requirements.**
> **ISO 27701:2019 covers ~80% of DPDP privacy-specific requirements.**
> **Together, ISO 27001 + ISO 27701 = ~85% of DPDP technical and governance obligations.**
>
> The remaining ~15% unique to DPDP = Consent management, Data Principal rights
> infrastructure, Children's data handling, and DPDP-specific governance (DPO, DPBI).

---

## PART 1 — ISO 27001:2022 CONTROL MAPPING TO DPDP

### Clause 5 — Organisational Controls

| ISO 27001:2022 Control | Control Description | DPDP Obligation Covered | DPDP Reference |
|----------------------|--------------------|-----------------------|---------------|
| A.5.1 | Policies for information security | Data Protection Policy, Consent Policy, Breach Response Policy | Sec 8 + Rule 6 |
| A.5.2 | Information security roles and responsibilities | DPO appointment, privacy responsibilities | Sec 10(2)(a) |
| A.5.9 | Inventory of information and other associated assets | Personal data inventory / data mapping | Sec 8 |
| A.5.10 | Acceptable use of information | Acceptable use of personal data; purpose limitation | Sec 6(1) + Sec 8 |
| A.5.12 | Classification of information | Personal data classification (general vs. sensitive vs. children's) | Sec 8 |
| A.5.13 | Labelling of information | Labelling personal data records for retention/deletion | Sec 8(7) |
| A.5.14 | Information transfer | Personal data transfer restrictions; cross-border transfer | Sec 16 |
| A.5.15 | Access control | Access limited to authorised personnel only | Rule 6 |
| A.5.19 | Information security in supplier relationships | Data Processor agreements; vendor security obligations | Sec 8 + Rule 6 |
| A.5.20 | Addressing information security within supplier agreements | DPA clause requirements for Data Processors | Sec 8 |
| A.5.22 | Monitoring, review and change management of supplier services | Vendor DPDP assessments; ongoing monitoring | Sec 8 |
| A.5.24 | Information security incident management planning and preparation | Breach response plan; IR team | Sec 8(6) + Rule 7 |
| A.5.25 | Assessment and decision on information security events | Determining if event = personal data breach under DPDP | Sec 2 + Rule 7 |
| A.5.26 | Response to information security incidents | Breach containment, remediation | Rule 7 |
| A.5.27 | Learning from information security incidents | Post-breach review; prevent recurrence | Sec 8(5) |
| A.5.28 | Collection of evidence | Preserving evidence for Board inquiry | Sec 28 |
| A.5.30 | ICT readiness for business continuity | Business continuity for personal data systems | Sec 8(5) |
| A.5.35 | Independent review of information security | Independent Data Audit for SDFs | Sec 10(2)(b) |
| A.5.36 | Compliance with policies, rules and standards | DPDP compliance monitoring | Sec 8 |

---

### Clause 6 — People Controls

| ISO 27001:2022 Control | Control Description | DPDP Obligation Covered | DPDP Reference |
|----------------------|--------------------|-----------------------|---------------|
| A.6.1 | Screening | Background checks for staff with access to sensitive personal data | Sec 8(5) |
| A.6.2 | Terms and conditions of employment | Staff obligations re personal data; confidentiality | Sec 8 |
| A.6.3 | Information security awareness, education, and training | DPDP training for all staff handling personal data | Sec 8 |
| A.6.5 | Responsibilities after termination or change of employment | Revoking access; data deletion obligations post-employment | Sec 8(5) + Rule 6 |
| A.6.8 | Information security event reporting | Internal reporting of potential personal data breaches | Rule 7 |

---

### Clause 7 — Physical Controls

| ISO 27001:2022 Control | Control Description | DPDP Obligation Covered | DPDP Reference |
|----------------------|--------------------|-----------------------|---------------|
| A.7.1 | Physical security perimeters | Physical security of personal data storage | Rule 6 |
| A.7.4 | Physical security monitoring | CCTV, access logs for areas with personal data | Rule 6 |
| A.7.8 | Equipment siting and protection | Securing hardware processing personal data | Rule 6 |
| A.7.10 | Storage media | Secure storage and disposal of media containing personal data | Rule 6 + Sec 8(7) |
| A.7.14 | Secure disposal or re-use of equipment | Secure erasure of personal data before equipment disposal | Sec 8(7) |

---

### Clause 8 — Technology Controls

| ISO 27001:2022 Control | Control Description | DPDP Obligation Covered | DPDP Reference |
|----------------------|--------------------|-----------------------|---------------|
| A.8.2 | Privileged access rights | Limit privileged access to personal data stores | Rule 6 |
| A.8.3 | Information access restriction | Role-based access to personal data | Rule 6 |
| A.8.4 | Access to source code | Control access to systems processing personal data | Rule 6 |
| A.8.5 | Secure authentication | Strong authentication for systems with personal data | Rule 6 |
| A.8.7 | Protection against malware | Malware protection for personal data systems | Rule 6 |
| A.8.8 | Management of technical vulnerabilities | Patching and vulnerability management | Rule 6 |
| A.8.10 | Information deletion | Data deletion when purpose served; erasure on request | Sec 8(7) + Sec 12 |
| A.8.11 | Data masking | Masking of personal data in non-production environments | Rule 6 |
| A.8.12 | Data leakage prevention | DLP controls to prevent unauthorised disclosure | Rule 6 + Sec 8(5) |
| A.8.15 | Logging | Audit logs for access to personal data | Rule 6 |
| A.8.16 | Monitoring activities | Monitoring for unauthorised access / processing | Rule 6 |
| A.8.17 | Clock synchronisation | Accurate timestamps for audit logs and breach timelines | Rule 7 |
| A.8.24 | Use of cryptography | Encryption of personal data at rest and in transit | Rule 6 |
| A.8.25 | Secure development lifecycle | Privacy-by-design; security in personal data systems development | Sec 8(5) |
| A.8.32 | Change management | Impact assessment for changes to personal data systems | Sec 10 (DPIA for SDFs) |
| A.8.33 | Test information | No real personal data in test environments (or controlled use) | Rule 6 + Sec 8 |

---

## PART 2 — ISO 27701:2019 MAPPING TO DPDP

> ISO 27701 is the privacy extension to ISO 27001. Its controls map most directly
> to DPDP obligations. This is the most efficient path to DPDP compliance for
> ISO 27001-certified organisations.

### Clause 6 — PIMS-Specific Requirements for PII Controllers (= Data Fiduciaries)

| ISO 27701 Clause | Description | DPDP Obligation | DPDP Reference |
|-----------------|-------------|----------------|---------------|
| 6.2.1 | Understanding the organisation and its context (privacy) | Personal data inventory; stakeholder mapping | Sec 8 |
| 6.3.1 | Privacy roles and responsibilities | DPO appointment; privacy governance | Sec 10(2)(a) |
| 6.4.1 | Limit collection | Data minimisation | Sec 6(1) + Sec 8(4) |
| 6.4.2 | Limit processing | Purpose limitation; process only for stated purpose | Sec 6(1) + Sec 8 |
| 6.4.3 | Accuracy and quality of PII | Data accuracy and completeness obligations | Sec 8(3) |
| 6.4.4 | PII minimisation objectives | Data minimisation policy | Sec 8(4) |
| 6.4.5 | De-identification and deletion at end of processing | Data deletion when purpose served | Sec 8(7) |
| 6.5.1 | Identify legal basis | Document legal basis (consent or Sec 7) for every processing activity | Sec 4 |
| 6.5.2 | Identify purpose | Document specific purpose for each data type | Sec 5 + Rule 3 |
| 6.5.3 | Determine when and how consent is to be obtained | Consent design; notice design | Sec 5 + Sec 6 + Rule 3 |
| 6.6.1 | Obligations to PII principals | Data Principal rights infrastructure | Secs 11–14 |
| 6.6.2 | Determining information for PII principals | Notice content requirements | Sec 5 + Rule 3 |
| 6.7.1 | Obligations to provide information | Proactive disclosure to Data Principals | Sec 5 |
| 6.8 | PII Principals who are minors | Children's data processing requirements | Sec 9 + Rule 8 |
| 6.9.1 | Responding to PII principals' requests | Rights request handling | Secs 11–14 + Rule 10 |
| 6.9.2 | Communicating to PII principals | Communication of privacy notices | Rule 3 |
| 6.10 | Automated decision-making | Algorithmic accountability | Sec 10 (SDF) |
| 6.11 | Direct marketing | Consent for marketing communications | Sec 6 |
| 6.12 | Third party agreements (processors) | Data Processor agreements; DPA requirements | Sec 8 + Rule 6 |
| 6.13.1 | PII sharing | Documenting data sharing with third parties | Secs 5, 11 |
| 6.13.2 | Notification of PII disclosure | Breach notification to Data Principals | Sec 8(6) + Rule 7 |
| 6.14 | Privacy Impact Assessment | DPIA (mandatory for SDFs; best practice for all) | Sec 10(2)(c) |
| 6.15 | PII processing conditions | Overall lawfulness of processing | Sec 4 |

---

### Clause 7 — PIMS-Specific Requirements for PII Processors (= Data Processors)

| ISO 27701 Clause | Description | DPDP Obligation | DPDP Reference |
|-----------------|-------------|----------------|---------------|
| 7.2.1 | Customer agreement | Written DPA with Data Fiduciary | Sec 8 |
| 7.2.2 | Organisation's purpose of PII processing | Process only on DF instructions | Sec 8 |
| 7.3.1 | Obligations to PII principals | Assist DF in responding to DP rights requests | Secs 11–14 |
| 7.4.1 | Limit collection | Data minimisation — collect only what DF instructs | Sec 8(4) |
| 7.4.4 | Access control to PII | Restrict access to authorised DP personnel | Rule 6 |
| 7.4.5 | Encryption of PII | Encrypt personal data at rest and in transit | Rule 6 |
| 7.4.6 | Temporary files | Secure handling and deletion of temp personal data | Sec 8(7) |
| 7.4.7 | Data retention | Delete personal data per DF instructions; on contract end | Sec 8(7) |
| 7.5 | Onward transfers of PII | Sub-processor restrictions; DF approval required | Sec 8 |
| 7.6 | Audit and compliance | Demonstrate compliance to DF; support DF audit rights | Sec 8 |

---

## PART 3 — GAP ANALYSIS: WHAT ISO 27001 + 27701 DOESN'T COVER

Even with full ISO 27001:2022 + ISO 27701:2019 certification, these DPDP-specific
obligations require additional work:

### 🔴 NEW — Not covered by ISO 27001 or 27701

| # | Gap | DPDP Reference | Action Required |
|---|-----|---------------|----------------|
| 1 | **Consent notice in Eighth Schedule language** (22 Indian languages) | Sec 5 + Rule 3 | Translate consent notices into relevant Indian languages |
| 2 | **Consent withdrawal as easy as consent giving** (specific UI/UX requirement) | Sec 6(4) + Rule 4 | Product/UI change to implement easy withdrawal |
| 3 | **Consent Manager integration** (if applicable) | Sec 6(7)–(9) + Rule 5 | Register with/integrate with Consent Manager if using one |
| 4 | **Verifiable parental consent for children** (under 18) | Sec 9 + Rule 8 | Implement age verification + parental verification |
| 5 | **Board notification format** (Schedule 3 of Rules) | Rule 7 | Update IR plan with Board-specific notification format |
| 6 | **Data Principal notification format** (Rule 7 language requirements) | Rule 7 | Add DP notification template in multiple languages to IR plan |
| 7 | **Right to nominate** (Indian-specific right) | Sec 14 + Rule 11 | Implement nomination form and process |
| 8 | **Complaint to Board** — include in all notices and consent forms | Sec 5 + Rule 3 | Add Board complaint reference to all notices |
| 9 | **Cross-border transfer — India blacklist monitoring** | Sec 16 | Create monitoring process for MeitY notifications |
| 10 | **Data Principal duty violations** — internal controls | Sec 15 | Build anti-fraud/impersonation checks into rights request process |

---

## PART 4 — IMPLEMENTATION PATHWAY FOR ISO 27001-CERTIFIED ORGANISATIONS

### If you have ISO 27001:2022 certification:

**Time to achieve DPDP compliance: 3–6 months** (significantly faster than non-certified orgs)

**Phase 1 (Month 1–2): Leverage existing controls**
- Map your existing ISO 27001 Statement of Applicability (SoA) to DPDP obligations
- Identify gaps (use the table above)
- Update your ISMS scope to include "DPDP Act 2023 compliance"

**Phase 2 (Month 2–4): Close DPDP-specific gaps**
- Implement consent notice upgrades (Rule 3)
- Build consent withdrawal mechanism
- Implement Data Principal rights portal
- Update IR plan for Board + DP notification
- Add DPDP clauses to vendor contracts (DPAs)

**Phase 3 (Month 4–6): Governance and SDF prep**
- Appoint DPO (or designate from existing CISO/DPO function if SDF)
- Conduct DPIA for highest-risk processing activities
- Update Privacy Policy and Grievance mechanism
- Children's data: age verification if applicable

---

### If you have ISO 27001:2022 + ISO 27701:2019:

**Time to achieve DPDP compliance: 2–4 months**

ISO 27701 certification means most privacy controls are already in place.
Key additions:
- Indian-language notice availability
- Board notification format
- Consent withdrawal ease-of-use
- Data Principal nomination right
- Children's data — Indian standard parental verification

---

### If you DON'T have ISO certification:

**Recommended path**: Pursue ISO 27001:2022 + ISO 27701:2019 simultaneously with DPDP compliance.

**Benefits**:
- One integrated programme satisfies DPDP + RBI + SEBI
- ISO certification → market differentiator for bank/financial sector onboarding
- ISO 27001 → reduces cyber insurance premiums
- ISO 27701 → demonstrates privacy commitment to customers

**Time to achieve ISO 27001 + DPDP compliance**: 9–18 months (depending on starting maturity)

---

## PART 5 — QUICK REFERENCE: DPDP OBLIGATION → ISO CONTROL

| DPDP Obligation | ISO 27001 Control | ISO 27701 Clause |
|----------------|-------------------|-----------------|
| Security safeguards | A.8.3, A.8.24, A.8.15, A.8.16 | 7.4.4, 7.4.5 |
| Data minimisation | A.5.12 | 6.4.1, 6.4.4 |
| Purpose limitation | A.5.10 | 6.4.2, 6.5.2 |
| Consent management | — | 6.5.3 |
| Consent notice | — | 6.6.2, 6.7.1 |
| Data accuracy | — | 6.4.3 |
| Storage limitation / deletion | A.8.10 | 6.4.5, 7.4.7 |
| Breach notification | A.5.26, A.5.27 | 6.13.2 |
| Vendor / DP management | A.5.19, A.5.20 | 6.12, 7.2.1 |
| DPIA | A.5.30 | 6.14 |
| DPO | A.5.2 | 6.3.1 |
| Data Principal rights | — | 6.6.1, 6.9.1 |
| Children's data | — | 6.8 |
| Cross-border transfer | A.5.14 | 7.5 |
| Algorithmic accountability | — | 6.10 |
| Audit | A.5.35 | 7.6 |
| Training | A.6.3 | — |

---

*Document Version 1.0 | Based on DPDP Act 2023 + DPDP Rules 2025 + ISO 27001:2022 + ISO 27701:2019*
*#ISO27001 #ISO27701 #DPDPCompliance #PrivacyManagement #ISMS #PIMS #IndiaPrivacy #GRC #DataProtection*
