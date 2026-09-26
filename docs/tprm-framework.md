# Third-Party Risk Management (TPRM) Framework
**Organization:** SecureBank Digital Services Pvt. Ltd.  
**Scope:** Technology, Cloud & AI Vendor Onboarding and Continuous Oversight  
**Framework Alignment:** ISO/IEC 27001:2022 A.5.19 & RBI TPRM Master Directions  

---

## 1. Executive Purpose & Scope

SecureBank Digital Services Pvt. Ltd. relies on external third-party service providers for cloud infrastructure, payment settlement gateways, biometric AI verification, credit risk algorithms, customer support chatbots, and SaaS productivity suites.

This **Third-Party Risk Management (TPRM) Framework** establishes a standardized, reproducible methodology to evaluate, score, onboard, monitor, and audit third-party technology and AI vendors.

---

## 2. Weighted Vendor Risk Scoring Methodology

Vendor security, privacy, and governance posture is calculated using a **six-domain weighted scoring algorithm**:

$$\text{Overall Score} = (0.25 \times S_{\text{InfoSec}}) + (0.20 \times S_{\text{Privacy}}) + (0.20 \times S_{\text{AIGov}}) + (0.15 \times S_{\text{BCP}}) + (0.10 \times S_{\text{Compliance}}) + (0.10 \times S_{\text{Incident}})$$

### Domain Weightage & Focus Breakdown

| Assessment Domain | Weightage | Key Evaluation Criteria |
| :--- | :--- | :--- |
| **1. Information Security** | **25%** | ISO 27001/SOC2 certs, AES-256 encryption, MFA, vulnerability SLA, PenTesting. |
| **2. Data Privacy & Protection**| **20%** | DPDP Act 2023 compliance, PII segregation, zero-data-retention, masking. |
| **3. AI Governance & Ethics** | **20%** | Model explainability, bias mitigation, prompt guardrails, training data exclusion. |
| **4. Business Continuity (BCP)**| **15%** | Documented DR plan, RTO/RPO SLA (< 2 hours), bi-annual failover testing. |
| **5. Regulatory Compliance** | **10%** | RBI Master Directions mapping, Indian geographic data residency. |
| **6. Incident Management** | **10%** | 24/7 SOC, 2-hour incident notification SLA, forensic logging capabilities. |

---

## 3. Vendor Classification Tiers & Governance Rules

Based on the calculated Overall Weighted Score, vendors are assigned to one of three Risk Classification Tiers:

```
+----------------------------------------------------------------------------------------------------+
|                                  VENDOR RISK CLASSIFICATION TIERS                                  |
+----------------------------------------------------------------------------------------------------+
|  LOW RISK VENDOR       | Overall Score ≥ 80%                                                        |
|                        | Governance: Standard onboarding due diligence, annual SOC2 review.        |
+------------------------+---------------------------------------------------------------------------+
|  MEDIUM RISK VENDOR    | Overall Score 60% – 79%                                                   |
|                        | Governance: Enhanced due diligence, bi-annual security PenTest audits.    |
+------------------------+---------------------------------------------------------------------------+
|  HIGH RISK VENDOR      | Overall Score < 60%                                                       |
|                        | Governance: Senior Management sign-off, quarterly audit, mandatory remediation.|
+----------------------------------------------------------------------------------------------------+
```

---

## 4. Vendor Assessment Results Summary (6 Evaluated Suppliers)

Our comprehensive evaluation of SecureBank's active technology suppliers yielded the following scores:

```
==========================================================================================
Vendor ID | Vendor Name                   | Domain | Weighted Score | Risk Classification
------------------------------------------------------------------------------------------
VND-001   | CloudScale Solutions Ltd.     | Cloud  |     90.0%      | 🟢 Low Risk
VND-006   | OfficeCloud SaaS Corp         | SaaS   |     86.7%      | 🟢 Low Risk
VND-004   | OmniChat AI Platforms         | AI/SaaS|     74.7%      | 🟡 Medium Risk
VND-002   | FinTech Pay Gateway Services | FinTech|     73.2%      | 🟡 Medium Risk
VND-005   | AnalyticsCore AI Solutions   | AI/ML  |     63.1%      | 🟡 Medium Risk
VND-003   | SmartKYC Verification Systems | AI/KYC |     56.9%      | 🔴 High Risk (CRITICAL)
==========================================================================================
```

### Critical Findings: High-Risk Vendor (`SmartKYC Verification Systems`)
- **Overall Score:** **56.9%** (Fails 60% threshold).
- **Core Deficiencies:** Unencrypted biometric audit logs in cloud storage, missing SOC 2 certification, unvetted 4th-party offshore sub-contractors, lack of ISO 30107-3 deepfake liveness testing.
- **Required Treatment:** Freeze onboarding of new customer KYC processing via SmartKYC until vendor remediates encryption and submits third-party audit proof within 60 days.

---

## 5. 25-Question Vendor Assessment Questionnaire Overview

The TPRM framework utilizes a standardized 25-question assessment matrix mapped to the six domains. (Refer to [`templates/vendor-questionnaire.csv`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/templates/vendor-questionnaire.csv) for full schema).

### Sample Key Questions:
1. **Q-SEC-01 (InfoSec):** Does your organization maintain active ISO/IEC 27001:2022 or SOC 2 Type II certifications?
2. **Q-PRV-03 (Privacy):** Do you guarantee zero-data-retention for customer inputs used in AI model inference?
3. **Q-AIG-02 (AI Gov):** Do you perform pre-deployment demographic bias and disparate impact testing for decision-making AI models?
4. **Q-CMP-02 (Compliance):** Do you guarantee that all customer financial data remains hosted strictly within Indian geographic boundaries?
5. **Q-INC-02 (Incident):** Will your organization notify SecureBank of any security incident or breach within 2 hours of detection?

---

## 6. Vendor Offboarding & Exit Governance

When a vendor contract is terminated or retired:
1. **Data Purge Verification:** Mandatory execution of cryptographic data deletion across all vendor cloud environments with a signed Certificate of Destruction.
2. **Access Revocation:** Instant revocation of API keys, SAML SSO integrations, and network tunnels within 2 hours of contract termination.
3. **Fourth-Party Pruning:** Verification that subcontractor access rights are pruned across downstream supply chains.
