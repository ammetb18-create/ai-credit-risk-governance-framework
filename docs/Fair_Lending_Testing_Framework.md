# Fair Lending Testing Framework v1.0  
**AI Credit Risk Governance Framework**  
Version: 1.0  
Status: Active  
Owner: Fair Lending & Compliance Office  
Last Updated: 2026-03-02  

---

# 1. Purpose

This document defines the methodology, controls, and governance standards for conducting Fair Lending and Bias Testing on AI/ML systems used in credit decisioning.

This framework ensures compliance with:

- Equal Credit Opportunity Act (ECOA)
- Fair Credit Reporting Act (FCRA)
- Regulation B
- UDAAP principles
- NIST AI Risk Management Framework (Measure & Manage Functions)

The objective is to proactively identify, measure, and mitigate disparate impact and discriminatory outcomes in AI-driven credit systems.

---

# 2. Scope

This framework applies to:

- Credit underwriting models
- Pricing models
- Credit limit assignment models
- Application screening systems
- Collections prioritization models
- Any AI system influencing credit outcomes

---

# 3. Protected Class Considerations

Testing must assess potential disparate impact related to:

- Race
- Ethnicity
- Gender
- Age
- National Origin
- Marital Status
- Proxy variables (ZIP code, education, income proxies, etc.)

Where direct protected class data is unavailable, proxy methodologies must be used.

---

# 4. Fair Lending Testing Components

## 4.1 Disparate Impact Analysis

Measure approval rates and outcomes across demographic groups.

### Required Metrics:

- Approval Rate Ratio
- Denial Rate Ratio
- Adverse Impact Ratio (80% rule)
- Statistical significance testing (Chi-square / Z-test)

Threshold:

- Any ratio below 0.80 requires investigation.

---

## 4.2 Disparate Treatment Review

Assess whether similarly situated applicants receive materially different outcomes.

Requirements:

- Controlled comparative testing
- Feature impact review
- Manual override monitoring

---

## 4.3 Proxy Variable Analysis

Identify features that may indirectly correlate with protected classes.

Examples:

- ZIP Code
- Employment Gap Indicators
- Education Level
- Transaction History Patterns

Testing Methods:

- Correlation analysis
- SHAP value fairness review
- Feature importance stability review

---

## 4.4 Model Explainability Review

AI models must provide:

- Clear adverse action reason codes
- Consumer-understandable explanations
- Feature-level contribution transparency

Accepted Methods:

- SHAP
- LIME
- Partial Dependence Plots

Black-box models without explainability controls require enhanced governance review.

---

# 5. Fairness Risk Scoring

Each model must receive a Fairness Risk Score using:

- Disparate Impact Severity
- Regulatory Exposure
- Consumer Harm Potential
- Model Complexity
- Explainability Level

Fairness risk must be integrated into:

AI_Credit_Risk_Scoring_Matrix_v1.md

---

# 6. Testing Frequency

| Risk Tier | Testing Frequency |
|------------|------------------|
| Tier 1 (Critical) | Quarterly |
| Tier 2 (High) | Semi-Annual |
| Tier 3 (Moderate) | Annual |
| Tier 4 (Low) | As needed |

Additional testing required:

- After model retraining
- After data source changes
- After regulatory updates

---

# 7. Escalation Protocol

If fairness thresholds are breached:

1. Immediate compliance notification
2. Root cause analysis
3. Legal review
4. Governance Committee escalation
5. Model suspension if necessary
6. Documented remediation plan

All incidents must be logged in:

/fair-lending-incidents/

---

# 8. Documentation Requirements

Each fairness review must produce:

- Statistical test results
- Dataset description
- Methodology explanation
- Identified disparities
- Mitigation strategy
- Executive sign-off

Reports must be stored in:

/fairness-reports/

---

# 9. Governance Accountability

Responsible Parties:

- Model Owner
- Fair Lending Officer
- Compliance Team
- Model Validation Team
- AI Governance Committee

Final deployment approval requires documented fairness clearance.

---

# 10. Alignment to NIST AI RMF

| AI RMF Function | Implementation |
|-----------------|---------------|
| Govern | Defined accountability structure |
| Map | Protected class risk identification |
| Measure | Statistical bias testing |
| Manage | Mitigation & escalation controls |

---

# 11. Regulatory Readiness Statement

This framework is designed to demonstrate:

- Proactive bias mitigation
- Documented testing methodology
- Ongoing monitoring controls
- Defensible AI decisioning practices

This document supports regulatory examinations and supervisory reviews.

---

**End of Document**
