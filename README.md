# 🇮🇳 DPDP Compliance Advisor — Claude AI Skill

> **The most comprehensive Claude AI skill for Digital Personal Data Protection Act 2023 & DPDP Rules 2025 compliance in India.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DPDP Act 2023](https://img.shields.io/badge/DPDP%20Act-2023-blue)](https://www.meity.gov.in/DigitalPersonalData)
[![DPDP Rules 2025](https://img.shields.io/badge/DPDP%20Rules-November%202025-green)](https://www.meity.gov.in/DigitalPersonalData)
[![Claude AI Skill](https://img.shields.io/badge/Claude%20AI-Skill-orange)](https://claude.ai)
[![GRC](https://img.shields.io/badge/Framework-GRC-red)](https://github.com/your-repo)
[![ISO 27001](https://img.shields.io/badge/ISO-27001%3A2022-lightblue)](https://iso.org)
[![ISO 27701](https://img.shields.io/badge/ISO-27701%3A2019-lightblue)](https://iso.org)

---

## 🚀 What Is This?

This repository contains a **production-ready Claude AI skill** that transforms
Claude into a **Senior Cybersecurity & GRC Expert** specialising in India's
**Digital Personal Data Protection (DPDP) Act, 2023** and the **DPDP Rules, 2025**.

Anyone — compliance consultants, CISOs, legal teams, startups, banks, fintech
companies — can use this skill to get **accurate, actionable, India-specific**
data protection compliance guidance directly from Claude AI.

### ✅ What You Get

- Complete structured knowledge base of the DPDP Act 2023 (all 44 sections)
- Full coverage of DPDP Rules 2025 (Gazette No. 760, notified 13 November 2025)
- Ready-to-use compliance checklists, templates, and gap assessment frameworks
- RBI / SEBI alignment mappings for financial institutions
- ISO 27001:2022 and ISO 27701:2019 control mappings
- Phased implementation roadmap with timelines and effort estimates
- Vendor/Data Processor agreement clause library
- Penalty exposure analysis framework (up to ₹250 crore)
- Children's data protection guidance
- Cross-border data transfer compliance guidance
- Breach notification playbook (Rule 7 compliant)

---

## 📂 Repository Structure

```
dpdp-compliance-skill/
├── SKILL.md                          # 🎯 Main skill file — load this into Claude
├── README.md                         # 📖 This file
├── docs/
│   ├── ACT_SUMMARY.md                # DPDP Act 2023 — complete structured summary
│   ├── RULES_SUMMARY.md              # DPDP Rules 2025 — complete structured summary
│   ├── PENALTY_SCHEDULE.md           # Penalty schedule with business impact analysis
│   ├── RBI_SEBI_ALIGNMENT.md         # Regulatory alignment for financial sector
│   └── ISO_MAPPING.md                # ISO 27001/27701 to DPDP mapping
├── checklists/
│   ├── GAP_ASSESSMENT_CHECKLIST.md   # DPDP compliance gap assessment checklist
│   ├── CONSENT_NOTICE_CHECKLIST.md   # Rule 3 consent notice review checklist
│   ├── BREACH_RESPONSE_CHECKLIST.md  # Rule 7 breach notification checklist
│   ├── VENDOR_DPA_CHECKLIST.md       # Data Processor Agreement review checklist
│   └── SDF_READINESS_CHECKLIST.md    # Significant Data Fiduciary readiness checklist
├── templates/
│   ├── CONSENT_NOTICE_TEMPLATE.md    # Rule 3 compliant consent notice template
│   ├── DATA_PROCESSOR_AGREEMENT.md   # DPDP-compliant DPA clause library
│   ├── BREACH_NOTIFICATION_BOARD.md  # Board notification template (Schedule 3)
│   ├── BREACH_NOTIFICATION_DP.md     # Data Principal notification template
│   ├── GRIEVANCE_POLICY_TEMPLATE.md  # Grievance redressal policy template
│   └── DPIA_TEMPLATE.md              # Data Protection Impact Assessment template
└── examples/
    ├── FINTECH_COMPLIANCE_EXAMPLE.md # Example: Fintech startup compliance plan
    ├── BANK_VENDOR_ONBOARDING.md     # Example: Bank vendor DPDP assessment
    └── HEALTHCARE_DPDP_EXAMPLE.md    # Example: Healthcare data fiduciary guide
```

---

## ⚡ Quick Start — How to Use This Skill with Claude

### Option 1: Claude.ai (Web Interface)

1. Open [claude.ai](https://claude.ai)
2. Copy the contents of [`SKILL.md`](./SKILL.md)
3. Start a new conversation
4. Paste the SKILL.md content as your **first message** (or in the System Prompt if using Projects)
5. Ask your DPDP compliance question

### Option 2: Claude Projects (Recommended)

1. In Claude.ai, create a new **Project**
2. Upload `SKILL.md` to the Project's knowledge base
3. Upload any additional context files (your privacy policy, vendor list, etc.)
4. Every conversation in this Project will have DPDP expertise built-in

### Option 3: Anthropic API

```python
import anthropic

with open("SKILL.md", "r") as f:
    skill_content = f.read()

client = anthropic.Anthropic()

response = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=4096,
    system=skill_content,
    messages=[
        {
            "role": "user",
            "content": "We are a fintech startup processing 500,000 users' financial data. What are our top 5 DPDP compliance priorities?"
        }
    ]
)

print(response.content[0].text)
```

### Option 4: Claude Code

```bash
# Install Anthropic SDK
pip install anthropic

# Set your API key
export ANTHROPIC_API_KEY="your-key-here"

# Run the example script
python examples/dpdp_advisor.py
```

---

## 🎯 Sample Queries You Can Ask

Once the skill is loaded, you can ask questions like:

### Compliance Gaps
```
"Conduct a DPDP gap assessment for a payment gateway processing 
2 million transactions per month. What are our highest penalty 
exposure areas?"
```

### Consent Management
```
"Review this consent notice and tell me what's missing under Rule 3 
of DPDP Rules 2025: [paste your consent notice]"
```

### Data Breach Response
```
"Our database was breached at 3 AM. 50,000 customers' names, emails, 
and masked credit card numbers were exposed. Walk me through the DPDP 
breach response process step by step."
```

### Vendor Management
```
"We're onboarding a cloud storage vendor who will store customer KYC 
documents. What DPDP clauses must be in our Data Processing Agreement?"
```

### RBI + DPDP Alignment
```
"We're an RBI-regulated NBFC. A customer has requested erasure of their 
data under DPDP Section 12. But RBI requires us to keep KYC records for 
10 years. How do we handle this conflict?"
```

### Significant Data Fiduciary
```
"We process health data of 10 million patients across India. Are we 
likely to be notified as a Significant Data Fiduciary? What should we 
do to prepare?"
```

### Children's Data
```
"Our ed-tech platform serves students aged 10–17. What DPDP obligations 
do we have? How do we implement verifiable parental consent?"
```

---

## 📋 Key DPDP Facts — At a Glance

| Topic | Key Fact |
|-------|---------|
| **Act Name** | Digital Personal Data Protection Act, 2023 |
| **Act Number** | No. 22 of 2023 |
| **President's Assent** | 11 August 2023 |
| **Rules Notified** | 13 November 2025 (Gazette No. 760) |
| **Enforcer** | Data Protection Board of India (DPBI) |
| **Appellate Authority** | TDSAT (Telecom Disputes Settlement & Appellate Tribunal) |
| **Max Penalty** | ₹250 Crore (security breach) |
| **Breach Notification** | As soon as reasonably practicable |
| **Child Age** | Under 18 years |
| **Rights** | Information, Correction, Erasure, Grievance, Nomination |
| **Cross-Border** | Blacklist approach — transfers allowed unless country notified |
| **SDF Criteria** | Volume, sensitivity, sovereignty risk, security risk, electoral democracy |
| **Consent Standard** | Free, specific, informed, unconditional, unambiguous |
| **Language Support** | English + 22 Eighth Schedule languages |
| **Appeal Window** | 60 days from Board order |

---

## 🏦 Sector-Specific Guidance

### Banking & Financial Institutions (RBI-regulated)
- DPDP + RBI IT Framework + RBI Outsourcing Guidelines
- Key challenge: Data retention conflicts (RBI 10-year retention vs. DPDP erasure rights)
- Key strength: Existing security frameworks align with Rule 6 requirements

### FinTech & Payment Aggregators
- High-risk: Large volume of financial personal data → likely SDF candidates
- Consent architecture critical for onboarding flows
- UPI/payment data processing — purpose limitation is key

### Healthcare & Hospitals
- Patient data = high sensitivity → highest breach penalty exposure
- Children's data of patients under 18 → parental consent required
- Health services likely exempt from parental consent (to be notified by Govt)

### Ed-Tech Platforms
- Large child user base → Section 9 compliance is critical
- Age verification mechanisms mandatory
- DPIA required for AI/algorithm-based learning personalisation

### E-Commerce & Retail
- Consent for personalisation, targeted advertising — must be granular
- Third-party sharing (analytics, advertising) — each third party must be disclosed
- Cross-border data transfers (international cloud, CDN) — monitor restriction list

### IT Services & Outsourcing (Data Processors)
- Must implement security safeguards equivalent to Data Fiduciary
- Breach notification to client DF within agreed SLA
- Support DF in responding to Data Principal rights requests
- DPAs must be updated for all Indian client contracts

---

## 📊 Penalty Exposure Quick Reference

| Violation | Section | Max Penalty |
|-----------|---------|------------|
| Failure to implement security safeguards | Sec 8(5) + Rule 6 | **₹250 Crore** |
| Failure to notify Board of breach | Sec 8(6) + Rule 7 | **₹200 Crore** |
| Processing children's data without parental consent | Sec 9 | **₹200 Crore** |
| Non-compliance with SDF additional obligations | Sec 10 | **₹150 Crore** |
| Non-compliance with Data Fiduciary general obligations | Sec 8 | **₹50 Crore** |
| Non-compliance with Data Principal rights requests | Secs 11–14 | **₹10,000/instance** |
| Data Principal duty violations | Sec 15 | As prescribed |
| Voluntary undertaking breach | Sec 31 | As prescribed |

---

## 🗺️ DPDP Implementation Roadmap (Summary)

```
Phase 0 (Weeks 1–4):    BASELINE ASSESSMENT
                         ↓ Gap report, data inventory, penalty exposure

Phase 1 (Months 1–3):   FOUNDATION
                         ↓ Consent notices, privacy policy, DPAs, breach SOP

Phase 2 (Months 3–6):   RIGHTS & CONTROLS
                         ↓ Rights portal, security controls, training, vendor assessment

Phase 3 (Months 6–12):  ADVANCED (SDFs & Complex DFs)
                         ↓ DPIA framework, auditor, algorithmic accountability, ISO 27701

Phase 4 (Ongoing):      SUSTAIN & MONITOR
                         ↓ Quarterly reviews, annual audits, regulatory monitoring
```

---

## 🤝 Contributing

We welcome contributions from compliance professionals, lawyers, CISOs, and
technologists working in the Indian data protection space.

**How to contribute:**
1. Fork this repository
2. Create a feature branch (`git checkout -b feature/add-healthcare-guidance`)
3. Commit your changes (`git commit -m 'Add DPDP healthcare sector guidance'`)
4. Push to the branch (`git push origin feature/add-healthcare-guidance`)
5. Open a Pull Request

**Contribution areas:**
- Sector-specific guidance (healthcare, fintech, telecom, etc.)
- State-specific considerations
- Case studies and illustrative examples
- Translation of guidance into Indian languages
- Integration examples with popular GRC tools
- Regulatory update tracking

---

## ⚠️ Disclaimer

This skill and all content in this repository is provided for **informational
and educational purposes only**. It does not constitute legal advice. The DPDP
Act and Rules are evolving — notifications, clarifications, and Board orders
will continue to refine compliance requirements.

**Always consult a qualified legal counsel** for advice specific to your
organisation's situation. The Data Protection Board of India has not reviewed
or endorsed this skill.

---

## 📜 License

This project is licensed under the **MIT License** — see [LICENSE](./LICENSE)
file for details. You are free to use, modify, and distribute this skill in
your own products and services.

---

## 🔗 Official Resources

- [MeitY DPDP Portal](https://www.meity.gov.in/DigitalPersonalData)
- [DPDP Act 2023 — Official Gazette](https://egazette.gov.in)
- [DPDP Rules 2025 — Official Gazette (Gazette No. 760, 13 Nov 2025)](https://egazette.gov.in)
- [Data Protection Board of India](https://www.meity.gov.in)
- [RBI IT Framework for Banks](https://rbi.org.in)
- [SEBI CSCRF](https://sebi.gov.in)
- [IT Act 2000](https://www.indiacode.nic.in)

---

## 🏷️ Tags & Keywords

`#DPDP` `#DPDPAct2023` `#DPDPRules2025` `#DigitalPersonalDataProtection`
`#IndiaPrivacyLaw` `#DataProtectionIndia` `#DPDPA` `#MeitY` `#DPBI`
`#DataProtectionBoardIndia` `#ConsentManagement` `#DataFiduciary`
`#DataPrincipal` `#SignificantDataFiduciary` `#DataBreachIndia`
`#GRC` `#Compliance` `#CyberSecurity` `#PrivacyCompliance`
`#ISO27001` `#ISO27701` `#RBICompliance` `#SEBICompliance`
`#FinTechCompliance` `#BankingCompliance` `#IndiaGDPR`
`#ClaudeAI` `#AISkill` `#ClaudeSkill` `#AnthropicClaude`
`#PrivacyByDesign` `#DataMinimization` `#ConsentNotice`
`#DataProcessorAgreement` `#VendorRiskManagement` `#ThirdPartyRisk`
`#CISO` `#DPO` `#DataProtectionOfficer` `#DPIA`
`#DataProtectionImpactAssessment` `#ChildrensDataProtection`
`#CrossBorderDataTransfer` `#DataLocalization` `#IndianPrivacyLaw`
`#PrivacyLaw` `#CyberLaw` `#InfoSec` `#DataGovernance`
`#StartupCompliance` `#NBFCCompliance` `#PaymentAggregator`
`#HealthcareDataProtection` `#EdTechCompliance` `#EcommercePrivacy`

---

*Built with ❤️ for India's compliance community. Star ⭐ this repo if it helps you!*

*Last updated: November 2025 | DPDP Rules 2025 compliant*
