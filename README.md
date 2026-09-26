# Enterprise AI Governance & Third-Party Risk Management (TPRM) Framework
**Organization:** SecureBank Digital Services Pvt. Ltd. (Fictional Entity)  
**Domain:** BFSI (Banking, Financial Services, and Insurance) — India  
**Engagement Type:** AI Governance & Cyber Risk Consulting Portfolio Project  

---

> [!NOTE]  
> **Disclaimer:** SecureBank Digital Services Pvt. Ltd. is a hypothetical organization created for cybersecurity & AI risk consulting portfolio purposes. All use cases, vendor assessments, scoring metrics, and governance rules represent simulated consulting assumptions created for portfolio demonstration.

---

## Executive Project Overview

As **SecureBank Digital Services Pvt. Ltd.** accelerates its digital transformation, the organization is deploying artificial intelligence (AI) across key financial workflows—ranging from customer-facing conversational chatbots to automated credit scoring and biometric KYC verification. Simultaneously, SecureBank relies heavily on third-party cloud infrastructure, payment gateways, and specialized AI SaaS vendors.

This repository establishes a comprehensive **Enterprise AI Governance & Third-Party Risk Management (TPRM) Framework** designed to ensure responsible AI deployment, regulatory compliance (RBI AI & Cyber Directions, DPDP Act 2023), robust algorithmic risk classification, weighted vendor scoring, and structured escalation pathways.

---

## Workspace Structure

```
project-2-ai-governance-tprm/
├── README.md                          # Project overview and navigation guide
├── docs/
│   ├── executive-summary.md           # Board-level executive summary & governance metrics
│   ├── ai-governance-framework.md     # AI risk classification, tiers & 10-stage lifecycle
│   ├── tprm-framework.md              # Vendor scoring methodology (6 weighted domains) & 25 Qs
│   └── management-recommendations.md  # Prioritized AI & TPRM risk remediation roadmap
├── data/
│   ├── ai-use-cases.csv               # 6 BFSI AI use cases mapped to risk tiers & approvals
│   ├── ai-risk-register.csv           # 12 identified AI risks across 11 risk categories
│   ├── vendor-assessment.csv          # 6 technology/AI vendor evaluations with weighted scores
│   └── vendor-risk-register.csv       # 10 third-party supplier risk entries
├── dashboard/
│   └── index.html                     # Interactive Executive AI & TPRM Risk Dashboard
├── presentation/
│   └── presentation-outline.md        # 10-slide executive presentation Deck Outline
└── templates/
    ├── ai-risk-assessment-template.csv # Reusable AI use case risk assessment schema
    ├── vendor-questionnaire.csv       # 25-question vendor assessment questionnaire
    └── vendor-risk-template.csv       # Reusable vendor risk register schema
```

---

## Framework Architecture & Highlights

### 1. AI Risk Classification Tiers

```
+--------------------------------------------------------------------------------------------------+
|                                    AI RISK CLASSIFICATION TIERS                                  |
+--------------------------------------------------------------------------------------------------+
|  TIER 1: LOW RISK       | Internal productivity tools (e.g. Employee HR Assistant)               |
|                         | Governance: Business Owner approval, zero-data-retention API check.      |
+-------------------------+------------------------------------------------------------------------+
|  TIER 2: MEDIUM RISK    | Customer-facing tools (e.g. Chatbot, Document OCR/NLP)                 |
|                         | Governance: Business Owner + Risk Lead approval, prompt guardrails.    |
+-------------------------+------------------------------------------------------------------------+
|  TIER 3: HIGH RISK      | Financial decisioning (e.g. Credit Scoring, Fraud Detection, AI KYC)   |
|                         | Governance: AI Governance Committee / Board approval, bias audit, SHAP.|
+--------------------------------------------------------------------------------------------------+
```

### 2. Weighted Vendor Risk Scoring Methodology

Vendor security & governance posture is calculated across **six weighted operational domains**:

$$\text{Overall Vendor Score} = (0.25 \times \text{InfoSec}) + (0.20 \times \text{Privacy}) + (0.20 \times \text{AI Governance}) + (0.15 \times \text{BCP}) + (0.10 \times \text{Compliance}) + (0.10 \times \text{Incident Mgmt})$$

- **Low Risk (Score ≥ 80%):** Standard annual review.
- **Medium Risk (Score 60–79%):** Enhanced due diligence & bi-annual monitoring.
- **High Risk (Score < 60%):** Senior management sign-off, quarterly re-assessments & mandatory risk treatment.

---

## Core Audit Statistics & Portfolio Metrics

| Metric Category | Count / Rating | Key Breakdown |
| :--- | :--- | :--- |
| **AI Use Cases Evaluated** | **6 Key BFSI Use Cases** | 3 High Risk (Tier 3), 2 Medium Risk (Tier 2), 1 Low Risk (Tier 1) |
| **AI Risks Registered** | **12 Detailed Risks** | Privacy, Cybersecurity, Model Drift, Bias, Transparency, Data Quality |
| **Vendors Assessed** | **6 Key Suppliers** | 2 Low Risk, 3 Medium Risk, 1 High Risk (`SmartKYC Verification`) |
| **Vendor Risks Registered** | **10 Vendor Risks** | Unencrypted biometrics, missing SOC2, unannounced API downtime |
| **Governance Approval** | **Multi-Tier Authority** | Business Owner → CISO/Risk → AI Governance Committee → Board |

---

## How to Access the Interactive Executive Dashboard

Open the self-contained HTML dashboard in any web browser:
```bash
# Path to dashboard
project-2-ai-governance-tprm/dashboard/index.html
```
Features include:
- Executive KPI summary cards for AI use cases, vendor risk distributions, and open items.
- Interactive Chart.js graphs (AI Risk Tier Breakdown, Vendor Risk Ratings, AI Risk Category Distribution).
- Filter dropdowns for AI Risk Tier, Risk Rating, Vendor Type, Governance Status, and Search query.
- Tabbed data view toggling between AI Use Cases, AI Risk Register, Vendor Scoring, and Vendor Risk Register.

---

## Deliverable References

- [`docs/executive-summary.md`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/docs/executive-summary.md)
- [`docs/ai-governance-framework.md`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/docs/ai-governance-framework.md)
- [`docs/tprm-framework.md`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/docs/tprm-framework.md)
- [`docs/management-recommendations.md`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/docs/management-recommendations.md)
- [`data/ai-use-cases.csv`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/data/ai-use-cases.csv)
- [`data/ai-risk-register.csv`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/data/ai-risk-register.csv)
- [`data/vendor-assessment.csv`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/data/vendor-assessment.csv)
- [`data/vendor-risk-register.csv`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/data/vendor-risk-register.csv)
- [`dashboard/index.html`](file:///Users/krishnarawat/Desktop/GRC_1/project-2-ai-governance-tprm/dashboard/index.html)
