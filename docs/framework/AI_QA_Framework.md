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

This section maps practical QA activities to the AI QA Lifecycle defined in the previous section.

The activities are not intended to be exhaustive or mandatory in every project. They should be selected and adapted according to the system context, risk level, AI technology, delivery model, available evidence and organisational maturity.

The activities can be applied to different AI contexts, including traditional Machine Learning models, Generative AI solutions, AI components provided by third parties and AI-enabled software products.

The purpose of this section is to help QA teams understand what can be assessed, tested, reviewed or monitored at each stage of the lifecycle.

### 6.1 Problem and Context Understanding

At this stage, QA helps clarify what the AI-based system is expected to do, who may be affected by it and what quality risks should be considered from the beginning.

#### QA Focus

- Understand the intended use of the AI-based system.
- Identify users, stakeholders and affected groups.
- Clarify expected outcomes and unacceptable behaviours.
- Identify early AI-specific risks.
- Define initial quality expectations.

#### Typical QA Activities

- Review the problem statement and intended use.
- Identify critical decisions or outputs supported by AI.
- Analyse possible consequences of incorrect, biased, unstable or misleading behaviour.
- Review assumptions about users, data, environment and system constraints.
- Support the definition of quality attributes relevant to the AI-based system.
- Identify initial acceptance criteria.
- Identify regulatory, ethical, security or operational concerns that may require specialist input.

#### Expected Evidence

- Problem statement review notes.
- Intended use description.
- Initial risk assessment.
- Stakeholder and user mapping.
- Initial quality expectations.
- Initial acceptance criteria.
- Assumption and constraint log.

### 6.2 Data Assessment and Preparation

At this stage, QA evaluates whether the data used by the AI-based system is suitable for its intended purpose.

#### QA Focus

- Assess the quality and suitability of data.
- Identify data limitations and risks.
- Check whether data preparation steps are controlled and documented.
- Support traceability between data, model behaviour and system quality.

#### Typical QA Activities

- Review data sources, ownership and lineage.
- Check data completeness, consistency and validity.
- Identify missing values, outliers, duplicates and imbalance.
- Assess whether the data is representative of the intended use context.
- Review data labelling or annotation quality, when applicable.
- Review data cleaning, transformation and feature engineering steps.
- Check for potential data leakage.
- Identify data drift risks.
- Document known data limitations and their possible impact.

#### Expected Evidence

- Data quality assessment results.
- Data profiling reports.
- Data lineage documentation.
- Data preparation review notes.
- Missing values and outlier analysis.
- Data limitation log.
- Data leakage checks.
- Data drift risk notes.

### 6.3 AI Component Development and Validation

At this stage, QA evaluates whether the AI component behaves adequately for its intended purpose before it is integrated into the wider system.

#### QA Focus

- Validate AI component behaviour.
- Assess whether performance is acceptable for the intended use.
- Analyse failures and limitations.
- Check robustness, fairness and explainability concerns.
- Ensure validation evidence is understandable and reviewable.

#### Typical QA Activities

- Review AI component objectives and assumptions.
- Review selected metrics and their relevance to the problem.
- Validate model or component performance against acceptance criteria.
- Analyse error patterns and failure cases.
- Test behaviour using representative, edge-case and adverse scenarios.
- Assess robustness to input variation.
- Review explainability outputs or reasoning traces, when applicable.
- Compare behaviour across relevant user groups, segments or scenarios.
- Review known limitations and residual risks.
- Validate configuration, prompting, fine-tuning or model selection decisions, when applicable.

#### Expected Evidence

- Validation results.
- Metric analysis.
- Error analysis.
- Edge-case test results.
- Robustness assessment.
- Fairness or bias assessment, when applicable.
- Explainability review notes.
- Known limitation log.
- Validation summary.

### 6.4 System Integration and Testing

At this stage, QA evaluates whether the AI component works correctly as part of the complete software system.

#### QA Focus

- Validate integration between AI components and the surrounding system.
- Check end-to-end behaviour.
- Verify input and output handling.
- Assess error handling, fallback mechanisms and traceability.
- Confirm that users can interact with AI-supported outputs appropriately.

#### Typical QA Activities

- Test integration points with upstream and downstream systems.
- Validate API contracts, data formats and response handling.
- Test input validation and output interpretation.
- Check fallback mechanisms when the AI component fails or produces low-confidence outputs.
- Test error handling, logging and alerting.
- Validate user interface behaviour for AI-supported outputs.
- Test end-to-end workflows involving AI decisions, predictions, recommendations or generated content.
- Check traceability between input, AI output, system action and user-visible result.
- Assess non-functional behaviour affected by the AI component, such as performance, reliability and maintainability.

#### Expected Evidence

- Integration test results.
- End-to-end test results.
- API and interface validation results.
- Error handling test results.
- Fallback mechanism test results.
- Logging and traceability checks.
- User workflow test evidence.
- Defect records.

### 6.5 Acceptance and Release Readiness

At this stage, QA supports an evidence-based decision on whether the AI-based system is ready for release.

#### QA Focus

- Consolidate quality evidence.
- Assess whether acceptance criteria are met.
- Review open risks, defects and limitations.
- Support release decisions with clear recommendations.
- Confirm monitoring and operational readiness.

#### Typical QA Activities

- Review test coverage and test results.
- Review validation evidence from data, AI component and system testing activities.
- Assess open defects and unresolved risks.
- Review known limitations and their expected impact.
- Confirm that acceptance criteria have been evaluated.
- Confirm that monitoring requirements are defined.
- Confirm that fallback, escalation and incident handling mechanisms are ready.
- Prepare a QA release recommendation.
- Support go/no-go decision-making.

#### Expected Evidence

- Test summary report.
- Validation summary.
- Risk assessment update.
- Open defect and limitation log.
- Acceptance criteria review.
- Monitoring readiness checklist.
- QA release recommendation.
- Go/no-go decision record.

### 6.6 Deployment and Operational Monitoring

At this stage, QA supports the observation of the AI-based system in real use.

#### QA Focus

- Monitor whether the system continues to behave acceptably after deployment.
- Detect degradation, drift, incidents or unexpected behaviour.
- Review operational evidence.
- Support timely response to quality issues.

#### Typical QA Activities

- Review production monitoring outputs.
- Monitor model or AI component performance.
- Monitor data drift and changes in input patterns.
- Track incidents, defects and user feedback.
- Review low-confidence, unexpected or harmful outputs.
- Check whether alerts and escalation mechanisms work as expected.
- Compare production behaviour with validation assumptions.
- Review whether retraining, recalibration or configuration changes may be needed.
- Support post-release quality reviews.

#### Expected Evidence

- Monitoring dashboards or reports.
- Data drift reports.
- Model degradation indicators.
- Incident records.
- User feedback analysis.
- Alert and escalation records.
- Production quality review notes.
- Post-release assessment results.

### 6.7 Continuous Improvement

At this stage, QA uses evidence collected across the lifecycle to improve the AI-based system and the QA approach itself.

#### QA Focus

- Learn from production behaviour, incidents and feedback.
- Improve quality controls.
- Update tests, risks and documentation.
- Support controlled change and reassessment.

#### Typical QA Activities

- Review lessons learned from testing, release and operation.
- Update risk assessments based on new evidence.
- Refine test scenarios and acceptance criteria.
- Update data quality checks.
- Review whether model, prompt, configuration or system changes require reassessment.
- Support regression testing after AI-related changes.
- Review the effectiveness of monitoring rules and thresholds.
- Update documentation, decision records and governance artefacts.
- Identify improvements to the QA process.

#### Expected Evidence

- Lessons learned.
- Updated risk assessment.
- Updated test scenarios.
- Regression test results.
- Updated monitoring rules.
- Change assessment notes.
- Updated documentation.
- Improvement backlog.

## 7. Evidence and Artefacts

Evidence and artefacts are central to the AI QA Framework because they make quality decisions observable, reviewable and traceable.

In AI-based systems, QA should not rely only on final test results or model performance metrics. Quality evidence should show how the system was understood, what risks were identified, what was tested, what limitations are known, what decisions were made and whether the system continues to behave acceptably after deployment.

The artefacts described in this section are not mandatory in every project. They should be selected according to the system context, risk level, lifecycle stage, regulatory expectations, delivery model and organisational maturity.

### 7.1 Evidence Principles

QA evidence should follow a small set of principles.

#### Traceable

Evidence should be linked to the relevant requirement, risk, assumption, dataset, model, AI component, test, defect, decision or monitoring outcome.

Traceability helps explain why a quality decision was made and what information supported it.

#### Reviewable

Evidence should be understandable by the people who need to review or use it.

This may include QA teams, developers, data scientists, product owners, business stakeholders, auditors, security teams, compliance teams or operational teams.

#### Risk-based

The level of evidence should be proportional to the level of risk.

High-impact AI-based systems should require stronger evidence than low-risk internal tools or experimental prototypes.

#### Current

Evidence should be kept up to date when the AI-based system, data, model, configuration, prompt, integration, usage pattern or operating environment changes.

Outdated evidence can create false confidence.

#### Decision-oriented

Evidence should support decisions.

The goal is not to produce documentation for its own sake, but to support informed decisions about quality, release readiness, risk acceptance, monitoring, reassessment and continuous improvement.

### 7.2 Core Artefact Categories

The framework groups artefacts into categories that support different QA concerns across the AI lifecycle.

### 7.2.1 Context and Risk Artefacts

Context and risk artefacts help clarify why the AI-based system exists, how it is expected to be used and what could go wrong.

Typical artefacts include:

- problem statement;
- intended use description;
- stakeholder and user mapping;
- initial quality expectations;
- assumption and constraint log;
- AI-specific risk assessment;
- domain-specific risk assessment;
- acceptance criteria;
- decision logs.

These artefacts are especially relevant during problem understanding, planning, acceptance and release readiness.

### 7.2.2 Data Quality Artefacts

Data quality artefacts provide evidence about the suitability, limitations and risks of the data used by the AI-based system.

Typical artefacts include:

- data source inventory;
- data lineage documentation;
- data profiling results;
- missing values analysis;
- outlier analysis;
- data imbalance analysis;
- data duplication checks;
- data leakage checks;
- data preparation review notes;
- data limitation log;
- data drift risk notes.

These artefacts help QA teams understand whether data issues may affect model behaviour, system reliability or user trust.

### 7.2.3 AI Component Validation Artefacts

AI component validation artefacts provide evidence about the behaviour, performance and limitations of the AI component before or during system integration.

Typical artefacts include:

- validation plan;
- metric selection rationale;
- validation results;
- error analysis;
- edge-case test results;
- robustness assessment;
- fairness or bias assessment;
- explainability review notes;
- prompt, configuration or fine-tuning review notes, when applicable;
- known limitation log;
- validation summary.

These artefacts help determine whether the AI component behaves adequately for its intended purpose.

### 7.2.4 System Testing Artefacts

System testing artefacts provide evidence about how the AI component behaves as part of the complete software system.

Typical artefacts include:

- integration test cases;
- end-to-end test cases;
- API and interface validation results;
- input and output handling test results;
- fallback mechanism test results;
- error handling test results;
- logging and traceability checks;
- user workflow test evidence;
- non-functional test evidence;
- defect records.

These artefacts help determine whether the AI-based system works acceptably in realistic workflows and operational conditions.

### 7.2.5 Release and Acceptance Artefacts

Release and acceptance artefacts support the decision on whether the AI-based system is ready to be released or used.

Typical artefacts include:

- test summary report;
- validation summary;
- updated risk assessment;
- open defect and limitation log;
- acceptance criteria review;
- monitoring readiness checklist;
- QA release recommendation;
- go/no-go decision record;
- risk acceptance record.

These artefacts should make release decisions transparent and based on evidence rather than assumptions.

### 7.2.6 Monitoring and Operational Artefacts

Monitoring and operational artefacts provide evidence about the behaviour of the AI-based system after deployment.

Typical artefacts include:

- monitoring dashboards or reports;
- data drift reports;
- model or AI component degradation indicators;
- incident records;
- user feedback analysis;
- alert and escalation records;
- production quality review notes;
- post-release assessment results;
- retraining, recalibration or configuration change records.

These artefacts help determine whether the system continues to behave acceptably in real use.

### 7.2.7 Continuous Improvement Artefacts

Continuous improvement artefacts support learning and controlled evolution of the AI-based system and the QA approach.

Typical artefacts include:

- lessons learned;
- updated risk assessment;
- updated test scenarios;
- regression test results;
- updated monitoring rules;
- change assessment notes;
- updated documentation;
- improvement backlog;
- updated decision records.

These artefacts help ensure that quality evidence leads to improvement rather than remaining static documentation.

### 7.3 Minimum Evidence Set

Not every project needs every artefact. However, for a first version of the framework, a minimum evidence set should normally include:

- intended use description;
- AI-specific risk assessment;
- data quality assessment;
- AI component validation summary;
- system test evidence;
- known limitations;
- QA release recommendation;
- monitoring approach, when the system is deployed or used operationally.

For higher-risk systems, this minimum evidence set should be expanded with stronger traceability, more detailed validation, fairness and bias analysis, explainability evidence, security and privacy input, operational monitoring and formal decision records.

### 7.4 Evidence Traceability

Evidence should not be isolated across documents, tools or teams.

Where possible, QA teams should maintain traceability between:

- intended use and acceptance criteria;
- risks and QA activities;
- data issues and validation results;
- validation findings and known limitations;
- test results and release recommendations;
- incidents and continuous improvement actions;
- monitoring results and reassessment decisions.

Traceability does not need to be complex at the beginning. It can start with simple links between documents, tables, issues, test cases, risks and decisions.

The important point is that quality decisions should be explainable from the evidence available.

### 7.5 Artefact Ownership

Artefacts may be created by different roles, but QA should help ensure that relevant evidence exists, is reviewable and supports quality decisions.

Possible ownership examples include:

- product teams owning intended use, business context and acceptance expectations;
- data teams owning data lineage, data preparation and data quality evidence;
- data scientists or AI engineers owning model or AI component validation evidence;
- QA teams owning test evidence, defect records, QA review notes and release recommendations;
- security, privacy, legal or compliance specialists owning specialist assessments;
- operations or support teams owning monitoring, incident and post-release evidence.

Ownership may vary by organisation. The framework does not prescribe a fixed ownership model, but it assumes that evidence responsibilities should be explicit.

## 8. Roles and Responsibilities

AI Quality Assurance is a shared responsibility. Although QA teams play a central role in defining, assessing, testing and evidencing quality, they cannot assure AI quality alone.

AI-based systems usually involve product decisions, data decisions, model or AI component decisions, software engineering, operational monitoring, governance and specialist assessments. The responsibilities described in this section are intended to clarify collaboration, not to prescribe a fixed organisational structure.

The same person or team may cover multiple responsibilities depending on the organisation, project size and level of AI maturity.

### 8.1 Quality Assurance

QA is responsible for helping make AI quality observable, testable, reviewable and evidence-based.

Typical responsibilities include:

- supporting the definition of quality expectations and acceptance criteria;
- identifying AI-specific quality risks;
- reviewing testability of AI-based system behaviour;
- defining QA activities across the AI lifecycle;
- designing and executing test activities;
- reviewing data, model, integration and system-level evidence;
- analysing defects, limitations and residual risks;
- supporting release readiness decisions;
- ensuring that quality evidence is documented and traceable;
- supporting monitoring and continuous improvement activities.

QA should act as a critical reviewer of quality evidence, not only as a test execution function.

### 8.2 Product and Business Stakeholders

Product and business stakeholders are responsible for defining why the AI-based system exists, what value it should provide and what outcomes are acceptable or unacceptable.

Typical responsibilities include:

- defining the problem, business objective and intended use;
- identifying users, affected groups and operational context;
- clarifying expected outcomes and business rules;
- defining acceptance expectations;
- identifying business risks and impact;
- reviewing known limitations and residual risks;
- participating in release readiness and risk acceptance decisions.

Product and business stakeholders should ensure that AI quality is assessed against real use, not only technical performance.

### 8.3 Data Roles

Data roles are responsible for the quality, suitability, preparation and governance of data used by the AI-based system.

Depending on the organisation, these responsibilities may be covered by data engineers, data analysts, data scientists, data stewards or data governance teams.

Typical responsibilities include:

- documenting data sources and data lineage;
- assessing data completeness, consistency, accuracy and representativeness;
- identifying missing values, outliers, imbalance, duplication and leakage risks;
- documenting data preparation and transformation steps;
- supporting data quality checks;
- identifying data limitations and possible impact;
- supporting monitoring for data drift or changes in input patterns.

Data roles should provide evidence that allows QA and stakeholders to understand how data quality may affect AI behaviour.

### 8.4 AI Engineering and Data Science

AI engineering and data science roles are responsible for the design, configuration, validation and evolution of AI components.

Depending on the context, this may include developing models, selecting third-party models, configuring AI services, designing prompts, fine-tuning models or validating AI component behaviour.

Typical responsibilities include:

- defining AI component objectives and assumptions;
- selecting models, techniques, prompts or configurations;
- selecting relevant evaluation metrics;
- validating AI component behaviour;
- analysing errors, limitations and failure patterns;
- assessing robustness, fairness and explainability where applicable;
- documenting model, prompt, configuration or fine-tuning decisions;
- supporting reassessment after changes or degradation;
- collaborating with QA on test scenarios and validation evidence.

AI engineering and data science roles should make AI component behaviour understandable and reviewable by other stakeholders.

### 8.5 Software Engineering

Software engineering roles are responsible for integrating AI components into the broader software system.

Typical responsibilities include:

- implementing system integration with AI components;
- managing APIs, data flows and dependencies;
- implementing input validation and output handling;
- implementing fallback mechanisms and error handling;
- supporting logging, traceability and observability;
- ensuring maintainability, reliability and performance of the system;
- supporting automated checks where appropriate;
- fixing defects identified during QA activities.

Software engineering should ensure that the AI component works safely and reliably within the complete system, not only in isolation.

### 8.6 Security, Privacy, Legal and Compliance Specialists

Specialist roles are responsible for assessing concerns that require specific expertise beyond general QA.

These roles may include security teams, privacy specialists, legal advisors, compliance officers, risk managers or ethics reviewers.

Typical responsibilities include:

- assessing security risks related to AI components, data and integrations;
- reviewing privacy and data protection concerns;
- assessing legal, regulatory or contractual obligations;
- reviewing misuse, abuse or harmful use scenarios;
- advising on auditability, explainability and accountability expectations;
- supporting risk acceptance or escalation decisions;
- providing specialist evidence for release and governance decisions.

The AI QA Framework does not replace specialist assessments. QA should collaborate with these roles and ensure that relevant specialist evidence is considered in quality decisions.

### 8.7 Operations and Support

Operations and support roles are responsible for observing and supporting the AI-based system after deployment.

Typical responsibilities include:

- monitoring production behaviour;
- reviewing alerts, incidents and user feedback;
- tracking operational failures or quality degradation;
- supporting escalation and incident handling;
- maintaining monitoring dashboards or reports;
- identifying patterns that may indicate data drift, model degradation or misuse;
- supporting post-release quality reviews;
- feeding operational evidence into continuous improvement activities.

Operations and support teams help determine whether the AI-based system continues to behave acceptably in real use.

### 8.8 Governance and Decision-Making

Governance responsibilities ensure that quality decisions are explicit, evidence-based and accountable.

These responsibilities may be covered by product leadership, delivery leadership, architecture boards, risk committees, governance forums or designated decision owners.

Typical responsibilities include:

- defining decision-making authority;
- reviewing quality evidence and residual risks;
- approving or rejecting release recommendations;
- accepting, escalating or mitigating risks;
- ensuring that decision records are maintained;
- reviewing whether monitoring and reassessment obligations are met;
- ensuring alignment with organisational policies and external obligations.

Governance should ensure that AI quality decisions are not informal, undocumented or based only on technical metrics.

### 8.9 Responsibility Matrix

The table below provides a simplified view of how responsibilities may be distributed.

| Area | Primary Responsibility | Supporting Roles |
|---|---|---|
| Intended use and business context | Product and Business Stakeholders | QA, Governance |
| Quality expectations and acceptance criteria | Product and Business Stakeholders | QA, AI Engineering, Software Engineering |
| AI-specific risk identification | QA | Product, Data Roles, AI Engineering, Security, Compliance |
| Data quality evidence | Data Roles | QA, AI Engineering |
| AI component validation | AI Engineering and Data Science | QA, Product, Data Roles |
| System integration and testing | Software Engineering and QA | AI Engineering, Product |
| Security and privacy assessment | Security and Privacy Specialists | QA, Software Engineering, Data Roles |
| Release readiness recommendation | QA | Product, AI Engineering, Software Engineering, Operations |
| Risk acceptance and go/no-go decision | Governance and Decision Owners | QA, Product, Specialist Roles |
| Operational monitoring | Operations and Support | QA, AI Engineering, Software Engineering |
| Continuous improvement | Product and Delivery Teams | QA, Operations, AI Engineering, Data Roles |

This matrix should be adapted to each organisation. Its purpose is to make responsibilities explicit, not to impose a fixed delivery model.

## 9. Governance and Decision Records

Governance in the AI QA Framework ensures that quality decisions are explicit, evidence-based, traceable and reviewable.

AI-based systems may introduce uncertainty, probabilistic behaviour, data dependency, model degradation, bias, explainability limitations and operational risks. For this reason, important quality decisions should not remain informal or undocumented.

Governance does not mean adding unnecessary bureaucracy. Its purpose is to ensure that relevant decisions are made by the right people, using appropriate evidence, with clear ownership and review points.

### 9.1 Governance Objectives

The governance approach in this framework has five main objectives:

- ensure that AI quality decisions are based on evidence;
- clarify who is responsible for making and approving decisions;
- document the rationale behind important decisions;
- make risks, limitations and assumptions visible;
- support reassessment when the system, data, model, context or risk changes.

Governance should help teams answer a simple question:

> Why was this AI-based system considered acceptable, and what evidence supported that decision?

### 9.2 Governance Principles

AI QA governance should follow a set of practical principles.

#### Evidence-based

Quality decisions should be supported by evidence such as test results, validation summaries, risk assessments, data quality checks, monitoring outputs, defect records and known limitation logs.

#### Risk-based

The level of governance should be proportional to the level of risk.

Higher-risk AI-based systems should require stronger evidence, more formal reviews and clearer decision records.

#### Traceable

Important decisions should be linked to the evidence, risks, assumptions, artefacts or lifecycle stage that supported them.

Traceability helps teams explain and review past decisions.

#### Accountable

Decision ownership should be explicit.

It should be clear who reviewed the evidence, who accepted the residual risk and who approved release or continued operation.

#### Reviewable

Governance decisions should be revisited when relevant changes occur.

AI quality may change over time due to data drift, model degradation, configuration changes, prompt changes, new usage patterns, incidents or external changes.

### 9.3 Decisions That Should Be Recorded

Not every operational detail needs a formal decision record. However, the following decisions should normally be recorded when they affect quality, risk, release readiness or operational acceptability.

#### Intended Use Decisions

Examples include:

- approval of the intended use of the AI-based system;
- confirmation of the target users or affected groups;
- agreement on unacceptable uses or out-of-scope scenarios;
- approval of assumptions and constraints.

#### Quality and Risk Decisions

Examples include:

- acceptance of quality criteria;
- prioritisation of AI-specific risks;
- acceptance of known data limitations;
- acceptance of model or AI component limitations;
- acceptance of fairness, explainability, robustness or monitoring limitations.

#### Validation and Testing Decisions

Examples include:

- approval of selected validation metrics;
- acceptance of validation results;
- acceptance of test coverage limitations;
- approval of unresolved defects or residual risks;
- decision to perform additional testing or reassessment.

#### Release Readiness Decisions

Examples include:

- QA release recommendation;
- go/no-go decision;
- risk acceptance decision;
- approval of monitoring readiness;
- approval of fallback or escalation mechanisms.

#### Operational Decisions

Examples include:

- decision to continue operation after an incident;
- decision to retrain, recalibrate, reconfigure or replace an AI component;
- decision to update monitoring thresholds;
- decision to restrict usage;
- decision to rollback or disable AI-supported functionality.

### 9.4 Decision Record Structure

Decision records should be short, practical and easy to review.

A decision record should normally include:

| Field | Description |
|---|---|
| Title | Short name of the decision |
| Date | Date when the decision was made |
| Status | Proposed, Accepted, Rejected, Superseded or Under Review |
| Context | Why the decision was needed |
| Decision | What was decided |
| Rationale | Why this option was selected |
| Evidence | Evidence used to support the decision |
| Risks and Limitations | Known residual risks, limitations or assumptions |
| Owner | Person, role or group accountable for the decision |
| Review Trigger | Conditions that should cause the decision to be revisited |

The structure may be adapted to the organisation, but the decision should remain understandable without requiring informal knowledge.

### 9.5 Architecture Decision Records and QA Decision Records

This framework distinguishes between two related types of decision records.

#### Architecture Decision Records

Architecture Decision Records document structural or architectural decisions about the framework, repository, design approach or technical direction.

Examples include:

- repository structure decisions;
- documentation structure decisions;
- framework design decisions;
- lifecycle or taxonomy decisions;
- tooling or format decisions.

In this repository, Architecture Decision Records are stored under:

```text
docs/adr/
```

#### QA Decision Records

QA Decision Records document quality-related decisions about an AI-based system being assessed with the framework.

Examples include:

- acceptance of a known model limitation;
- approval of a release recommendation;
- acceptance of residual risk;
- decision to require additional monitoring;
- decision to reassess after data drift;
- decision to reject release readiness.

QA Decision Records may be stored in a project-specific location, test management tool, governance tool or documentation repository, depending on the organisation.

### 9.6 Governance Checkpoints Across the AI QA Lifecycle

Governance should be applied at meaningful points across the lifecycle, not only at release time.

| Lifecycle Stage | Governance Focus |
|---|---|
| Problem and Context Understanding | Confirm intended use, stakeholders, impact and initial risks |
| Data Assessment and Preparation | Review data suitability, limitations and lineage |
| AI Component Development and Validation | Review validation approach, metrics, behaviour and limitations |
| System Integration and Testing | Review system-level quality evidence and unresolved defects |
| Acceptance and Release Readiness | Review QA recommendation, residual risks and go/no-go decision |
| Deployment and Operational Monitoring | Review production behaviour, incidents and monitoring evidence |
| Continuous Improvement | Review lessons learned, reassessment needs and improvement actions |

These checkpoints help ensure that quality is governed throughout the lifecycle rather than inspected only at the end.

### 9.7 Reassessment Triggers

Some decisions should be reviewed when relevant changes occur.

Typical reassessment triggers include:

- significant changes in input data;
- data drift or model degradation;
- changes to the AI model, prompt, configuration or fine-tuning;
- changes to system integration or business workflow;
- new user groups or usage patterns;
- production incidents or harmful outputs;
- regulatory, legal, security or compliance changes;
- repeated user complaints or feedback patterns;
- changes in acceptance criteria or risk tolerance;
- evidence that previous assumptions are no longer valid.

Reassessment does not always mean repeating all previous QA activities. It means determining what needs to be reviewed, retested, monitored or reapproved based on the change and associated risk.

### 9.8 Governance Outputs

Governance activities should produce clear outputs that can support accountability and future review.

Typical outputs include:

- decision records;
- risk acceptance records;
- release readiness decisions;
- monitoring review notes;
- reassessment decisions;
- change impact assessments;
- escalation records;
- updated assumptions and limitations;
- updated governance or QA recommendations.

The goal is to ensure that important AI quality decisions can be explained later using available evidence.

### 9.9 Practical Governance Guidance

The governance approach should remain proportional.

For low-risk prototypes or internal experiments, lightweight decision notes may be sufficient.

For high-impact AI-based systems, governance may require formal review boards, stronger evidence, specialist assessments, approval workflows and periodic reassessment.

The AI QA Framework does not prescribe a single governance model. It provides a structure that helps teams decide what should be reviewed, who should decide, what evidence is needed and when decisions should be revisited.

## 10. References and Influences

_To be drafted._
