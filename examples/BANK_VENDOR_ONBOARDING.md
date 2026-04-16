# Example: Bank Vendor DPDP Assessment & Onboarding
## How Banks Should Assess Vendors Under DPDP Act 2023

> **Scenario**: IndNational Bank (a large private sector bank with 3 crore
> customers) is onboarding CloudDocs Pvt. Ltd., a SaaS company that will
> provide document management services for KYC documents of 50 lakh customers.
> The bank's TPRM team must assess CloudDocs for DPDP compliance.

---

## CONTEXT: WHY BANKS MUST ASSESS VENDORS FOR DPDP

Under DPDP Act Section 8, the **Data Fiduciary (Bank)** remains accountable
to Data Principals for the actions of its Data Processors (vendors).

A bank cannot outsource its DPDP liability. If CloudDocs has a breach →
the **Bank is liable** to the Board for:
- Security safeguard failure (up to ₹250 Crore)
- Breach notification failure (up to ₹200 Crore)

The bank's existing **RBI Master Direction on Outsourcing** obligations also
require vendor due diligence. DPDP compliance assessment should be integrated
into the bank's existing Third-Party Risk Management (TPRM) framework.

---

## PHASE 1 — VENDOR RISK CLASSIFICATION

IndNational Bank classifies CloudDocs:

| Classification Criterion | Assessment |
|-------------------------|-----------|
| **Personal data access** | Yes — direct access to KYC documents containing PAN, Aadhaar, address, photos of 50 lakh customers |
| **Data sensitivity** | HIGH — KYC documents are sensitive financial personal data |
| **Criticality to operations** | HIGH — KYC is core regulatory function |
| **Contract duration** | 3 years |
| **Cross-border** | CloudDocs' backup data center is in Singapore |

**Verdict**: **Tier 1 Critical Vendor** — Full DPDP assessment required before onboarding

---

## PHASE 2 — DPDP VENDOR ASSESSMENT QUESTIONNAIRE RESPONSES

IndNational Bank sends DPDP Assessment Questionnaire to CloudDocs.
CloudDocs responds (with supporting evidence):

### Section A: Governance

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Do you have an appointed DPO or Privacy Officer? | Yes — Amit Kumar, CPO | Appointment letter | ✅ Pass |
| Do you have a Data Protection Policy? | Yes, reviewed annually | Policy document (v2.1, Oct 2025) | ✅ Pass |
| Are you certified under ISO 27001? | ISO 27001:2022 certified since 2024 | Certificate (valid until 2027) | ✅ Pass |
| Are you certified under ISO 27701? | In progress — expected Q2 2026 | Gap assessment report | ⚠️ Partial |

### Section B: Security Controls (Rule 6)

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Do you encrypt data at rest? | Yes — AES-256 | Architecture doc + VAPT report | ✅ Pass |
| Do you encrypt data in transit? | Yes — TLS 1.3 | Architecture doc | ✅ Pass |
| Do you implement RBAC? | Yes — 3-tier access controls | Access control policy | ✅ Pass |
| Do you maintain access audit logs? | Yes — 12-month retention | SIEM configuration doc | ✅ Pass |
| Do you conduct annual VAPT? | Yes — last conducted Sept 2025 | VAPT report summary (redacted) | ✅ Pass |
| Do you have a tested DR plan? | Yes — last tested June 2025 | DR test report | ✅ Pass |
| Do you perform background checks on staff? | Yes — for all staff with customer data access | HR policy | ✅ Pass |

### Section C: Data Handling

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Do you process client data only for instructed purposes? | Yes — contractual commitment | DPA template | ✅ Pass |
| Do you use client data for your own ML/AI training? | No — explicitly prohibited | DPA + technical config | ✅ Pass |
| Do you have sub-processors for this service? | Yes — AWS India (compute/storage) | Sub-processor list | ⚠️ Flag — bank must approve |
| Is AWS India your ONLY sub-processor? | Plus Datadog (monitoring — no personal data access) | Sub-processor list | ✅ Pass (Datadog = no data access) |
| Cross-border: is data processed/stored outside India? | Backup data center in Singapore | Architecture diagram | 🔴 FLAG — Singapore not yet restricted but must be contractually addressed |

### Section D: Breach Management (Rule 7)

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Do you have a documented breach response plan? | Yes | IR Plan v3.0 (Oct 2025) | ✅ Pass |
| Can you notify the bank within 4 hours of a breach? | Yes — committed to 4-hour notification | DPA clause commitment | ✅ Pass |
| Have you experienced any personal data breaches in last 3 years? | No | Self-declaration + reference checks | ✅ Pass |
| Do you have cyber insurance? | Yes — ₹50 Cr coverage | Insurance certificate | ✅ Pass |

### Section E: Data Retention and Deletion

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Do you have a data retention schedule? | Yes | Retention policy | ✅ Pass |
| Can you securely delete data on contract end with certification? | Yes — NIST 800-88 standard | Sample deletion certificate | ✅ Pass |
| Can you fulfil bank's erasure requests within 5 business days? | Yes | DPA commitment | ✅ Pass |

### Section F: Rights Request Support

| Question | CloudDocs Response | Evidence | Bank Assessment |
|----------|-------------------|---------|-----------------|
| Can you support bank in responding to customer data rights requests? | Yes — API available for data export/deletion | Technical spec | ✅ Pass |
| Response timeline for rights request assistance? | 3 business days | DPA commitment | ✅ Pass |

---

## PHASE 3 — ASSESSMENT FINDINGS & RISK TREATMENT

| Finding | Risk Level | Required Action |
|---------|-----------|-----------------|
| ISO 27701 in progress (not yet certified) | 🟡 Medium | Accept with condition: CloudDocs provides certification within 12 months; annual review |
| Sub-processor AWS India — not pre-approved | 🟡 Medium | Bank formally approves AWS India as sub-processor; document in DPA |
| Backup data center in Singapore | 🟠 High | Contractually require: if Singapore added to restricted list, immediate notification + data migration plan. Alternatively, require India-only storage |

**Overall Assessment**: **CONDITIONALLY APPROVED** — subject to:
1. Contract must specify India-only storage (or Singapore restriction clause)
2. AWS India formally approved as sub-processor in DPA
3. ISO 27701 certification within 12 months
4. Annual VAPT report shared with Bank

---

## PHASE 4 — DATA PROCESSING AGREEMENT (DPA) KEY CLAUSES

IndNational Bank's Legal team negotiates the following key DPDP clauses into the contract:

### Clause 1 — Data Processor Acknowledgment
> CloudDocs acknowledges that it acts as a Data Processor (as defined under Section 2
> of the DPDP Act, 2023) and the Bank acts as the Data Fiduciary. CloudDocs shall
> process KYC documents only on the Bank's documented instructions.

### Clause 2 — Purpose Restriction
> CloudDocs shall process KYC documents solely for the purpose of document storage,
> retrieval, and management services as described in Schedule A. CloudDocs shall not
> use KYC documents for any other purpose, including but not limited to training of
> artificial intelligence models, commercial analytics, or any purpose beneficial
> to CloudDocs.

### Clause 3 — India Storage
> All KYC documents and metadata shall be stored and processed exclusively within
> India. CloudDocs shall not transfer, replicate, or back up KYC documents to any
> data center, server, or storage facility located outside India without the Bank's
> prior written approval, which may be withheld at the Bank's absolute discretion.
> Should the Government of India notify any restriction on transfer to any country
> where CloudDocs operates, CloudDocs shall notify the Bank within 24 hours and
> immediately cease any transfers to that country.

### Clause 4 — Breach Notification (4-Hour SLA)
> CloudDocs shall notify the Bank by telephone AND in writing within FOUR (4) hours
> of becoming aware of any personal data breach affecting KYC documents. The written
> notification shall include: (a) nature of the breach; (b) categories and number of
> customers affected; (c) likely consequences; (d) measures taken. CloudDocs shall
> not notify any regulator (including DPBI or CERT-In) or any customer without the
> Bank's prior written approval unless independently required to do so by law.

### Clause 5 — Deletion on Termination
> Within ten (10) business days of expiry or termination of this Agreement, CloudDocs
> shall securely delete all KYC documents and associated metadata using NIST 800-88
> compliant methods and shall provide the Bank with a written certificate of deletion
> specifying the deletion method, scope, and date. CloudDocs shall ensure AWS India
> (sub-processor) performs equivalent deletion.

### Clause 6 — Audit Rights
> The Bank shall have the right to audit CloudDocs' compliance with this Agreement
> and the DPDP Act 2023, including through: (a) annual security questionnaire;
> (b) review of CloudDocs' ISO 27001 surveillance audit reports; (c) independent
> third-party audit (maximum once per year unless material incident occurs); and
> (d) on-site inspection on reasonable notice in case of material breach.

---

## PHASE 5 — ONGOING MONITORING PLAN

After onboarding, IndNational Bank's TPRM team sets up:

| Activity | Frequency | Trigger |
|----------|-----------|---------|
| VAPT report review | Annual | CloudDocs shares after annual VAPT |
| Security questionnaire | Annual | Jan each year |
| ISO certification verification | Annual | At renewal |
| Contract compliance review | Annual | Before renewal |
| ISO 27701 certification verification | Within 12 months | CloudDocs commitment |
| Breach drill / tabletop exercise | Annual | Test CloudDocs' 4-hour SLA |
| Special audit (on cause) | As needed | On breach, major change, material concern |

---

## LESSONS LEARNED FROM THIS EXAMPLE

1. **Singapore backup was the key risk** — always check where ALL copies of data are stored, not just primary
2. **Sub-processor approval** — banks must formally approve and document all sub-processors
3. **4-hour SLA is achievable** — for critical vendors, build this into the contract
4. **Audit rights are non-negotiable** — do not accept a DPA without meaningful audit rights
5. **RBI + DPDP = one DPA** — integrate DPDP clauses into your existing RBI outsourcing agreement template

---

*Illustrative example for educational purposes. All names are fictional.*
*#BankVendorAssessment #ThirdPartyRisk #TPRM #DPDPBanking #DPDPVendor #DataProcessorAgreement #RBIOutsourcing #IndiaPrivacy*
