# Fair Lending Testing Framework v1.0  
**AI Credit Risk Governance Framework**  
Version: 1.0  
Status: Active  
Owner: Fair Lending & Model Risk Governance  
Last Updated: 2026-03-03  

---

# 1. Purpose

This framework establishes a structured methodology to identify, measure, monitor, and mitigate discriminatory risk in AI-driven credit decision systems operating in regulated financial environments.

It operationalizes fair lending controls in alignment with:

- Equal Credit Opportunity Act (ECOA)
- Regulation B
- Fair Housing Act (FHA)
- Fair Credit Reporting Act (FCRA)
- CFPB Supervisory Expectations
- NIST AI Risk Management Framework (Measure & Manage)

---

# 2. Scope

This framework applies to:

- Credit approval models
- Risk-based pricing models
- Credit limit assignment models
- Alternative data scoring systems
- Fraud screening systems that influence credit decisions
- Prequalification and prescreening AI tools

---

# 3. Fair Lending Risk Categories

## 3.1 Disparate Treatment

Intentional or direct discrimination based on protected characteristics.

Control Objective:
- Ensure no protected attributes are explicitly used in model training or decision logic.

---

## 3.2 Disparate Impact

Neutral variables that produce statistically significant adverse outcomes for protected classes.

Control Objective:
- Detect statistically significant disparities in approval rates, pricing, or limits.

---

## 3.3 Proxy Discrimination

Use of variables highly correlated with protected characteristics (e.g., ZIP code, behavioral signals).

Control Objective:
- Identify proxy correlations exceeding defined thresholds.

---

## 3.4 Algorithmic Drift Bias

Bias introduced post-deployment due to data shifts, macroeconomic change, or retraining cycles.

Control Objective:
- Ongoing fairness monitoring.

---

# 4. Testing Methodology

## 4.1 Protected Class Proxy Identification

Where direct protected class data is unavailable:

- Use BISG (Bayesian Improved Surname Geocoding)
- Geospatial demographic estimation
- Statistically validated proxy methodologies

Documentation Required:
- Method description
- Data sources
- Validation approach
- Confidence thresholds

---

## 4.2 Disparate Impact Analysis

Primary Statistical Metrics:

- Adverse Impact Ratio (AIR)
- Approval Rate Differential
- Pricing Differential
- Confidence Intervals
- Statistical Significance Testing (p-values)

Threshold Standard (example baseline):

- AIR < 0.80 triggers escalation review

---

## 4.3 Feature-Level Bias Testing

For each model feature:

- Correlation analysis with protected proxies
- SHAP-based fairness contribution analysis
- Sensitivity testing via feature perturbation

Escalation Trigger:
- Feature materially contributes to disparate impact without business necessity justification

---

## 4.4 Explainability & Adverse Action Compliance

Models must support:

- Reason codes aligned with ECOA requirements
- Consumer-friendly explanation logic
- Feature importance traceability
- Audit-ready documentation

---

# 5. Governance Escalation Matrix

| Severity | Description | Required Action |
|----------|------------|----------------|
| Low | Minor statistical variance | Document & monitor |
| Moderate | Statistically significant but explainable disparity | Mitigation plan required |
| High | Persistent disparity with limited business justification | Governance committee review |
| Critical | Significant disparate impact with regulatory exposure | Immediate remediation & legal review |

---

# 6. Monitoring Frequency

| Risk Tier | Monitoring Frequency |
|-----------|--------------------|
| Tier 1 (Critical Credit Models) | Monthly |
| Tier 2 (High Impact) | Quarterly |
| Tier 3 (Operational Models) | Semi-Annual |
| Tier 4 (Low Risk) | Annual |

---

# 7. Documentation Requirements

Each fairness review cycle must produce:

- Fair Lending Testing Report
- Statistical output documentation
- Escalation decision record
- Mitigation tracking log
- Governance approval record

All reports must be stored in:

/fair-lending-reviews/

---

# 8. Integration with AI Risk Lifecycle

This framework integrates with:

- Risk Scoring Matrix
- Model Inventory Register
- AI Governance Audit Checklist
- Model Validation Framework
- Regulatory Alignment Map

---

# 9. Alignment to NIST AI RMF

| AI RMF Function | Implementation |
|-----------------|---------------|
| Govern | Fair lending oversight ownership |
| Map | Risk identification for protected groups |
| Measure | Statistical bias testing |
| Manage | Mitigation & escalation |

---

# 10. Regulatory Readiness

This framework ensures readiness for:

- CFPB examination
- OCC supervisory review
- Federal Reserve model risk review
- State-level regulatory audits

---

# 11. Continuous Improvement

The Fair Lending Testing Framework must be reviewed:

- Annually
- Following major regulatory updates
- After model incidents
- After material model retraining

---

**End of Document**
