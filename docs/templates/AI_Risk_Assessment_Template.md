# AI Risk Assessment Template

## Purpose

This template supports the initial identification, analysis, prioritisation, treatment and review of risks associated with an AI system.

It should be completed after or alongside the AI System Context Template and updated when the system, data, AI component, users, operating environment, intended use or external obligations change.

The assessment should consider the complete AI system, not only the model or AI component.

---

## Assessment Guidance

- Describe risks as clearly as possible, including their causes and potential consequences.
- Consider technical, human, business, operational, legal, ethical, security and societal impacts.
- Base risk ratings on available evidence and document relevant uncertainty.
- Involve specialist reviewers when the assessment requires expertise outside the core QA team.
- Record who owns each risk, who is responsible for treatment actions and who may accept residual risk.
- Review the assessment when relevant changes or incidents occur.

---

## 1. Assessment Overview

| Field                                 | Description |
| ------------------------------------- | ----------- |
| System name                           |             |
| System owner                          |             |
| Business area                         |             |
| Version or release                    |             |
| Current lifecycle stage               |             |
| Assessment date                       |             |
| Assessment owner                      |             |
| Related system context document       |             |
| Previous assessment reference         |             |
| Applicable risk method or policy      |             |
| Risk tolerance or acceptance criteria |             |

---

## 2. Risk Assessment Scope

| Question                                                        | Answer |
| --------------------------------------------------------------- | ------ |
| What part of the AI system is covered by this assessment?       |        |
| What intended uses are covered?                                 |        |
| What uses or scenarios are excluded?                            |        |
| Which users, stakeholders or affected groups are considered?    |        |
| Which operational environments are considered?                  |        |
| Which external systems, services or third parties are relevant? |        |
| What limitations affect the scope of this assessment?           |        |

---

## 3. Risk Rating Approach

The following simple rating approach may be used for an initial assessment. Organisations may replace it with an approved internal risk method.

### Likelihood

| Rating       | Description                                                            |
| ------------ | ---------------------------------------------------------------------- |
| 1 – Unlikely | The risk is not expected under normal conditions but remains possible. |
| 2 – Possible | The risk could occur under realistic conditions.                       |
| 3 – Likely   | The risk is expected to occur or has already occurred.                 |
| Unknown      | There is not enough evidence to estimate likelihood.                   |

### Impact

| Rating          | Description                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------- |
| 1 – Limited     | The consequence is contained, reversible and has limited effect.                                                       |
| 2 – Significant | The consequence affects users, operations, decisions or quality objectives and requires intervention.                  |
| 3 – Severe      | The consequence may cause serious harm, major operational disruption, legal exposure, financial loss or loss of trust. |
| Unknown         | There is not enough evidence to estimate impact.                                                                       |

### Initial Risk Level

The initial risk level represents the risk at the time of assessment, considering controls already in place and before any additional treatment actions defined in this assessment.

Where numerical ratings are used:

`Risk score = Likelihood × Impact`

| Score         | Initial risk level |
| ------------- | ------------------ |
| 1–2           | Low                |
| 3–4           | Medium             |
| 6–9           | High               |
| Unknown input | Unknown            |

A numerical score should not replace professional judgement. The rationale for the rating should always be recorded.

---

## 4. Risk Identification

### 4.1 Risk Category Review

| Risk category                                  | Relevant?          | Initial observations |
| ---------------------------------------------- | ------------------ | -------------------- |
| Data quality                                   | Yes / No / Unknown |                      |
| Model behaviour                                | Yes / No / Unknown |                      |
| System integration                             | Yes / No / Unknown |                      |
| Reliability and robustness                     | Yes / No / Unknown |                      |
| Explainability and transparency                | Yes / No / Unknown |                      |
| Fairness and bias                              | Yes / No / Unknown |                      |
| Security, privacy and misuse                   | Yes / No / Unknown |                      |
| Human oversight and usability                  | Yes / No / Unknown |                      |
| Monitoring and continuous quality              | Yes / No / Unknown |                      |
| Legal, regulatory or compliance obligations    | Yes / No / Unknown |                      |
| Domain-specific safety or operational concerns | Yes / No / Unknown |                      |
| Third-party or supply-chain dependency         | Yes / No / Unknown |                      |

### 4.2 Initial Risk Register

A risk statement should describe what may happen, why it may happen and what consequence may result.

| Risk ID | Risk category | Risk statement | Cause or source | Potential consequence | Affected users, groups or processes |
| ------- | ------------- | -------------- | --------------- | --------------------- | ----------------------------------- |
| R-001   |               |                |                 |                       |                                     |

---

## 5. Risk Analysis and Prioritisation

| Risk ID | Existing controls | Likelihood | Impact | Initial risk level | Rating rationale | Risk owner |
| ------- | ----------------- | ---------- | ------ | ------------------ | ---------------- | ---------- |
| R-001   |                   |            |        |                    |                  |            |

The analysis should consider, where relevant:

- severity and reversibility of potential harm;
- number and characteristics of affected people or processes;
- degree of system autonomy;
- availability and effectiveness of human oversight;
- detectability of incorrect or harmful behaviour;
- availability of fallback or recovery mechanisms;
- exposure frequency and duration;
- quality and reliability of available evidence;
- uncertainty in the assessment.

---

## 6. Risk Treatment Plan

Treatment actions may prevent, reduce, detect, contain, monitor or formally accept a risk.

| Risk ID | Treatment decision                                     | Required action | Action owner | Target date | Success or completion criteria | Status                                         |
| ------- | ------------------------------------------------------ | --------------- | ------------ | ----------- | ------------------------------ | ---------------------------------------------- |
| R-001   | Prevent / Reduce / Detect / Contain / Monitor / Accept |                 |              |             |                                | Not started / In progress / Complete / Blocked |

---

## 7. Residual Risk and Acceptance

Residual risk is the risk remaining after planned controls or treatment actions have been applied.

| Risk ID | Residual likelihood | Residual impact | Residual risk level | Remaining limitations or uncertainty | Acceptance decision               | Decision owner | Decision record reference |
| ------- | ------------------- | --------------- | ------------------- | ------------------------------------ | --------------------------------- | -------------- | ------------------------- |
| R-001   |                     |                 |                     |                                      | Accepted / Not accepted / Pending |                |                           |

Residual risk should not be considered accepted unless an authorised decision owner has reviewed the available evidence and recorded the decision.

---

## 8. Evidence Requirements

| Risk ID | Evidence needed | Evidence source or artefact | Evidence owner | Target date | Status                                                       |
| ------- | --------------- | --------------------------- | -------------- | ----------- | ------------------------------------------------------------ |
| R-001   |                 |                             |                |             | Not available / Planned / In progress / Available / Reviewed |

Examples of relevant evidence may include:

- data quality assessment;
- model or AI component validation results;
- system and integration test results;
- robustness or adversarial testing;
- fairness or bias assessment;
- explainability review;
- security and privacy assessment;
- human oversight evaluation;
- monitoring design;
- incident records;
- user feedback;
- known limitation log;
- specialist review or approval.

---

## 9. Assumptions, Constraints and Unknowns

| ID      | Type                              | Description | Risk implication | Owner | Validation or review date |
| ------- | --------------------------------- | ----------- | ---------------- | ----- | ------------------------- |
| ACU-001 | Assumption / Constraint / Unknown |             |                  |       |                           |

Assumptions should be validated where possible. Unknowns that could materially affect the assessment should be treated as risks or evidence gaps.

---

## 10. Specialist Review Needs

| Review area                    | Needed?            | Reason | Reviewer or owner | Status |
| ------------------------------ | ------------------ | ------ | ----------------- | ------ |
| Data and data quality          | Yes / No / Unknown |        |                   |        |
| AI engineering or data science | Yes / No / Unknown |        |                   |        |
| Security                       | Yes / No / Unknown |        |                   |        |
| Privacy and data protection    | Yes / No / Unknown |        |                   |        |
| Legal or regulatory compliance | Yes / No / Unknown |        |                   |        |
| Responsible AI or ethics       | Yes / No / Unknown |        |                   |        |
| Domain or safety expertise     | Yes / No / Unknown |        |                   |        |
| Accessibility and usability    | Yes / No / Unknown |        |                   |        |
| Operations and support         | Yes / No / Unknown |        |                   |        |

---

## 11. Reassessment Triggers

| Reassessment trigger                                         | Applicable?        | Required response or notes | Owner |
| ------------------------------------------------------------ | ------------------ | -------------------------- | ----- |
| Significant change in input data                             | Yes / No / Unknown |                            |       |
| Data drift or model degradation                              | Yes / No / Unknown |                            |       |
| Change to the AI model, prompt, configuration or fine-tuning | Yes / No / Unknown |                            |       |
| Change to system integration or business workflow            | Yes / No / Unknown |                            |       |
| New user groups, affected groups or usage patterns           | Yes / No / Unknown |                            |       |
| Production incident or harmful output                        | Yes / No / Unknown |                            |       |
| Regulatory, legal, security or compliance change             | Yes / No / Unknown |                            |       |
| Repeated user complaints or feedback patterns                | Yes / No / Unknown |                            |       |
| Change in acceptance criteria or risk tolerance              | Yes / No / Unknown |                            |       |
| Evidence that a previous assumption is no longer valid       | Yes / No / Unknown |                            |       |
| New or changed third-party dependency                        | Yes / No / Unknown |                            |       |

Reassessment does not always require repeating the complete assessment. The team should determine which risks, controls, evidence and decisions are affected by the change.

---

## 12. Review and Ownership

| Field                     | Description                                  |
| ------------------------- | -------------------------------------------- |
| Prepared by               |                                              |
| Assessment participants   |                                              |
| Reviewed by               |                                              |
| Risk decision owner       |                                              |
| Residual risk accepted by |                                              |
| Review date               |                                              |
| Next planned review       |                                              |
| Assessment status         | Draft / Under review / Approved / Superseded |
| Related decision records  |                                              |

---

## Notes

This template supports an initial and reviewable AI risk assessment.

It does not replace specialised security, privacy, legal, regulatory, safety or domain-specific risk assessments where these are required.

The depth of the assessment, strength of evidence and level of governance should be proportional to the risk associated with the AI system.
