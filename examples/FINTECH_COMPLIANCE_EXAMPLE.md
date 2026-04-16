# Example: FinTech Startup DPDP Compliance Plan
## Illustrative Case Study — Payments + Lending Platform

> **Scenario**: PaySmart India Pvt. Ltd. is a Series B FinTech offering a
> mobile app combining UPI payments, BNPL (Buy Now Pay Later), and personal
> loans. 15 lakh registered users. 3 lakh monthly active users. Processes
> financial and biometric data. Seeking to onboard with 3 major private banks.

---

## COMPANY PROFILE

| Parameter | Details |
|-----------|---------|
| **Entity** | PaySmart India Pvt. Ltd. |
| **Sector** | FinTech — Payments + Digital Lending |
| **Data Principal Base** | 15 lakh registered users |
| **Data Types** | Name, email, phone, PAN, Aadhaar (VID only), bank account, income, credit score, UPI transaction history, biometric (fingerprint for app login), device data |
| **Third Parties** | Cloud provider (AWS India), credit bureau (CIBIL), KYC vendor, RBI-regulated bank partner, merchant aggregator, analytics vendor |
| **Regulatory Status** | RBI PA (Payment Aggregator) licensed; NBFC-P2P pending |
| **Current Frameworks** | None — greenfield compliance |

---

## STEP 1 — DPDP GAP ASSESSMENT FINDINGS

### Critical Gaps (Penalty Exposure: ₹200–250 Crore)

| Gap | Section | Penalty |
|-----|---------|---------|
| Biometric data (fingerprint) encrypted in app but **not in backend storage** | Sec 8(5) + Rule 6 | ₹250 Cr |
| **No breach notification SOP** — would not know how to notify Board/users if breach occurred | Rule 7 | ₹200 Cr |
| **No age verification** — minors can register by entering false date of birth | Sec 9 + Rule 8 | ₹200 Cr |

### Major Gaps (Penalty Exposure: ₹50 Crore)

| Gap | Section | Penalty |
|-----|---------|---------|
| Consent notice is embedded in 47-page Terms of Service — not itemised per Rule 3 | Sec 5 + Rule 3 | ₹50 Cr |
| No valid legal basis documented for **sharing transaction data with analytics vendor** | Sec 4 | ₹50 Cr |
| **3 of 5 vendor contracts** have no DPA clauses | Sec 8 | ₹50 Cr |
| No consent withdrawal mechanism in app | Sec 6(4) + Rule 4 | ₹50 Cr |
| Data retention policy not defined — data retained indefinitely | Sec 8(7) | ₹50 Cr |

### Medium Gaps (Penalty Exposure: ₹10,000/instance)

| Gap | Section | Penalty |
|-----|---------|---------|
| No in-app rights request mechanism | Secs 11–14 | ₹10,000/instance |
| No grievance officer published on website | Sec 13 | ₹10,000/instance |
| No process to respond to correction/erasure requests | Sec 12 | ₹10,000/instance |

**Total Maximum Penalty Exposure**: **~₹800 Crore**

---

## STEP 2 — LEGAL BASIS MAPPING

For each processing activity, PaySmart maps its legal basis:

| Processing Activity | Data Involved | Legal Basis | DPDP Reference |
|--------------------|--------------|------------|---------------|
| Account registration | Name, email, phone, DOB | Consent | Sec 6 |
| UPI payment processing | Bank account, UPI ID, transaction data | Sec 7(a) — voluntary provision for payment service | Sec 7(a) |
| KYC verification | PAN, Aadhaar VID | Sec 7(c) — legal obligation under RBI KYC MD | Sec 7(c) |
| Credit score check | PAN, income, transaction history | Consent (separate — for lending product) | Sec 6 |
| Biometric app login | Fingerprint | Consent (optional — user can choose PIN instead) | Sec 6 |
| Marketing emails | Email, usage data | Consent — separate opt-in | Sec 6 |
| Analytics (aggregate) | Anonymised transaction data | Post-anonymisation: not personal data | N/A |
| Analytics (individual) | User transaction patterns | **GAP — no legal basis** → Action: Obtain consent or remove | Sec 4 |
| Fraud detection (internal) | Transaction data, device data | Sec 7(a) — implied in service; Sec 7(c) — RBI fraud reporting | Sec 7 |
| Credit bureau reporting | PAN, loan data | Sec 7(c) — legal obligation (Credit Info Companies Act) | Sec 7(c) |

---

## STEP 3 — CONSENT NOTICE REDESIGN

**Before (Non-Compliant):**
> "By downloading the app, you agree to our Terms of Service and Privacy Policy.
> We may use your data to improve our services."

**After (DPDP-Compliant, Rule 3 Format):**

---

### PaySmart — How We Use Your Data

| # | Your Data | Why We Use It | How Long |
|---|-----------|--------------|----------|
| 1 | Name, email, phone | Creating and managing your account | Until you close your account + 6 months |
| 2 | PAN, Aadhaar VID | Identity verification (required by RBI) | 10 years (legal requirement) |
| 3 | Bank account details | Processing your UPI payments | Until you delink account |
| 4 | Credit score and income | Assessing your loan eligibility (only if you apply for a loan) | Duration of loan + 5 years |
| 5 | Fingerprint | Securing your app login (optional — you can use PIN instead) | Until you disable this feature |

**Who we share your data with:**
- CIBIL (credit bureau) — for credit checks when you apply for a loan
- Your bank — to process payments
- AWS India — stores all your data securely in India

**You can withdraw your consent at any time**: Settings → Privacy → Manage Consents

**Your rights**: Information / Correction / Erasure / Grievance — tap here

**Grievance Officer**: Priya Sharma | privacy@paysmart.in | Responds in 3 business days

**Complaint to Board**: [Board portal link]

---

**Separate consent captures (each with own checkbox):**
- ☐ I agree to the above (required for account creation)
- ☐ I agree to credit assessment for loan products (optional — required only when applying for loan)
- ☐ I agree to receive marketing communications (optional)
- ☐ I agree to biometric login (optional)

---

## STEP 4 — BANK ONBOARDING REQUIREMENTS

PaySmart is seeking to onboard with IndSecure Bank as a technology partner.
The bank's TPRM team sends a DPDP assessment questionnaire. Here's how
PaySmart responds after completing its compliance programme:

| Bank Requirement | PaySmart Response | Evidence |
|-----------------|-------------------|---------|
| Valid DPDP consent notices | Rule 3-compliant notices in app | Screenshot + legal review |
| Data encryption at rest and transit | AES-256 encryption; TLS 1.3 | CISO certification + VAPT report |
| Breach notification SOP | 4-hour notification to bank + Board | Written SOP document |
| Data Processor Agreement | Executed with all sub-processors | DPA copies |
| Data retention policy | Defined per data type + RBI alignment | Policy document |
| Vendor DPDP risk assessments | All Tier 1 vendors assessed | Assessment reports |
| Grievance mechanism | Published on website; officer named | Website screenshot |
| Age verification | In-app age gate + parental consent for minors | Technical specification |
| DPO (or Privacy Lead) | Privacy Lead appointed; DPO search for SDF notification | Appointment letter |
| ISO 27001 | Certification in progress; gap closure plan provided | Gap assessment report |

**Outcome**: Bank approves onboarding subject to ISO 27001 certification within 12 months.

---

## STEP 5 — SDF ASSESSMENT FOR PAYSMART

**Question**: Is PaySmart at risk of being notified as a Significant Data Fiduciary?

**Assessment:**

| SDF Criterion | PaySmart Position | Risk |
|--------------|-------------------|------|
| Volume | 15 lakh users — below 1 crore threshold | Low currently; monitor as scale grows |
| Sensitivity | Financial + biometric data | High |
| Sovereignty risk | Payment infrastructure; could be targeted | Medium |
| Electoral democracy | No direct link | Low |
| Security of State | No direct link | Low |

**Verdict**: Not an immediate SDF candidate at current scale. However, at 1 crore users (which PaySmart projects within 3 years), SDF notification becomes likely.

**Recommendation**: Prepare SDF-ready governance NOW:
- Begin DPO search and appointment
- Implement DPIA framework
- Engage potential independent data auditor

---

## STEP 6 — IMPLEMENTATION ROADMAP FOR PAYSMART

### Month 1 (Critical — ₹450 Cr exposure)
- [ ] Encrypt biometric data in backend storage (CISO)
- [ ] Draft and implement Breach Notification SOP (CISO + Legal)
- [ ] Implement age verification gate in app (Product + Tech)

### Month 2 (Major — ₹50 Cr exposure)
- [ ] Redesign consent notice per Rule 3 (Product + Legal)
- [ ] Add consent withdrawal to app Settings (Product + Tech)
- [ ] Execute DPAs with all 5 vendors (Legal)
- [ ] Document legal basis for analytics vendor data sharing (Legal)
- [ ] Define data retention policy (Legal + IT)

### Month 3–4 (Medium)
- [ ] Build in-app rights request mechanism (Product + Tech)
- [ ] Publish grievance officer on website (Marketing + Legal)
- [ ] Build rights request workflow (Compliance + Customer Service)
- [ ] Conduct all-staff DPDP awareness training (HR + Compliance)
- [ ] Complete data inventory and flow maps (IT + Compliance)

### Month 5–6 (SDF Prep)
- [ ] Appoint Privacy Lead / begin DPO search
- [ ] Initiate ISO 27001 gap assessment
- [ ] Conduct first DPIA (for AI-based credit scoring)
- [ ] Update all customer communications for DPDP alignment

**Total compliance budget estimate**: ₹80–120 Lakh
**Penalty exposure mitigated**: ~₹800 Crore
**ROI**: 67:1

---

*Illustrative example for educational purposes. All company names are fictional.*
*#FinTechCompliance #DPDPFinTech #PaymentAggregator #DPDPStartup #IndiaPrivacy #DPDPAct2023 #RBICompliance*
