# Model Inventory Register v1.0  
**AI Credit Risk Governance Framework**  
Version: 1.0  
Status: Active  
Owner: Model Risk Management (MRM)  
Last Updated: 2026-03-02  

---

# 1. Purpose

This register serves as the centralized inventory of all AI/ML models used within the credit risk lifecycle.

It ensures:

- Enterprise-wide model visibility  
- Regulatory traceability  
- Risk tier classification  
- Validation and revalidation tracking  
- Governance accountability  

Aligned with:

- NIST AI RMF (Govern Function)  
- SR 11-7 Model Risk Management  
- OCC / Federal Reserve Supervisory Expectations  

---

# 2. Model Inventory Table

| Model ID | Model Name | Business Function | Risk Tier | Owner | Validation Status | Last Validation | Next Review | Deployment Status |
|----------|------------|------------------|-----------|--------|------------------|----------------|-------------|------------------|
| CR-001 | Credit Approval Model v2 | Loan Underwriting | High | Credit Risk | Validated | 2026-01-15 | 2027-01-15 | Production |
| CR-002 | Fraud Detection Model | Application Screening | Moderate | Risk Ops | In Review | 2025-11-10 | 2026-11-10 | Production |
| CR-003 | Collections Prioritization Model | Collections | Low | Operations | Pending | N/A | 2026-06-01 | Pilot |

---

# 3. Risk Tier Definitions

## Tier 1 – Critical
- Direct credit decisioning impact
- Regulatory exposure (ECOA, FCRA)
- High fairness risk
- Consumer harm potential

## Tier 2 – High
- Indirect credit influence
- Moderate regulatory exposure

## Tier 3 – Moderate
- Operational optimization
- Limited consumer exposure

## Tier 4 – Low
- Internal analytics only
- No consumer-facing decision impact

---

# 4. Required Documentation Per Model

Each registered model must include:

- Risk Assessment (Scoring Matrix)
- Fair Lending Testing Report
- Validation Report
- Data Lineage Documentation
- Deployment Approval Record
- Monitoring Dashboard Link

---

# 5. Governance Requirements

- All new AI models must be registered prior to deployment.
- Quarterly review of inventory completeness.
- Annual revalidation required for Tier 1 and Tier 2 models.
- Decommissioned models must remain archived for audit traceability.

---

# 6. Alignment to NIST AI RMF

| AI RMF Function | Implementation |
|-----------------|---------------|
| Govern | Model ownership & accountability |
| Map | Business function classification |
| Measure | Validation status tracking |
| Manage | Revalidation & lifecycle control |

---

**End of Document**
