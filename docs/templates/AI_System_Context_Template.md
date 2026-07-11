# AI System Context Template

## Purpose

This template helps QA teams understand the context of an AI system before defining risks, QA activities, evidence needs, validation scope or release readiness criteria.

It should be completed early in the AI QA Lifecycle and updated when the system, data, model, users, operating context or intended use changes.

---

## 1. System Overview

| Field | Description |
|---|---|
| System name |  |
| System owner |  |
| Business area |  |
| Main purpose |  |
| AI capability used |  |
| Current lifecycle stage |  |
| Version or release |  |
| Date of assessment |  |

---

## 2. Intended Use

| Question | Answer |
|---|---|
| What is the AI system intended to support or automate? |  |
| Who are the intended users? |  |
| Who may be affected by the system outputs or actions? |  |
| What decisions, recommendations, predictions or actions may depend on the system? |  |
| What is explicitly out of scope for this system? |  |

---

## 3. AI Component Context

| Question | Answer |
|---|---|
| What AI component or capability is used? |  |
| Is the component internally developed, externally provided or integrated as a third-party service? |  |
| What type of AI capability is involved? |  |
| What are the main inputs? |  |
| What are the main outputs? |  |
| Are outputs deterministic, probabilistic or variable? |  |
| Are confidence scores, explanations or reasoning traces available? |  |

---

## 4. Data Context

| Question | Answer |
|---|---|
| What data is used to train, validate, test, operate or monitor the system? |  |
| What are the main data sources? |  |
| Is personal, sensitive or confidential data involved? |  |
| Are known data quality issues documented? |  |
| Are missing values, outliers, bias or representativeness issues relevant? |  |
| Is data drift expected or possible after deployment? |  |

---

## 5. User and Operational Context

| Question | Answer |
|---|---|
| Where will the system be used? |  |
| How often will it be used? |  |
| Will it be used by internal users, external users or both? |  |
| Is human review, approval or override possible? |  |
| What happens if the AI component fails or produces an unreliable output? |  |
| Are fallback mechanisms defined? |  |

---

## 6. Impact and Criticality

| Question | Answer |
|---|---|
| What could happen if the AI system produces an incorrect, biased, misleading or unreliable output? |  |
| Could the system affect people, customers, employees or vulnerable groups? |  |
| Could the system affect legal, financial, operational, safety or reputational outcomes? |  |
| Is the AI output advisory, partially automated or fully automated? |  |
| Is human approval required before action is taken? |  |
| What is the initial impact level? | High / Medium / Low / Unknown |

---

## 7. Quality Concerns

| Quality dimension | Relevance | Notes |
|---|---|---|
| Data quality | High / Medium / Low / Not applicable |  |
| Model behaviour | High / Medium / Low / Not applicable |  |
| System integration | High / Medium / Low / Not applicable |  |
| Reliability and robustness | High / Medium / Low / Not applicable |  |
| Explainability and transparency | High / Medium / Low / Not applicable |  |
| Fairness and bias | High / Medium / Low / Not applicable |  |
| Security, privacy and misuse risk | High / Medium / Low / Not applicable |  |
| Human oversight and usability | High / Medium / Low / Not applicable |  |
| Monitoring and continuous quality | High / Medium / Low / Not applicable |  |

---

## 8. Initial Risk Notes

| Risk area | Initial notes |
|---|---|
| Incorrect or unreliable output |  |
| Biased or unfair outcome |  |
| Lack of explainability |  |
| Poor data quality |  |
| Data drift or model degradation |  |
| Security or prompt injection |  |
| Privacy or sensitive data exposure |  |
| Misuse or harmful use |  |
| Lack of human oversight |  |
| Operational failure or poor fallback |  |

---

## 9. Evidence Needed

| Evidence type | Needed? | Notes |
|---|---|---|
| Intended use description | Yes / No |  |
| Risk assessment | Yes / No |  |
| Data quality assessment | Yes / No |  |
| AI component validation summary | Yes / No |  |
| System test evidence | Yes / No |  |
| Explainability review | Yes / No |  |
| Fairness or bias assessment | Yes / No |  |
| Security and privacy input | Yes / No |  |
| Monitoring approach | Yes / No |  |
| Decision record | Yes / No |  |

---

## 10. Open Questions

| Question | Owner | Target date |
|---|---|---|
|  |  |  |

---

## 11. Review and Ownership

| Field | Description |
|---|---|
| Prepared by |  |
| Reviewed by |  |
| Decision owner |  |
| Review date |  |
| Next review trigger |  |

---

## Notes

This template is intentionally lightweight. It is not a full risk assessment, validation plan or release readiness checklist.

Its purpose is to establish enough context to decide what QA activities, evidence and governance steps are needed next.
