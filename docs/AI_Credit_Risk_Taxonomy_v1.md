# AI Credit Risk Taxonomy v1

## Purpose
A practical taxonomy of risks for AI-driven credit decisioning systems. This taxonomy is designed to support:
- Risk identification during model design and deployment
- Governance + audit readiness (NIST AI RMF alignment)
- Fair lending and compliance controls (e.g., ECOA/Reg B concepts)
- Monitoring and incident response planning

---

## 1) Algorithmic Bias & Discrimination Risk
Risks where AI systems create or amplify unequal outcomes for protected groups.

**Examples / Drivers**
- Disparate impact risk
- Proxy variable risk (features correlated with protected traits)
- Historical bias propagation (training data reflects past discrimination)

**Signals**
- Significant approval-rate gaps by group
- Higher false negative/positive rates for specific populations
- Feature importance dominated by socioeconomic proxies

**Typical Controls**
- Fairness testing (group metrics) before and after deployment
- Feature review for proxy variables
- Bias remediation plan + documentation

---

## 2) Regulatory & Compliance Risk
Risks of violating laws, regulations, or internal policy requirements.

**Examples / Drivers**
- ECOA / fair lending violations
- Adverse action notice deficiencies (insufficient explainability)
- Documentation insufficiency for audits/exams

**Signals**
- Inability to justify key decisions in plain language
- Missing model documentation, approvals, or change logs
- Inconsistent policy application across channels/regions

**Typical Controls**
- Compliance mapping (controls ↔ requirements)
- Governance gates (approval before release)
- Audit-ready documentation pack

---

## 3) Model Transparency & Explainability Risk
Risks arising from “black-box” behavior and limited interpretability.

**Examples / Drivers**
- Lack of explainability
- Black-box scoring dependency
- Audit traceability gaps

**Signals**
- Adverse action reasons are vague/unstable
- Stakeholders cannot explain outcomes
- Explanations change significantly with small input changes

**Typical Controls**
- Explainability tooling (global + local explanations)
- Stable adverse action logic
- Traceability (model cards, decision logs)

---

## 4) Operational Risk
Risks from failures in data pipelines, monitoring, processes, or model lifecycle.

**Examples / Drivers**
- Model drift / performance degradation
- Data pipeline corruption (missing/shifted distributions)
- Governance oversight failure (unapproved changes)

**Signals**
- Sudden change in approval rates or score distributions
- Data quality alerts (null spikes, outliers)
- Model version mismatch in production

**Typical Controls**
- Monitoring (drift, performance, fairness)
- Change management + rollback procedures
- Incident response playbooks

---

## 5) Reputational & Systemic Risk
Risks that damage trust and brand, or contribute to broader financial instability.

**Examples / Drivers**
- Consumer trust erosion
- Litigation / enforcement exposure
- Institutional instability from model-driven decisions at scale

**Signals**
- Complaint spikes / social backlash
- Regulator inquiries
- Unexpected concentration of risk in portfolios

**Typical Controls**
- Human oversight and escalation paths
- Risk appetite limits and kill-switch criteria
- Periodic independent reviews

---

## Notes (v1)
This is a v1 taxonomy intended to be expanded with:
- Clear severity/likelihood scoring (risk matrix)
- Mapping to NIST AI RMF functions (Govern / Map / Measure / Manage)
- Control library and audit checklist
