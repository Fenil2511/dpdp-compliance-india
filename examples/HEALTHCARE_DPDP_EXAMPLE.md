# Example: Healthcare Data Fiduciary DPDP Compliance Guide
## Hospitals, Diagnostic Labs, Health Apps & Telemedicine Platforms

> **Scenario**: MedFirst Health Pvt. Ltd. operates a telemedicine app
> (5 lakh users), a chain of 12 diagnostic labs (processes 2 lakh tests/month),
> and an AI-powered diagnostic tool. Patients include adults and minors.
> Processes health, contact, insurance, and prescription data.

---

## WHY HEALTHCARE IS HIGH-RISK UNDER DPDP

| Risk Factor | Healthcare Context | DPDP Penalty |
|-------------|-------------------|-------------|
| Data sensitivity | Health data = highest sensitivity | Sec 8(5) — ₹250 Cr for security failure |
| Volume | Lakhs of patients | Likely SDF candidate |
| Vulnerability | Patients are vulnerable individuals (ill, elderly, children) | Higher breach impact = higher penalty |
| Children's data | Paediatric patients | Sec 9 — ₹200 Cr |
| Breach consequences | Medical identity fraud; discrimination by insurers; reputational harm | Maximum penalty justified |
| Cross-border | International telemedicine; overseas health insurance | Sec 16 monitoring required |

---

## STEP 1 — DATA INVENTORY FOR HEALTHCARE

MedFirst maps all personal data categories:

| Data Category | Source | Sensitivity | DPDP Obligation |
|--------------|--------|-------------|----------------|
| Patient name, DOB, gender, contact | Registration | General personal data | Standard DPDP + consent |
| Health condition / diagnosis | Consultation, lab results | **Sensitive** — health data | Higher security; consent |
| Prescription and medication history | Consultation | **Sensitive** | Higher security; consent |
| Lab test results (blood, urine, imaging) | Diagnostic labs | **Sensitive** — health data | Higher security; consent |
| Health insurance details | Billing | Financial + health | Consent |
| Biometric (if used for identification) | Some facilities use thumbprint check-in | **Very sensitive** | Explicit consent + security |
| AI diagnostic data (symptoms, patterns) | AI tool | Health data | DPIA required if SDF |
| Minor patient data (under 18) | Paediatric services | **Children's data** | Parental consent + Section 9 |
| Employee medical records | Occupational health | Health + employment | Sec 7(h) legitimate use |
| CCTV (hospital/lab premises) | Physical security | Identifiable footage | Rule 6; 30-day retention |

---

## STEP 2 — LEGAL BASIS FOR HEALTHCARE PROCESSING

| Processing Activity | Legal Basis | DPDP Reference | Notes |
|--------------------|------------|---------------|-------|
| Diagnosing and treating patients | Consent (explicit for health data) | Sec 6 | Medical consent form = DPDP consent notice |
| Emergency treatment (unconscious patient) | Sec 7(f) — medical emergency | Sec 7(f) | No consent needed; document emergency nature |
| Epidemic / public health reporting | Sec 7(g) — public health threat | Sec 7(g) | COVID-19 type notifications = legitimate |
| Processing children's health data | Verifiable parental/guardian consent | Sec 9 | Parent signs consent form |
| Sharing with insurance company | Consent (at registration/claim stage) | Sec 6 | Must be explicit; separate consent |
| Sharing with specialist referral | Consent | Sec 6 | Patient authorises referral |
| Health data for research | Sec 17(2)(d) — research exemption | Sec 17 | Only if anonymised + standards followed |
| Employee health screening | Sec 7(h) — employment | Sec 7(h) | Occupational health requirements |

---

## STEP 3 — CONSENT NOTICE FOR HEALTHCARE (Rule 3)

MedFirst redesigns its patient registration form to be the DPDP consent notice:

---

### PATIENT DATA CONSENT — MedFirst Health

**MedFirst Health Pvt. Ltd.** | [Address] | privacy@medFirst.in

**How We Use Your Health Information**

| # | Your Information | Why We Use It | Who We Share With | How Long |
|---|-----------------|--------------|------------------|----------|
| 1 | Name, DOB, contact | Creating your patient record; scheduling | Our clinical staff only | Until you request deletion (minimum 7 years — medical records law) |
| 2 | Health complaints, symptoms | Diagnosis and treatment | Your treating doctor + lab technicians | 7 years minimum (Medical Council of India guidelines) |
| 3 | Lab test results | Diagnosis and follow-up | Your doctor; you (via app/report) | 7 years minimum |
| 4 | Prescription and medicines | Treatment management; pharmacy if needed | Your doctor; pharmacy (only with your approval) | 7 years minimum |
| 5 | Health insurance details | Processing insurance claims (only if you use insurance) | Your insurance company (only for your claims) | Duration of insurance + 3 years |
| 6 | Your child's health information (if applicable) | Paediatric treatment and care | Treating paediatrician + MedFirst staff | 7 years minimum from date of treatment |

**Who we do NOT share your data with:** Pharmaceutical companies for marketing; data brokers; advertisers.

**Your Rights:** You can ask us what data we hold about you, correct any errors, or raise a concern with us at any time.

**Contact:** privacy@medFirst.in | Grievance: Dr. [Name], CMO — respond in 5 business days

**Complaint to Board:** [Board portal link — when published]

---

**☐ I have read and understood the above. I consent to MedFirst Health processing my health information as described.**

**For patients under 18 — Parent/Guardian must sign:**
**☐ I am the parent/lawful guardian of [patient name]. I provide consent for processing my child's health information as described.**

**Parent/Guardian Name:** ___________________
**Relationship to Patient:** ___________________
**Signature:** ___________________

---

## STEP 4 — CHILDREN'S DATA (PAEDIATRIC PATIENTS)

Under Section 9 and Rule 8, MedFirst must:

### Age Determination
- Registration form captures date of birth → system flags patients under 18
- Front desk staff trained to verify parental presence for patients under 18

### Verifiable Parental Consent
- Parent/guardian signs physical consent form (see above)
- Parent/guardian identity verified via photo ID (Aadhaar, PAN, driving licence)
- Both patient DOB and parent ID documented in patient record

### What MedFirst CANNOT do for child patients:
- Share minor's health data with any third party for marketing
- Use minor's data for AI training without proper anonymisation
- Process minor's data for any purpose beyond their healthcare

### Emergency exception:
- If a minor presents alone with a medical emergency → treat first under Section 7(f)
- Obtain parental consent retrospectively as soon as feasible
- Document the emergency nature in the record

---

## STEP 5 — AI DIAGNOSTIC TOOL — DPIA REQUIREMENT

MedFirst uses an AI tool that analyses symptoms and suggests diagnoses for doctors to review.

**DPIA trigger**: New technology + health data + automated processing affecting patients → DPIA mandatory (SDF) or strongly recommended (all DFs).

### DPIA Summary for AI Diagnostic Tool

| DPIA Element | Assessment |
|-------------|-----------|
| **Purpose** | AI-assisted differential diagnosis — aids doctors, does not replace them |
| **Data used** | Patient symptoms, vitals, lab results, age, gender |
| **Legal basis** | Consent (part of treatment consent); human review of all AI outputs |
| **Data minimisation** | AI uses minimum symptom data; no unnecessary data ingested |
| **Risk: algorithmic bias** | HIGH — AI may underperform for certain demographics (women, elderly, non-urban presentations) |
| **Risk: over-reliance by doctors** | MEDIUM — doctors may follow AI without critical review |
| **Risk: data breach of AI training data** | MEDIUM — if training data includes patient records |
| **Mitigation: bias** | Regular bias audits; diverse training data; monitor diagnostic accuracy by demographic |
| **Mitigation: over-reliance** | AI outputs labelled as "suggested" — doctor override mandatory |
| **Mitigation: training data** | All training data anonymised; no identifiable patient records in training |
| **Residual risk** | Medium — acceptable with monitoring |
| **DPO Opinion** | Approved with conditions: quarterly bias audit; patient informed of AI use in notice |

---

## STEP 6 — BREACH SCENARIO WALKTHROUGH

**Incident**: MedFirst's lab result database is accessed by an unauthorised external party. 80,000 patient records (names, phone numbers, and diagnostic test results including HIV and STI tests) are potentially exposed.

### Immediate Assessment (Hour 0–1)
- **DPDP breach?** YES — unauthorised access to personal data (health data) → compromises confidentiality → personal data breach
- **Severity?** CRITICAL — HIV/STI test results are extremely sensitive; discrimination and stigma risk
- **Affected DPs?** ~80,000

### Response Actions
| Timeline | Action |
|----------|--------|
| Hour 0 | Database taken offline; IRT activated |
| Hour 1 | CEO and DPO briefed |
| Hour 3 | Containment confirmed; affected records scope determined |
| Hour 5 | DPBI notification sent (via Digital Office) |
| Hour 5 | RBI (if bank partner involved) / State Health Ministry informed (as applicable) |
| Hour 6 | CERT-In notification sent |
| Hour 12 | Legal team reviews notification obligation to patients |
| Hours 24–48 | Patient notifications sent via registered email/SMS |
| Day 3 | Dedicated patient helpline established |
| Day 7 | External forensic investigation initiated |
| Day 30 | Root cause analysis complete; Board supplementary update |

### Patient Notification Content (Critical Sensitivity)
The notification must be carefully worded to minimise harm to patients:
- Do NOT identify which specific tests were involved in the notification subject line
- Use neutral language: "your health information" not "your HIV test results"
- Be clear about what to do; provide support resources
- Example: "If you believe your information has been misused, please contact our helpline. We can assist you in understanding your legal options."

---

## STEP 7 — SDF ASSESSMENT FOR MEDIRST

| SDF Criterion | MedFirst Position |
|--------------|------------------|
| Volume | 5 lakh app users + 2 lakh tests/month = 7 lakh+ DPs | Approaching SDF threshold |
| Sensitivity | Health data (highest sensitivity) | HIGH indicator |
| Sovereignty | No direct link | Low |
| Security of State | No direct link | Low |

**Verdict**: MedFirst is a **strong SDF candidate** based on health data sensitivity.
Even below the formal SDF notification, MedFirst should voluntarily implement:
- DPO appointment (Privacy Officer / CMO as DPO)
- DPIA for AI tool (already done above)
- Independent audit (annual)

---

## KEY HEALTHCARE-SPECIFIC COMPLIANCE POINTS

| Point | Detail |
|-------|--------|
| **Medical records retention** | Minimum 7 years (Medical Council of India); cannot erase before this even if patient requests |
| **Emergency exemption** | Section 7(f) covers emergency treatment without consent |
| **Research exemption** | Section 17(2)(d) allows use of anonymised health data for research if proper standards followed |
| **Health data sensitivity** | While DPDP doesn't explicitly create a "special category" like GDPR, health data attracts the highest penalties due to sensitivity factor in Section 33(2)(b) |
| **Insurance sharing** | Patient must give explicit consent for sharing with insurer — cannot bundle with treatment consent |
| **Pharmacy sharing** | Only share prescription with pharmacy after patient authorises |
| **International telemedicine** | If consulting overseas specialist → check if destination country is on restriction list |
| **Sensitive breach** | Health data breaches require careful communication — risk of discrimination, stigma, harm |

---

*Illustrative example for educational purposes. All names are fictional.*
*#HealthcareCompliance #DPDPHealthcare #MedicalDataProtection #PatientPrivacy #TelemedicineCompliance #DPDPAct2023 #IndiaHealthPrivacy*
