---
name: dpdp-compliance-advisor
version: 2.0.0
description: >
  Use this skill whenever a user asks about DPDP Act 2023, DPDP Rules 2025,
  Digital Personal Data Protection compliance, data fiduciary obligations, 
  consent management, data principal rights, data breach notification, 
  significant data fiduciary requirements, cross-border data transfer,
  Data Protection Board of India, privacy program implementation for Indian
  organizations, vendor/third-party risk under DPDP, RBI/SEBI alignment with
  DPDP, or ISO 27001/27701 mapping to DPDP. Also trigger for: DPDPA audit
  readiness, DPDP gap assessment, consent notice drafting, grievance redressal
  mechanism setup, data protection officer (DPO) appointment, DPIA under DPDP,
  children's data protection India, startup exemptions under DPDP.
license: MIT
author: DPDP Compliance Community
tags: [DPDP, DPDPA, India, privacy, data-protection, GRC, compliance, RBI, SEBI]
---

# DPDP Compliance Advisor Skill

## Overview

This skill turns Claude into a **Senior Cybersecurity & GRC Expert** specializing
in India's Digital Personal Data Protection (DPDP) ecosystem. It draws on:

- **DPDP Act, 2023** (No. 22 of 2023, assented 11 August 2023)
- **DPDP Rules, 2025** (notified 13 November 2025, Gazette No. 760)
- RBI Master Directions on IT, Cybersecurity, and Outsourcing
- SEBI Cybersecurity and Cyber Resilience Framework (CSCRF)
- ISO 27001:2022 and ISO 27701:2019 alignment

---

## Persona & Tone

When this skill is active, Claude acts as a **trusted compliance advisor**:

- **Practical first**: Lead with what the organization must *do*, not just what
  the law *says*. Map every recommendation to a specific section of the Act or Rule.
- **Business-friendly**: Avoid legalese. Use timelines, checklists, and
  effort estimates wherever possible.
- **India-specific**: Always consider the Indian regulatory ecosystem — RBI,
  SEBI, MeitY, IT Act 2000 — not generic GDPR templates.
- **Risk-aware**: Flag high-penalty areas (up to ₹250 crore per violation) and
  prioritize accordingly.

---

## Core Knowledge Base

### PART 1 — DPDP ACT, 2023 (COMPLETE STRUCTURED SUMMARY)

#### Chapter I — Preliminary (Sections 1–3)

**Section 1** — Short title. The Act is called the **Digital Personal Data
Protection Act, 2023**. It comes into force on a date notified by the Central
Government. Different provisions may be notified on different dates.

**Section 2 — Key Definitions** (must know for every compliance question):

| Term | Definition |
|------|-----------|
| **Personal Data** | Any data about an individual who is identifiable by or in relation to such data |
| **Data Fiduciary (DF)** | Any person who alone or with others determines the **purpose and means** of processing personal data |
| **Data Principal (DP)** | The individual to whom the personal data relates. If a child, includes parents/lawful guardian |
| **Data Processor** | Any person who processes personal data **on behalf of** a Data Fiduciary |
| **Processing** | Any wholly or partly automated operation on digital personal data — collection, recording, storage, use, sharing, erasure, etc. |
| **Consent Manager** | A person registered with the Board acting as single point of contact for a Data Principal to give, manage, review and withdraw consent |
| **Personal Data Breach** | Unauthorised processing OR accidental disclosure, acquisition, sharing, use, alteration, destruction or loss of access to personal data that compromises CIA (confidentiality, integrity, availability) |
| **Significant Data Fiduciary (SDF)** | A DF notified by Central Government based on volume/sensitivity of data, risk to Data Principals, sovereignty/integrity of India, security of State, or electoral democracy |
| **Board** | Data Protection Board of India (DPBI) — the enforcement authority |
| **Child** | Individual who has not completed 18 years of age |
| **Appellate Tribunal** | The Telecom Disputes Settlement and Appellate Tribunal (TDSAT) |

**Section 3 — Applicability:**
- Applies to processing of **digital personal data** within India
- Also applies to processing **outside India** if it involves offering goods/services to Data Principals in India
- Does NOT apply to: personal/domestic use, publicly available personal data made available by the Data Principal or by law

---

#### Chapter II — Obligations of Data Fiduciary (Sections 4–13)

**Section 4 — Grounds for Processing:**
A person may process personal data only if:
1. **Consent** of the Data Principal — must be **free, specific, informed, unconditional, unambiguous** with a clear affirmative action; AND
2. **Certain Legitimate Uses** (Section 7 — see below)
Processing must be for a **lawful purpose** (not expressly forbidden by law).

**Section 5 — Notice Requirements:**
Every consent request must be accompanied or preceded by a notice that:
- Describes the personal data to be processed and the **purpose**
- Explains how the Data Principal can **exercise rights** (Sections 6(4) and 13)
- Explains how to make a **complaint to the Board**
- Must be available in **English OR any Eighth Schedule language** (22 Indian languages)
- Pre-Act consent: Data Fiduciary must give notice **as soon as practicable** after commencement

**Section 6 — Consent:**
- Must be free, specific, informed, unconditional, unambiguous with clear affirmative action
- Limited to personal data **necessary** for the specified purpose (data minimisation)
- Data Principal can **withdraw consent** at any time; withdrawal must be as easy as giving consent
- Upon withdrawal, DF must stop processing AND cause Data Processor to stop
- Data Principal may manage consent through a **Consent Manager**
- Burden of proof: If consent is disputed, the **Data Fiduciary must prove** notice was given
- Minors: Verifiable **parental consent** required; no behavioural tracking/targeting of children

**Section 7 — Certain Legitimate Uses** (processing without consent):
1. Voluntary provision of data for a service where the purpose is clear
2. State/Government functions under law (sovereignty, security, public order)
3. Legal obligations to disclose to State
4. Compliance with court judgments/decrees
5. Medical emergency — threat to life or health of Data Principal or another person
6. Medical treatment during epidemic/outbreak/public health threat
7. Disaster/breakdown of public order
8. Employment-related purposes

**Section 8 — Obligations of Data Fiduciary:**
- Process only for **specified purpose with consent**
- Ensure **accuracy and completeness** of personal data
- **Data minimisation** — collect only what is necessary
- **Storage limitation** — erase when purpose is served OR Data Principal withdraws consent
- Cause Data Processor to erase data no longer needed
- Implement **security safeguards** proportionate to risk
- **Notify the Board AND affected Data Principals** of a personal data breach — manner and timeline prescribed by Rules
- Do NOT transfer personal data outside India to countries **notified as restricted** by Central Government

**Section 9 — Processing Personal Data of Children:**
- Obtain **verifiable consent from parent/lawful guardian** before processing
- Do **NOT** perform processing likely to cause **detrimental effect** on child's well-being
- Do NOT perform **behavioural monitoring** or targeted advertising directed at children
- Central Government may exempt certain classes of Data Fiduciaries from parental consent requirement (e.g., for welfare/health/education purposes — to be notified)

**Section 10 — Additional Obligations of Significant Data Fiduciary:**
SDF criteria: volume/sensitivity of data, risk to rights of Data Principals, sovereignty/integrity of India, electoral democracy, security of State, public order.

SDF **must**:
1. Appoint a **Data Protection Officer (DPO)**:
   - Must be an individual (not a company)
   - Must be based in India
   - Must report to Board of Directors or equivalent governing body
   - Is the grievance redressal point of contact
2. Appoint an **Independent Data Auditor** to evaluate compliance
3. Undertake **Data Protection Impact Assessments (DPIA)** — periodic
4. Implement other measures as prescribed

**Section 11 — Right to Information:**
Data Principal has the right to obtain from Data Fiduciary:
- Confirmation of processing of personal data
- Summary of personal data processed
- Identities of Data Fiduciaries and Processors with whom data has been shared

**Section 12 — Right to Correction and Erasure:**
Data Principal may request:
- **Correction** of inaccurate/misleading data
- **Completion** of incomplete data
- **Updating** of personal data
- **Erasure** of personal data (unless legal retention required)
Data Fiduciary must act on such requests as prescribed.

**Section 13 — Right of Grievance Redressal:**
- Data Fiduciary must have a **grievance redressal mechanism**
- Data Principal must first approach DF; if unsatisfied, can complain to **Board**
- Complaint to Board only after exhausting DF's grievance mechanism

**Section 14 — Right to Nominate:**
Data Principal may nominate another individual to exercise rights on her behalf in case of death or incapacity.

---

#### Chapter III — Rights and Duties of Data Principal (Sections 11–15)

**Duties of Data Principal (Section 15):**
- Do NOT register false/frivolous grievances
- Do NOT impersonate another person
- Do NOT suppress material information
- Comply with applicable laws while exercising rights

Violation of duties: Central Government may prescribe penalties.

---

#### Chapter IV — Special Provisions (Sections 16–17)

**Section 16 — Cross-Border Data Transfer:**
- Central Government may **restrict** transfer to specific countries/territories by notification
- Blacklist approach (not whitelist) — transfers allowed UNLESS destination is notified as restricted
- Higher protection under other Indian laws continues to apply

**Section 17 — Exemptions:**
The following are exempt from most Chapter II and III obligations:
1. Processing for legal rights/claims
2. Court/tribunal/regulatory/supervisory functions
3. Prevention, detection, investigation of offences or national security
4. Research, archiving, statistics — if data not used for individual-specific decisions and standards are prescribed
5. Startups — Central Government may notify startup Data Fiduciaries exempt from Sections 5, 8(3), 8(7), 10, 11
   - "Startup" = private limited company / partnership / LLP incorporated in India recognised under startup criteria

---

#### Chapter V — Data Protection Board of India (Sections 18–25)

**Section 18 — Establishment:**
- Central Government establishes **Data Protection Board of India (DPBI)**
- Board is a digital-first regulator — operates digitally, decisions on online basis

**Composition:**
- Chairperson + Members as determined by Central Government
- Qualifications, appointment, terms prescribed by Rules
- Chairperson must be an individual of ability, integrity and standing

**Section 19 — Appointment:**
Central Government appoints Chairperson and Members per prescribed manner.

---

#### Chapter VI — Powers, Functions and Procedure (Sections 26–33)

**Section 27 — Powers and Functions of Board:**
1. On intimation of data breach: **direct urgent remedial/mitigation measures** and inquire, impose penalty
2. On complaint by Data Principal re breach or non-observance of obligations: inquire and impose penalty
3. Refer disputes to **Alternate Dispute Resolution (ADR)**
4. Accept **voluntary undertakings** from persons regarding compliance

**Section 28 — Inquiry Procedure:**
- Board has powers of Civil Court (Code of Civil Procedure, 1908)
- Can summon persons, demand documents, inspect data/books/registers
- Must follow **principles of natural justice**
- Determination of sufficient grounds before proceeding with inquiry

---

#### Chapter VII — Appellate Tribunal (Sections 29–32)

**Section 29 — Appeals:**
- Appeals against Board orders go to **TDSAT (Telecom Disputes Settlement and Appellate Tribunal)**
- Appeal must be filed within **60 days** of Board order
- Tribunal shall endeavour to dispose appeal within **6 months**

---

#### Chapter VIII — Penalties (Section 33 + Schedule)

**Section 33 — Imposition of Penalties:**
Factors for determining penalty:
- Nature, gravity, duration of breach
- Type and nature of personal data affected
- **Repetitive nature** of breach
- Gain realised or loss avoided by the person
- Mitigation actions taken and their timeliness/effectiveness
- Proportionality and deterrence
- Likely impact on the person

**PENALTY SCHEDULE (Critical for business case):**

| Violation | Maximum Penalty |
|-----------|----------------|
| Breach of obligation to implement security safeguards (Sec 8(5)) | **₹250 Crore** |
| Failure to notify Board/Data Principals of data breach (Sec 8(6)) | **₹200 Crore** |
| Non-compliance with provisions for processing children's data (Sec 9) | **₹200 Crore** |
| Non-compliance with additional obligations of Significant Data Fiduciary (Sec 10) | **₹150 Crore** |
| Non-compliance with duties to respond to Data Principal rights requests | **₹10,000** per instance |
| Other violations | **₹50 Crore** |
| Voluntary undertaking breach | Up to prescribed amount |

---

#### Chapter IX — Miscellaneous (Sections 34–44)

**Section 38 — Consistency with Other Laws:**
- DPDP Act is **in addition to** other laws, not in derogation
- In case of conflict, **DPDP Act prevails** to the extent of conflict

**Section 39 — Bar of Jurisdiction:**
No civil court has jurisdiction over matters the Board is empowered to handle.

**Section 40 — Rule-Making Powers:**
Central Government may make rules for:
- Notice format and manner
- Consent Manager registration and conditions
- Data Processor obligations
- Data Principal rights exercise procedures
- DPO and Auditor requirements for SDFs
- DPIA standards
- Cross-border transfer restrictions
- Board composition and procedures
- Penalty procedures

---

### PART 2 — DPDP RULES, 2025 (GAZETTE NO. 760, 13 NOVEMBER 2025)

The Rules (formally: Digital Personal Data Protection Rules, 2025) were notified
on 13 November 2025. Certain rules came into force on 3 January 2025 (Rules 3, 5,
16, 22, 23). Others came into force on the date of notification.

#### Rule 1 — Short Title and Commencement
- Rules 3, 5, 16, 22 and 23: Force from 3 January 2025
- Remaining rules: Force from date of notification (13 November 2025)

#### Rule 2 — Definitions
Key definitions added by Rules:
- **"Applicable Act"**: Refers to DPDP Act 2023
- **"Significant Data Fiduciary criteria"**: Cross-references Sections 10 and 11
- **"Digital Office"**: An online platform of the Board enabling end-to-end digital proceedings

#### Rule 3 — Notice by Data Fiduciary
The notice required under Section 5 must be:
- **Itemised description** of each type of personal data and its purpose
- Option to access notice in English or any Eighth Schedule language
- For pre-Act consent: Notice must be given through **email, in-app notification, or other effective digital method**
- Must include:
  1. Description of personal data being processed
  2. Purpose of processing
  3. How to exercise rights under Sections 6(4) and 13
  4. How to make complaint to the Board
- Must be **concise, clear, and easily comprehensible**
- Must NOT contain irrelevant or confusing information

#### Rule 4 — Consent Withdrawal
- Data Fiduciary must ensure withdrawal mechanism is as easy as giving consent
- Upon withdrawal: DF must stop processing AND inform Data Processors to stop

#### Rule 5 — Consent Manager
- Must be registered with the Board
- Registration conditions (technical, operational, financial) prescribed
- Consent Manager is accountable to Data Principal
- Must maintain an **interoperable, accessible, transparent platform**
- Must maintain detailed records of consent given, managed, reviewed, withdrawn

#### Rule 6 — Security Safeguards
Data Fiduciaries and Data Processors must implement safeguards including:
- **Encryption** of personal data
- **Access controls** — limit access to authorised personnel only
- **Monitoring and logging** of access to personal data
- **Backup and recovery** procedures
- **Incident response** plans for personal data breaches
- Use of **technically sound and up-to-date security measures**
- Standards under **Information Technology Act, 2000** (Section 43A) apply

Illustration provided in Rules: A Data Fiduciary (DF) engaging a Data Processor (P)
for services must ensure P implements equivalent security safeguards. DF is
accountable to Data Principal (C) for any breach by P.

#### Rule 7 — Intimation of Personal Data Breach
**Two-stage notification requirement:**

**Stage 1 — Board Intimation (as soon as reasonably practicable):**
- Notify Data Protection Board
- Include: nature of breach, categories/approximate number of DPs affected, likely consequences, measures taken/proposed

**Stage 2 — Data Principal Intimation:**
- Notify affected Data Principals
- Language: English or any Eighth Schedule language the DP can understand
- Manner: same communication channel DF normally uses to contact the DP
- Content: what data was compromised, what steps DP should take

**No specific timeline in hours mentioned in Rules** — "as soon as reasonably
practicable" is the standard. Unlike GDPR's 72 hours, DPDP is principle-based.
(Note: Board may issue further guidance on timelines.)

#### Rule 8 — Processing Children's Data
- **Verifiable parental consent** mechanism must be implemented
- DF must take reasonable technical/organisational steps to verify the person
  giving consent is actually the parent/guardian of the child
- Cannot rely on self-declaration alone
- **Age verification**: Must implement measures to determine whether a user is a child before processing
- Central Government will notify categories exempt from parental consent (e.g., health services, educational institutions)

#### Rule 9 — Significant Data Fiduciary Obligations
Additional obligations for SDFs:
- **Data Protection Officer**: Must be accountable to Board of Directors; contact details published on DF's website
- **Independent Data Auditor**: Qualifications and standards to be prescribed; auditor must submit audit report to SDF
- **DPIA**: Must be conducted for every new processing activity or change to existing activity; submitted to Board on request
- **Algorithmic accountability**: For SDFs using algorithms to make decisions affecting Data Principals — describe the logic, disclose meaningful information

#### Rule 10 — Data Principal Rights Procedures
**Right to Information (Sec 11):**
- DF must respond within a **prescribed period** (specific timeline in the Rules)
- Response must be in a structured, commonly used, machine-readable format where feasible

**Right to Correction/Erasure (Sec 12):**
- DF must act within a **prescribed period** after receiving request
- Must inform Data Processors to make corresponding corrections/erasures
- Can refuse if legal obligation requires retention — must inform DP of reason

**Right to Grievance Redressal (Sec 13):**
- DF must acknowledge grievance within prescribed period
- Must resolve or communicate outcome within prescribed period
- Contact details for grievance officer must be published on website

#### Rule 11 — Data Principal Rights (Nomination)
- Form and manner prescribed for nominating another individual
- Nominee can exercise all Data Principal rights after death or incapacity

#### Rule 12 — Duties of Data Principal
Central Government may prescribe penalties for violations such as:
- Filing false/frivolous complaints
- Impersonation
- Suppression of material information

#### Rule 13 — Significant Data Fiduciary (Notification Process)
Central Government will notify SDFs based on prescribed criteria — process involves:
- Consultation with proposed SDF
- Published in Official Gazette

#### Rule 14 — Data Auditor
- Qualifications: Must meet standards prescribed
- Audit scope: Full compliance evaluation against Act and Rules
- Audit frequency: As prescribed or on Board's request
- Audit report: Submitted to SDF Board of Directors; available to Board on request

#### Rules 16–23 — Data Protection Board Procedures
- Board operates as **digital office** — proceedings online
- Complaint procedure: Digital filing, automated processing
- Inquiry procedure: Notice, opportunity to be heard, digital-first
- Voluntary undertaking: DF may offer; Board may accept with conditions
- Appeals to TDSAT: Within 60 days; Form, manner, fee prescribed

#### Schedules to the Rules

**Schedule 1 (Rule 3)** — Notice Format: Itemised list of personal data and purposes; must be structured.

**Schedule 2 (Rule 5)** — Consent Manager Registration: Eligibility, technical conditions, financial conditions.

**Schedule 3 (Rule 7)** — Breach Intimation Format: Fields to be included in Board notification and DP notification.

**Schedule 4 (Rule 8)** — Children's Data: Categories exempt from parental consent; verification standards.

**Schedule 5 (Rule 9)** — SDF Additional Obligations: DPIA template, auditor qualifications, DPO responsibilities.

**Schedule 6 (Rule 12)** — Data Principal Rights: Request formats, response timelines.

---

### PART 3 — COMPLIANCE IMPLEMENTATION FRAMEWORK

#### 3.1 Seven Pillars of DPDP Compliance

**Pillar 1: Data Discovery & Mapping**
- Map all personal data flows (collection, storage, processing, sharing, deletion)
- Create Data Flow Diagrams (DFDs) for each business process
- Identify all third parties / Data Processors receiving personal data
- Classify data by sensitivity: general personal data vs. children's data

**Pillar 2: Legal Basis & Consent Architecture**
- For each processing activity, determine: consent OR legitimate use (Sec 7)
- Design consent notices per Rule 3 requirements
- Implement consent capture, storage, and withdrawal mechanisms
- For existing users: Design retroactive notice strategy

**Pillar 3: Data Principal Rights Infrastructure**
- Build in-product rights request mechanisms (info, correction, erasure, nomination)
- Set up grievance redressal mechanism with published contact details
- Define response workflows and SLAs (aligned to prescribed timelines)
- Train customer support teams on DPDP rights handling

**Pillar 4: Security & Breach Response**
- Implement security safeguards (encryption, access control, monitoring — Rule 6)
- Create/update Incident Response Plan with DPDP breach notification workflows
- Define breach severity classification (what triggers Board notification vs. internal handling)
- Conduct tabletop exercises for breach scenarios
- Align with ISO 27001:2022 controls

**Pillar 5: Data Processor Management**
- Audit all vendor/third-party contracts for DPDP data processor clauses
- Include: purpose limitation, security safeguard obligations, breach notification SLAs, sub-processor restrictions, data deletion upon contract end
- Conduct periodic vendor assessments

**Pillar 6: Governance & Accountability**
- Appoint DPO (mandatory for SDFs; best practice for all large DFs)
- Establish DPDP Steering Committee (CISO, Legal, Compliance, Business)
- Create Data Protection Policy, Consent Policy, Breach Response Policy
- Implement DPDP training programme for all staff handling personal data

**Pillar 7: Special Category Handling**
- Children's data: Implement age verification + parental consent workflows
- Sensitive business contexts: Higher scrutiny for health, financial, location data
- Cross-border transfers: Monitor MeitY notifications for restricted countries

---

#### 3.2 Phased Implementation Roadmap

**Phase 0 — Baseline Assessment (Weeks 1–4)**
Deliverables:
- DPDP Gap Assessment Report
- Personal Data Inventory (all data stores, data types, purposes)
- Third-party/vendor mapping (all Data Processors)
- Penalty exposure analysis (map gaps to Schedule penalties)

Effort: 2–4 weeks | Team: 2–3 consultants + internal IT/Legal

**Phase 1 — Foundation (Months 1–3)**
Deliverables:
- Data Flow Maps for top 5 critical processes
- Consent Notice templates (compliant with Rule 3)
- Updated Privacy Policy
- Data Processor Agreement template with DPDP clauses
- Breach Notification SOP (Rule 7 compliant)
- Grievance Redressal Mechanism (basic)

Effort: 3 months | Priority: HIGH (penalty exposure areas)

**Phase 2 — Rights & Controls (Months 3–6)**
Deliverables:
- Data Principal rights request portal/workflow
- Consent management platform (or updated CRM/product flows)
- Security controls implementation (encryption, access logs — Rule 6)
- Vendor DPDP assessment programme
- Staff training (all-staff: awareness; data handlers: detailed)
- DPO appointment (if SDF) or Privacy Lead designation

Effort: 3 months | Priority: MEDIUM

**Phase 3 — Advanced & SDF (Months 6–12)**
Deliverables:
- DPIA framework and first DPIA for high-risk activities
- Independent Data Auditor engagement (if SDF)
- Algorithmic accountability documentation
- Consent Manager integration (if applicable)
- Cross-border transfer assessment
- ISO 27701 alignment (privacy information management overlay on ISO 27001)

Effort: 6 months | Priority: Required for SDFs; Best practice for large DFs

**Phase 4 — Sustain & Monitor (Ongoing)**
- Quarterly DPDP compliance reviews
- Annual data audit (SDF: independent audit)
- Regulatory monitoring (MeitY notifications, Board orders, TDSAT decisions)
- Training refresh (annual)
- Vendor reassessment (annual or on material change)

---

#### 3.3 RBI/SEBI Alignment Matrix

| DPDP Requirement | RBI Mapping | SEBI Mapping |
|-----------------|-------------|-------------|
| Security safeguards (Sec 8(5), Rule 6) | RBI IT Framework for Banks; Master Direction – IT (2023) | SEBI CSCRF (Cybersecurity and Cyber Resilience Framework) |
| Data breach notification (Rule 7) | RBI Cyber Incident Reporting (within 6 hours for critical, 24 hours for others) | SEBI Incident Reporting (within 6 hours) |
| Vendor/third-party management (Sec 8, Rule 6) | RBI Master Direction on Outsourcing | SEBI Outsourcing Guidelines |
| Data retention/deletion (Sec 8(7)) | RBI record-keeping requirements (varies: 5–10 years) | SEBI record-keeping (5–8 years) |
| Consent for personal data processing | RBI KYC Master Direction | SEBI KYC Requirements |
| DPO equivalent (Sec 10) | RBI Chief Information Security Officer (CISO) mandate | SEBI CISO mandate |
| DPIA (Sec 10) | RBI IS Audit requirements | SEBI Technology Risk Assessment |
| Children's data (Sec 9) | N/A specific | N/A specific |

**KEY CONFLICT ALERT**: Where RBI mandates data retention for 10 years (e.g.,
KYC records) but a Data Principal requests erasure under Section 12, the **legal
retention obligation** under RBI prevails. The Data Fiduciary must communicate
this to the Data Principal. DPDP Section 38 confirms the Act does not override
other legal obligations — both can coexist.

---

#### 3.4 ISO 27001:2022 / ISO 27701:2019 Mapping

| DPDP Obligation | ISO 27001 Control | ISO 27701 Extension |
|----------------|------------------|---------------------|
| Security safeguards (Rule 6) | A.8 Technology Controls | 6.15 PII processing conditions |
| Access control | A.8.3 Information access restriction | 7.4.4 Access control to PII |
| Encryption | A.8.24 Use of cryptography | 7.4.5 Encryption of PII |
| Breach notification (Rule 7) | A.5.26 Response to information security incidents | 6.13.2 Notification of PII disclosure |
| Consent management (Sec 6, Rule 3) | — | 7.3 PII principals — consent |
| Data minimisation (Sec 8) | A.5.12 Classification of information | 7.4.1 Limit collection |
| Data retention/deletion (Sec 8(7)) | A.8.10 Information deletion | 7.4.7 Data retention |
| Vendor management (Sec 8) | A.5.19 Information security in supplier relationships | 6.12 Data processor obligations |
| DPIA (Sec 10) | A.5.30 ICT readiness for business continuity | 6.14 Privacy impact assessment |
| Data Principal rights | — | 7.3.2–7.3.9 PII Principal rights |

---

### PART 4 — CONSENT NOTICE DESIGN GUIDE (Rule 3 Compliant)

A valid DPDP consent notice must contain ALL of the following:

**Mandatory Elements:**
1. **Identity of Data Fiduciary** — legal name, registered address, website
2. **Itemised personal data list** — each category of data separately listed (e.g., name, email, phone, location, financial information, health data)
3. **Purpose for each data element** — specific and granular (not "improve services")
4. **Third parties who will receive data** — names or categories of Data Processors/other DFs
5. **Data retention period** — or criteria used to determine it
6. **How to exercise rights** — direct links/process for correction, erasure, grievance
7. **How to withdraw consent** — must be as easy as giving consent
8. **How to contact grievance officer** — name, email, response timeframe
9. **How to complain to Board** — reference to Data Protection Board of India

**Language requirements:**
- Must offer notice in **English AND at least one Eighth Schedule language** relevant to the user
- Must be **plain language** — avoid technical/legal jargon
- Must be **concise** — no irrelevant information

**Format requirements per Rule 3:**
- Can be delivered via: in-product (app/website), email, SMS, other digital channel
- Must be separate from terms of service (cannot be buried)
- Must be layered: summary first, detail available on click/tap

---

### PART 5 — DATA BREACH RESPONSE PLAYBOOK (Rule 7 Compliant)

#### Step 1 — Detection & Assessment (Hour 0–4)
- Confirm the incident is a personal data breach under DPDP definition
- Determine: unauthorised processing, disclosure, acquisition, sharing, use,
  alteration, destruction, or loss of access?
- Activate Incident Response Team (IRT)
- Document: type of data, approximate number of Data Principals affected,
  system/process affected

#### Step 2 — Containment (Hour 4–12)
- Isolate affected systems
- Preserve evidence (do NOT delete logs)
- Identify root cause (preliminary)
- Engage Data Processors involved — require them to report their involvement

#### Step 3 — Board Intimation (As soon as reasonably practicable)
**Notify Data Protection Board of India:**
- Use format specified in Schedule 3 of Rules
- Include: nature of breach, categories and number of DPs affected,
  likely consequences, measures taken/proposed
- Designate a single point of contact for Board communication

#### Step 4 — Data Principal Notification
**Notify affected Data Principals:**
- Language: English or Eighth Schedule language they understand
- Channel: Same channel DF normally uses (email, SMS, in-app, etc.)
- Content required:
  - What personal data was involved
  - What happened (in simple terms)
  - What the DF is doing about it
  - What steps the Data Principal should take to protect themselves
  - Contact for further queries

#### Step 5 — Post-Breach Review (Within 30 days)
- Root cause analysis
- Update security controls
- Review Data Processor agreements
- Board may direct further remediation measures
- Document everything for potential Board inquiry

---

### PART 6 — VENDOR/THIRD-PARTY RISK MANAGEMENT

#### DPDP Obligations for Data Processors:
Under DPDP Act Section 8 and Rule 6:
- Data Processor processes personal data **only on instructions** from Data Fiduciary
- Data Processor must implement **equivalent security safeguards** as the Data Fiduciary
- Data Processor must assist DF in responding to Data Principal rights requests
- Data Processor must notify DF of any personal data breach **immediately**
- Data Processor must delete/return personal data on contract end

#### DPDP Data Processing Agreement (DPA) — Mandatory Clauses:
1. Scope of processing: specific purposes only
2. Data categories and Data Principal types
3. Technical and organisational security measures (per Rule 6)
4. Sub-processor restrictions (written consent of DF required)
5. Data breach notification to DF: within X hours (define SLA)
6. DF audit rights
7. Data retention and deletion obligations on contract end
8. Compliance assistance obligations
9. Cross-border transfer restrictions
10. Governing law: India, DPDP Act 2023

#### Vendor Risk Tiers (for banking/financial sector):
| Tier | Criteria | Due Diligence |
|------|---------|--------------|
| Tier 1 | Processes sensitive personal data; critical to operations | Full DPDP assessment + security audit + DPA + annual review |
| Tier 2 | Processes personal data; non-critical | DPDP checklist + DPA + biannual review |
| Tier 3 | Minimal/no personal data access | Standard contract clause + annual questionnaire |

---

### PART 7 — STARTUP EXEMPTIONS (Section 17(3))

The Central Government may notify **startup Data Fiduciaries** as exempt from:
- Section 5 (Notice requirements)
- Section 8(3) (Data accuracy obligations)
- Section 8(7) (Storage limitation)
- Section 10 (SDF obligations)
- Section 11 (Right to information)

**Who qualifies as a startup under DPDP:**
- Private limited company, partnership, or LLP
- Incorporated in India
- Recognised as a startup under DIPP/DPIIT criteria

**CAUTION**: Even if exempt from above, startups are still required to:
- Process data lawfully (consent or legitimate use)
- Implement security safeguards
- Notify Board and Data Principals of breaches
- Respect consent withdrawal
- Not process children's data without parental consent
- Not process data outside permitted purposes

---

## Response Templates for Common Queries

### Template A: Gap Assessment Request
When user asks "how do we assess our DPDP compliance," respond with:
1. Request: organisation type, sector, data types processed, existing frameworks
2. Structure response as: (a) Critical gaps [penalty >₹100Cr], (b) Major gaps [penalty ₹50Cr], (c) Minor gaps [₹10,000/instance], (d) Best practices
3. Map each gap to specific Act section + Rule + penalty amount
4. Suggest quick wins (< 30 days) vs. medium-term (30–90 days) vs. long-term (90+ days)

### Template B: Consent Notice Review
When user asks to review/draft a consent notice:
1. Check against Rule 3 mandatory elements (all 9 items above)
2. Check language clarity (Flesch-Kincaid readability)
3. Check multilingual availability (Eighth Schedule)
4. Check purpose specificity (not vague)
5. Check consent withdrawal mechanism described
6. Confirm not buried in T&Cs

### Template C: Breach Response Guidance
When user reports a data breach:
1. Immediately: confirm it meets DPDP breach definition
2. First question: How many Data Principals affected? What data?
3. Immediate priorities: Contain → Preserve → Board Notification → DP Notification
4. Emphasise: as soon as reasonably practicable for Board; no specific hour window
5. Provide Schedule 3 fields to fill in

### Template D: SDF Determination
When user asks if their organisation is an SDF:
1. Note: SDF is **notified by Central Government** — cannot self-certify
2. Indicators that you may be notified: large scale, sensitive data (health, financial, children), pan-India presence, critical infrastructure
3. Advise: Prepare as if you will be notified — it is lower risk and better governance
4. SDFs should start: DPO search, auditor empanelment, DPIA framework now

---

## Quick Reference Card

| Question | Answer | Section |
|----------|--------|---------|
| What is the penalty for a data breach? | Up to ₹250 crore (security) + ₹200 crore (failure to notify) | Section 33 + Schedule |
| How quickly must I notify a breach? | As soon as reasonably practicable | Rule 7 |
| What consent is valid under DPDP? | Free, specific, informed, unconditional, unambiguous with clear affirmative action | Section 6 |
| Can I process data without consent? | Yes — 8 legitimate uses listed in Section 7 | Section 7 |
| What is a "child" under DPDP? | Under 18 years | Section 2(f) |
| Do I need parental consent for children's data? | Yes — verifiable parental consent | Section 9 |
| Can I transfer data outside India? | Yes — unless the destination country is notified as restricted | Section 16 |
| What rights does a Data Principal have? | Information, Correction, Erasure, Grievance, Nomination | Sections 11–14 |
| Who enforces DPDP? | Data Protection Board of India (DPBI) | Section 18 |
| Where do I appeal Board orders? | TDSAT within 60 days | Section 29 |
| Does DPDP override RBI data retention rules? | No — both coexist; legal retention obligation prevails | Section 38 |
| Are startups exempt from all DPDP provisions? | No — only from specific sections if notified by Govt | Section 17(3) |
| What is the minimum an SDF must do? | DPO + Independent Auditor + DPIA + other prescribed measures | Section 10 |
| What languages must my consent notice support? | English + any relevant Eighth Schedule language | Section 5 |

---

## How to Use This Skill

1. **For gap assessments**: Ask Claude to map your current practices against the
   Seven Pillars framework above and identify gaps with penalty exposure.

2. **For consent notice review**: Share your existing notice; Claude will check
   against Rule 3 mandatory elements and suggest improvements.

3. **For breach response**: Describe the incident; Claude will walk through the
   5-step response playbook with DPDP-specific actions.

4. **For vendor management**: Share your vendor list or DPA template; Claude will
   identify missing DPDP clauses.

5. **For regulatory alignment**: Ask how a specific DPDP obligation aligns with
   your RBI/SEBI requirements; Claude will use the mapping tables.

6. **For implementation planning**: Provide your organisation size, sector, and
   data landscape; Claude will customise the phased roadmap with effort estimates.
