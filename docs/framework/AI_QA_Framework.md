# AI QA Framework

## What is AI Quality Assurance?

AI Quality Assurance is the structured set of practices used to define, evaluate and provide evidence that an AI-based system behaves in a reliable, responsible and fit-for-purpose way across its lifecycle.

In this framework, AI Quality Assurance is not limited to testing model outputs. It also includes understanding the problem context, identifying AI-specific risks, assessing data quality, validating model behaviour, evaluating system integration, monitoring operation and supporting informed decisions.

The goal is to make AI quality observable, testable and governable.

## 1. Purpose

The purpose of the AI QA Framework is to provide a practical and reusable approach for assuring the quality of systems that use Artificial Intelligence.

The framework helps Quality Assurance professionals, test leads, product teams and stakeholders understand what quality means in AI-based systems, identify relevant risks, define appropriate QA activities and collect evidence to support informed decisions.

It is designed to support quality activities across the AI system lifecycle, from early analysis and risk identification to testing, validation, monitoring and continuous improvement.

The framework is vendor-independent and is intended to be applicable across different AI technologies, domains and delivery contexts.

## 2. Scope

This framework applies to the Quality Assurance of systems that use Artificial Intelligence as part of their decision-making, prediction, classification, generation, recommendation or automation capabilities.

The framework supports QA activities across the AI system lifecycle, including problem understanding, data quality assessment, model validation, system testing, risk analysis, monitoring and continuous improvement.

It covers both model-level and system-level quality concerns. This includes the quality of data used by AI components, the behaviour of AI models, the integration of AI components into software systems, the risks introduced by probabilistic behaviour and the evidence required to support quality-related decisions.

This framework does not prescribe a specific AI technology, tool, vendor, platform or development methodology. It is designed to be adaptable to different contexts, including traditional machine learning systems, generative AI systems and AI-enabled software products.

The framework does not replace legal, regulatory, ethical or security assessments. Instead, it provides a QA-oriented structure that can support and complement those assessments when AI quality needs to be evaluated, tested, monitored and evidenced.

## 3. Framework Principles

The AI QA Framework is guided by a set of principles that define how quality should be approached in AI-based systems.

### 3.1 Quality must be defined in context

AI quality cannot be assessed in isolation from the problem, users, data, business process, operational environment and potential impact of the system.

The framework assumes that quality criteria should be defined according to the intended use of the AI system and the risks associated with incorrect, unstable, biased or unreliable behaviour.

### 3.2 QA must cover the full AI system, not only the model

AI Quality Assurance is not limited to validating model performance metrics.

The framework considers the complete AI-based system, including data, AI components, model behaviour, software integration, user interaction, monitoring, governance and evidence.

### 3.3 Evidence is required for quality decisions

Quality-related decisions should be supported by observable and reviewable evidence.

This may include test results, data quality checks, validation reports, risk assessments, monitoring outputs, defect records, decision logs and other artefacts that help explain why a system is considered acceptable or not acceptable.

### 3.4 AI-specific risks must be explicitly addressed

AI-based systems may introduce risks that are less common or less visible in traditional software systems.

These include data drift, model degradation, bias, lack of explainability, non-deterministic behaviour, hallucination, overfitting, weak generalisation and unexpected behaviour in real-world conditions.

### 3.5 The framework must remain vendor-independent

The framework does not depend on a specific AI platform, cloud provider, model, testing tool or development methodology.

It should be adaptable to different organisational contexts, technologies and levels of AI maturity.

### 3.6 QA should support continuous improvement

AI quality is not a one-time validation activity.

The framework assumes that AI systems may need ongoing monitoring, feedback analysis, reassessment and improvement after deployment, especially when data, usage patterns or operating conditions change.

## 4. AI System Quality Dimensions

AI-based systems should be assessed through multiple quality dimensions. These dimensions help QA teams identify what needs to be evaluated, tested, monitored and evidenced.

The dimensions below are intended to provide a practical structure for analysing AI quality. They may be adapted according to the type of system, level of risk, domain, regulatory context and organisational maturity.

### 4.1 Data Quality

Data quality refers to the suitability of the data used to train, validate, test, operate or monitor an AI system.

Relevant aspects include completeness, accuracy, consistency, representativeness, timeliness, missing values, outliers, imbalance, duplication and data drift.

Poor data quality can directly affect model behaviour, system reliability and the trustworthiness of AI-supported decisions.

### 4.2 Model Behaviour

Model behaviour refers to how the AI model performs and responds under expected, unexpected and edge-case conditions.

Relevant aspects include predictive performance, stability, generalisation, error patterns, sensitivity to input changes, robustness and behaviour across different user groups or operational scenarios.

Model behaviour should not be evaluated only through aggregate metrics. QA activities should also examine where, when and why the model fails.

### 4.3 System Integration

System integration refers to how AI components interact with the surrounding software system, data pipelines, user interfaces, APIs, business rules and operational processes.

Relevant aspects include input and output handling, integration points, fallback mechanisms, error handling, logging, traceability and compatibility with existing workflows.

An AI model may perform well in isolation but still introduce quality risks when integrated into a real system.

### 4.4 Reliability and Robustness

Reliability and robustness refer to the ability of the AI-based system to behave consistently and acceptably under normal, variable and adverse conditions.

Relevant aspects include resilience to noisy inputs, incomplete data, unexpected usage patterns, changing environments, model degradation and operational failures.

QA should consider both technical failures and quality degradation over time.

### 4.5 Explainability and Transparency

Explainability and transparency refer to the ability to understand, communicate and review how AI-supported outputs, recommendations or decisions are produced.

Relevant aspects include interpretability, traceability, documentation, decision rationale, limitations, assumptions and communication to stakeholders.

The required level of explainability depends on the impact, risk and intended use of the AI system.

### 4.6 Fairness and Bias

Fairness and bias refer to the need to identify and assess whether the AI system produces unfair, discriminatory or systematically harmful outcomes for specific individuals, groups or contexts.

Relevant aspects include dataset representativeness, biased historical patterns, performance differences across groups, proxy variables and unintended exclusion.

Fairness cannot be assumed from overall model performance. It requires explicit analysis and evidence.

### 4.7 Security, Privacy and Misuse Risk

Security, privacy and misuse risk refer to the protection of the AI system, its data, its outputs and its users against unauthorised access, exposure, manipulation or harmful use.

Relevant aspects include data protection, sensitive information leakage, prompt injection, adversarial inputs, model misuse, access control and monitoring of suspicious behaviour.

These concerns should be considered as part of AI quality because they may affect the trustworthiness and acceptability of the system.

Within this framework, these concerns are addressed from a QA perspective and may require collaboration with security, privacy, legal or compliance specialists.

### 4.8 Human Oversight and Usability

Human oversight and usability refer to the ability of users and stakeholders to understand, use, challenge, override or act upon AI-supported outputs appropriately.

Relevant aspects include user interface clarity, confidence indicators, escalation paths, human-in-the-loop controls, feedback mechanisms and the risk of automation bias.

AI quality depends not only on technical performance, but also on how people interact with and rely on the system.

### 4.9 Monitoring and Continuous Quality

Monitoring and continuous quality refer to the ability to observe the AI system after deployment and detect changes that may affect its behaviour or acceptability.

Relevant aspects include performance monitoring, data drift detection, model degradation, incident tracking, user feedback, retraining triggers and periodic reassessment.

AI systems may change in quality over time, even when the software itself has not changed.

## 5. AI QA Lifecycle

The AI QA Lifecycle describes how Quality Assurance activities can be applied across the lifecycle of an AI-based system.

The lifecycle is not intended to replace a delivery methodology. It can be adapted to agile, waterfall, hybrid, experimental or product-oriented contexts. Its purpose is to help QA teams identify when quality risks should be analysed, tested, monitored and evidenced.

### 5.1 Problem and Context Understanding

QA should start before data preparation or model development.

At this stage, the objective is to understand the problem the AI system is expected to support, the intended users, the operational context, the expected impact and the consequences of incorrect or unreliable behaviour.

Typical QA activities include:

- clarifying the intended use of the AI system;
- identifying stakeholders and affected users;
- defining initial quality expectations;
- identifying AI-specific and domain-specific risks;
- understanding business rules, constraints and acceptance expectations.

### 5.2 Data Assessment and Preparation

Data quality has a direct impact on AI system behaviour.

At this stage, QA activities focus on assessing whether the available data is suitable for the intended use of the AI system.

Typical QA activities include:

- reviewing data sources and data lineage;
- checking completeness, consistency and representativeness;
- identifying missing values, outliers, imbalance and duplication;
- assessing data drift risks;
- reviewing data preparation and transformation steps;
- documenting known data limitations.

### 5.3 AI Component Development and Validation

AI component development or configuration should be accompanied by validation activities that assess whether the component behaves adequately for its intended purpose.

At this stage, QA should not focus only on aggregate performance metrics or isolated output checks. It should also examine failure patterns, robustness, fairness, explainability and behaviour under relevant scenarios.

Typical QA activities include:

- reviewing model objectives and assumptions;
- validating performance metrics;
- analysing error patterns;
- testing behaviour with edge cases and boundary scenarios;
- assessing robustness and stability;
- reviewing explainability and limitations;
- comparing model behaviour against acceptance criteria.

### 5.4 System Integration and Testing

An AI component becomes part of a broader software system when it is integrated with applications, APIs, user interfaces, workflows, monitoring tools and operational processes.

At this stage, QA activities focus on verifying that the AI component works correctly within the complete system.

Typical QA activities include:

- testing input and output handling;
- validating integration with upstream and downstream systems;
- checking fallback mechanisms and error handling;
- testing user interaction with AI-supported outputs;
- verifying logging, traceability and auditability;
- validating end-to-end workflows;
- assessing non-functional quality attributes affected by AI behaviour.

### 5.5 Acceptance and Release Readiness

Before release, QA should support an evidence-based decision on whether the AI-based system is acceptable for deployment.

At this stage, the focus is not only on whether tests passed, but on whether the remaining risks are understood, documented and acceptable.

Typical QA activities include:

- reviewing test evidence;
- assessing open defects and known limitations;
- validating acceptance criteria;
- reviewing risk assessments;
- confirming monitoring requirements;
- documenting release recommendations;
- supporting go/no-go decisions.

### 5.6 Deployment and Operational Monitoring

AI quality may change after deployment due to changes in data, user behaviour, environment, business processes or external conditions.

At this stage, QA activities focus on observing whether the system continues to behave acceptably in real use.

Typical QA activities include:

- monitoring model performance;
- detecting data drift and model degradation;
- reviewing production incidents;
- analysing user feedback;
- checking unexpected or harmful outputs;
- validating alerts and escalation mechanisms;
- reviewing operational evidence.

### 5.7 Continuous Improvement

AI QA should support ongoing improvement after deployment.

At this stage, evidence collected from monitoring, incidents, feedback and reassessment should be used to improve the AI system and its quality controls.

Typical QA activities include:

- reviewing lessons learned;
- updating risk assessments;
- refining test scenarios;
- reassessing data and model quality;
- supporting retraining or recalibration decisions;
- improving monitoring rules;
- updating documentation and governance artefacts.

## 6. QA Activities by Lifecycle Stage

_To be drafted._

## 7. Evidence and Artefacts

_To be drafted._

## 8. Roles and Responsibilities

_To be drafted._

## 9. Governance and Decision Records

_To be drafted._

## 10. References and Influences

_To be drafted._
