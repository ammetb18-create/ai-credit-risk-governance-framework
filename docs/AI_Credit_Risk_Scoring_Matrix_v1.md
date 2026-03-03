# AI Credit Risk Scoring Matrix v1.0  
**AI Credit Risk Governance Framework**  
Version: 1.0  
Status: Draft  
Owner: AI Governance & Model Risk Team  
Last Updated: 2026-03-02  

---

## 1. Purpose

This document defines the standardized scoring methodology used to assess, quantify, and prioritize risks associated with AI systems deployed in credit decisioning environments.

The matrix aligns with:

- NIST AI Risk Management Framework (AI RMF 1.0)
- Model Risk Management (SR 11-7 principles)
- Fair Lending & Credit Compliance Standards
- Enterprise Risk Governance Programs

This scoring matrix enables:

- Consistent AI risk classification
- Escalation thresholds for governance review
- Model approval and revalidation prioritization
- Audit traceability and defensibility

---

## 2. Risk Scoring Methodology Overview

Each identified risk is evaluated across five dimensions:

1. Impact Severity
2. Likelihood of Occurrence
3. Detectability
4. Regulatory Sensitivity
5. Fairness & Consumer Harm Exposure

Each dimension is scored on a scale of 1–5.

Final Risk Score is calculated using a weighted formula.

---

## 3. Risk Dimensions

### 3.1 Impact Severity (IS)

Assesses potential harm if the risk materializes.

| Score | Description |
|-------|-------------|
| 1 | Minimal operational impact; no customer harm |
| 2 | Limited business disruption; minor customer inconvenience |
| 3 | Moderate financial or reputational impact |
| 4 | Significant financial, regulatory, or consumer impact |
| 5 | Severe systemic impact; regulatory enforcement likely |

---

### 3.2 Likelihood of Occurrence (LO)

Probability the risk will materialize.

| Score | Description |
|-------|-------------|
| 1 | Rare (highly unlikely) |
| 2 | Unlikely |
| 3 | Possible |
| 4 | Likely |
| 5 | Highly probable or recurring |

---

### 3.3 Detectability (DE)

Ability to detect the issue before harm occurs.

| Score | Description |
|-------|-------------|
| 1 | Easily detectable via automated controls |
| 2 | Detectable via standard monitoring |
| 3 | Detectable with manual review |
| 4 | Difficult to detect |
| 5 | Not detectable before impact |

*Note: Detectability is inversely related to risk control strength.*

---

### 3.4 Regulatory Sensitivity (RS)

Exposure to legal, regulatory, or supervisory consequences.

| Score | Description |
|-------|-------------|
| 1 | No regulatory relevance |
| 2 | Limited internal policy exposure |
| 3 | Subject to standard regulatory oversight |
| 4 | Direct regulatory scrutiny (e.g., ECOA, FCRA) |
| 5 | High enforcement or litigation risk |

---

### 3.5 Fairness & Consumer Harm Exposure (FH)

Risk of discriminatory impact or consumer injustice.

| Score | Description |
|-------|-------------|
| 1 | No consumer impact |
| 2 | Low impact; no protected class exposure |
| 3 | Potential indirect bias exposure |
| 4 | Measurable disparate impact risk |
| 5 | High likelihood of unlawful discrimination |

---

## 4. Weighted Risk Formula

Final Risk Score (FRS) is calculated as:
