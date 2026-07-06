# AI Glossary for Quality Assurance

## Purpose

This glossary provides a common vocabulary for Artificial Intelligence Quality Assurance.

Its objective is to define AI concepts from a Quality Engineering perspective, helping testers, developers, product owners and stakeholders use consistent terminology when designing, testing, validating, monitoring and governing AI systems.

The definitions are written for practical QA usage. They are not intended to replace formal definitions from standards, regulations or certification bodies.

The glossary should evolve together with the AI QA Framework.

---

## Contents

### A
### Agent

An AI system capable of autonomously planning, deciding and executing actions in order to achieve one or more objectives.

Unlike traditional AI assistants, agents may interact with external tools, retrieve information, execute workflows and make decisions based on their environment.

### Artificial Intelligence (AI)

The capability of computer systems to perform tasks that typically require human intelligence, such as reasoning, learning, problem-solving, language understanding and decision-making.

### AI Quality Assurance

AI Quality Assurance is the structured set of practices used to define, evaluate and provide evidence that an AI system behaves in a reliable, responsible and fit-for-purpose way across its lifecycle.

It includes more than testing model outputs. It also covers data quality, AI component behaviour, system integration, risk analysis, monitoring, governance and evidence-based decision-making.

### AI system

An AI system is a software system that uses one or more AI components to support decision-making, prediction, classification, generation, recommendation, automation or analysis.

In this framework, the term refers to the complete system, not only to the AI model.

Related term: AI-based system.

### AI-based system

AI-based system is used in this framework as an alternative term for AI system.

The preferred term is AI system, especially when referring to the complete system across its lifecycle.

### AI component

An AI component is a part of an AI system that provides AI-related capability.

Examples include a machine learning model, a generative AI model, a prompt-based component, a recommendation engine, a classification component, an AI service or a third-party AI capability integrated into a software system.

### AI QA Lifecycle

The AI QA Lifecycle describes how Quality Assurance activities can be applied across the lifecycle of an AI system.

It includes activities from problem and context understanding through data assessment, AI component validation, system testing, release readiness, operational monitoring and continuous improvement.

### AI-specific risk

An AI-specific risk is a quality, operational, ethical, security or governance risk that arises from the use of AI capabilities in a system.

Examples include data drift, model degradation, biased outputs, hallucination, lack of explainability, non-deterministic behaviour, overfitting, weak generalisation, prompt injection and unexpected behaviour in real-world conditions.

### Artefact

An artefact is a document, record, output or work product that provides evidence of a QA activity, decision, review or assessment.

Examples include test results, risk assessments, validation summaries, data quality reports, decision records, monitoring reports and known limitation logs.

### B

### Bias

Bias refers to systematic patterns in data, model behaviour, system design or operational use that may lead to unfair, inaccurate or harmful outcomes.

In AI QA, bias should be assessed through data analysis, model behaviour review, performance comparison across relevant groups or scenarios, and review of known limitations.

### C

### Continuous improvement

Continuous improvement refers to the ongoing use of evidence, feedback, monitoring results, incidents and reassessment findings to improve the AI system and the QA approach itself.

In AI QA, continuous improvement is important because data, usage patterns, operating conditions and model behaviour may change after release.

### Continuous quality

Continuous quality refers to the ability to observe, evaluate and maintain the acceptability of an AI system after deployment.

It includes monitoring, reassessment, incident review, feedback analysis and updates to quality controls.

### D

### Data quality

Data quality refers to the suitability of data used to train, validate, test, operate or monitor an AI system.

In AI QA, data quality includes aspects such as completeness, correctness, consistency, representativeness, relevance, timeliness and the presence of missing values, outliers or biased patterns.

### Data drift

Data drift occurs when the data received or used by an AI system changes over time in a way that may affect the behaviour or performance of the AI component.

Data drift can make previous validation evidence less reliable if the system is now operating under different data conditions.

### Decision record

A decision record is a documented explanation of an important decision, including the context, decision, rationale, supporting evidence, risks, owner and review trigger.

In this framework, decision records help make quality decisions explicit, traceable and reviewable.

### E

### Evidence

Evidence is information that supports a quality-related decision.

In AI QA, evidence may include test results, validation reports, data quality checks, risk assessments, monitoring outputs, defect records, known limitations, decision logs and specialist assessments.

### Evidence traceability

Evidence traceability refers to the ability to link quality evidence to the relevant requirement, risk, assumption, dataset, model, AI component, test, defect, decision or monitoring outcome.

Traceability helps explain why a quality decision was made and what information supported it.

### Explainability

Explainability refers to the ability to understand and communicate how an AI-supported output, recommendation or decision was produced.

In AI QA, explainability should be assessed according to the risk, impact and intended use of the AI system.

### F

### Fallback mechanism

A fallback mechanism is a predefined behaviour used when an AI component fails, produces an unreliable output, returns low confidence or cannot support the expected action safely.

Examples include asking for human review, using a rule-based alternative, blocking an automated action, showing a warning or escalating the case.

### Fairness

Fairness refers to the need to assess whether an AI system produces unfair, discriminatory or systematically harmful outcomes for specific individuals, groups or contexts.

Fairness cannot be assumed from overall model performance. It requires explicit analysis and evidence.

### G

### Governance

Governance refers to the structures, responsibilities, decision points and evidence expectations used to make quality decisions explicit, accountable, traceable and reviewable.

In AI QA, governance helps ensure that important decisions about risk, validation, release readiness and operational acceptability are not informal or undocumented.

### Governance checkpoint

A governance checkpoint is a defined point in the AI QA Lifecycle where evidence, risks, decisions or readiness are reviewed.

Examples include reviews during problem understanding, data assessment, validation, release readiness and operational monitoring.

### H

### Hallucination

Hallucination is an AI behaviour where a generative AI system produces content that appears plausible but is incorrect, unsupported, misleading or fabricated.

In QA, hallucination risk should be considered when AI-generated outputs may influence users, decisions, documents, recommendations or actions.

### Human oversight

Human oversight refers to the ability of people to understand, review, challenge, approve, override or intervene in AI-supported outputs, recommendations or actions.

The required level of human oversight depends on the risk, impact and intended use of the AI system.

### I

### Intended use

Intended use describes the purpose, context, users, expected outcomes and boundaries of an AI system.

In AI QA, intended use is important because quality criteria, risks, validation evidence and release decisions depend on how the system is expected to be used.

### J

### K

### L

### M

### Misuse risk

Misuse risk is the risk that an AI system, its data, its outputs or its capabilities may be used in an unintended, harmful, abusive or unsafe way.

In AI QA, misuse risk should be considered when defining test scenarios, controls, monitoring needs and release readiness evidence.

### Model behaviour

Model behaviour refers to how an AI model or AI component performs and responds under expected, unexpected and edge-case conditions.

In AI QA, model behaviour should be assessed through metrics, scenario-based testing, failure analysis, robustness checks, fairness review and explainability review where applicable.

### Model degradation

Model degradation occurs when the behaviour or performance of an AI model or AI component becomes worse over time.

It may be caused by data drift, changes in user behaviour, changes in the operating environment, outdated assumptions, system changes or new usage patterns.

### Monitoring

Monitoring refers to the ongoing observation of an AI system to detect changes, issues or risks that may affect its behaviour, performance or acceptability.

In AI QA, monitoring may include performance monitoring, data drift detection, model degradation detection, incident tracking, user feedback review, misuse indicators and reassessment triggers.

### N

### O

### Operational monitoring

Operational monitoring refers to the observation of an AI system after deployment or real-world use.

It may include monitoring of model performance, data drift, model degradation, incidents, user feedback, misuse indicators and reassessment triggers.

### P

### Privacy

Privacy refers to the protection of personal, sensitive or confidential information used, processed, generated or exposed by an AI system.

In AI QA, privacy concerns may include data minimisation, sensitive information leakage, access control, output exposure, logging practices and collaboration with privacy, legal or compliance specialists.

### Prompt injection

Prompt injection is a type of attack or misuse where input is crafted to manipulate the behaviour of a generative AI system.

It may cause the system to ignore instructions, reveal sensitive information, perform unintended actions or produce harmful outputs.

### Q

### Quality dimension

A quality dimension is an area of quality that should be considered when assessing an AI system.

In this framework, quality dimensions include data quality, model behaviour, system integration, reliability and robustness, explainability and transparency, fairness and bias, security and privacy, human oversight and monitoring.

### QA Decision Record

A QA Decision Record is a documented quality-related decision about an AI system.

It should normally include the context, decision, rationale, supporting evidence, known risks, owner and review trigger.

### R

### Release readiness

Release readiness refers to the evidence-based assessment of whether an AI system is acceptable for deployment or use.

In AI QA, release readiness should consider validation results, system testing, residual risks, known limitations, monitoring readiness, governance decisions and stakeholder acceptance.

### Reliability

Reliability refers to the ability of an AI system to behave consistently and acceptably under expected operating conditions.

In AI QA, reliability should be assessed together with robustness, monitoring evidence and known limitations.

### Reassessment trigger

A reassessment trigger is an event or condition that indicates the need to review previous quality decisions or validation evidence.

Examples include data drift, model degradation, incidents, changes in usage patterns, system changes, regulatory changes or new risk findings.

### Robustness

Robustness refers to the ability of an AI system or AI component to maintain acceptable behaviour under variable, unexpected or adverse conditions.

In AI QA, robustness may be assessed through input variation, edge cases, stress conditions, adversarial examples or real-world scenario testing.

### Residual risk

Residual risk is the risk that remains after controls, tests, mitigations or decisions have been applied.

In AI QA, residual risks should be visible, documented and considered during release readiness, risk acceptance and operational monitoring.

### S

### Security

Security refers to the protection of an AI system, its data, its components, its outputs and its users against unauthorised access, manipulation, exposure or harmful use.

In AI QA, security concerns may include prompt injection, adversarial inputs, insecure output handling, access control, logging and misuse monitoring.

### System integration

System integration refers to the way an AI component is connected with applications, APIs, user interfaces, workflows, monitoring tools and operational processes.

In AI QA, system integration testing should assess input and output handling, fallback mechanisms, logging, traceability, error handling and compatibility with existing workflows.

### System testing

System testing refers to the evaluation of the complete AI system in realistic workflows and operational conditions.

It goes beyond isolated model validation and considers how the AI component behaves within the broader software system.

### T

### Traceability

Traceability refers to the ability to link related quality information across requirements, risks, data, models, tests, defects, evidence, decisions and monitoring results.

In AI QA, traceability helps teams understand what was assessed, what evidence exists and why a quality decision was made.

### Transparency

Transparency refers to the ability to make relevant information about an AI system understandable, accessible and reviewable by appropriate stakeholders.

In AI QA, transparency may include documentation of intended use, assumptions, limitations, data sources, validation evidence, decision rationale and monitoring results.

### U

### Usability

Usability refers to the ability of users and stakeholders to understand, use and act upon AI-supported outputs appropriately.

In AI QA, usability is closely related to human oversight, interface clarity, confidence indicators, warnings, escalation paths and feedback mechanisms.

### V

### Validation

Validation refers to the assessment of whether an AI component or AI system is suitable for its intended use.

In AI QA, validation may include performance evaluation, scenario-based assessment, robustness testing, fairness review, explainability review and comparison against acceptance criteria.

### Vendor independence

Vendor independence means that the framework does not depend on a specific AI technology, tool, vendor, platform or development methodology.

In this framework, vendor independence helps keep QA principles, evidence expectations and governance practices reusable across different AI contexts.

### W

### X

### Y

### Z

---

## References

To be completed.