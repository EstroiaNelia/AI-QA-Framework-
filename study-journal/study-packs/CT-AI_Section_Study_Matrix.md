# CT-AI Section Study Matrix

## Purpose

This matrix supports section-based revision for the ISTQB Certified Tester AI Testing (CT-AI) exam.

It is based on the practice questions already transcribed from the uploaded Word files. The goal is to track weak areas, focus revision, and move each syllabus area from below-pass level to exam-ready level.

## Scoring rule

Use the following status after each practice attempt:

| Score | Status | Meaning |
|---:|---|---|
| < 65% | Red | Below pass level. Needs focused revision. |
| 65%–79% | Amber | Pass level reached, but not stable enough. |
| >= 80% | Green | Exam-ready target level. |

Current baseline: all section-based attempts were below 65%, so all areas start as Red.

---

## Main Study Matrix

| Priority | Syllabus area | Source questions | Main topics | Current status | Revision objective | Study action | Output to produce |
|---|---|---|---|---|---|---|---|
| P2 | 1.1–1.9 | Questions_63_1, Q1–Q45 | Definition of AI, AI Effect, narrow/general/super AI, conventional vs AI-based systems, AI technologies, frameworks, hardware, AIaaS, pre-trained models, standards and regulation | Red | Stabilise the basic CT-AI vocabulary and avoid confusing AI concepts with ML implementation details | Review definitions and create short flashcards for each concept | Chapter 1 flashcards and wrong-answer notes |
| P2 | 2.1–2.8 | Questions_63_1, Q46–Q63 | Flexibility, adaptability, autonomy, bias, ethics, side effects, XAI, safety | Red | Distinguish AI quality characteristics and understand their testing implications | Build a comparison table for quality characteristics | Chapter 2 comparison table |
| P1 | 3.1–3.5 | Questions_36_2, Q1–Q20 | Supervised, unsupervised and reinforcement learning, ML workflow, objectives, data preparation, hyperparameters, tuning, underfitting | Red | Understand the ML workflow and distinguish learning types | Draw the ML workflow and map each activity to its purpose | ML workflow one-page summary |
| P1 | 4.1–4.5.1 | Questions_36_2, Q21–Q36 | Data preparation, data pre-processing, data augmentation, feature selection, datasets, data quality, wrong/unfair/obsolete data, labelling | Red | Consolidate data-related concepts because they affect many CT-AI questions | Create a data quality glossary with examples | Data quality study sheet |
| P1 | 5.1–5.5 | Questions_38_3, Q1–Q15 | Accuracy, Precision, Recall, F1-score, ROC, AUC, R-squared, benchmark suites | Red | Select the correct metric based on risk and problem type | Practise confusion matrix scenarios and metric-selection questions | Metrics decision table |
| P2 | 6.1–6.2 | Questions_38_3, Q16–Q23 | Neural networks, perceptron, deep neural networks, activation values, neural network coverage criteria | Red | Understand neural-network terminology sufficiently for exam questions | Create a minimal neural-network glossary | Neural networks flashcards |
| P1 | 7.1–7.7 | Questions_38_3, Q24–Q38 | Requirements, AI component testing, input data testing, component integration, system testing, masked defects, automation/complacency bias, documentation, concept drift | Red | Understand how AI testing differs from conventional testing across test levels | Build a test-level comparison table | Chapter 7 testing levels map |
| P0 | 8.1–8.8 | Questions_45_4, Q1–Q26 | Self-learning systems, autonomy testing, bias testing, probabilistic systems, test oracle problem, complexity, explainability, correctness, AI quality characteristics | Red | Recover the weakest area: testing challenges specific to AI-based systems | Study one subtopic per day and answer short scenario questions | Chapter 8 recovery pack |
| P0 | 9.1.1–9.7 | Questions_45_4, Q27–Q45 | Adversarial attacks, data poisoning, exhaustive/combinatorial testing, pairwise testing, back-to-back testing, pseudo-oracle, A/B testing, metamorphic testing, experience-based testing, EDA, test oracle mitigation | Red | Master AI-specific test techniques and distinguish similar techniques in exam scenarios | Create comparison tables and exam traps for each technique | Chapter 9 technique comparison pack |
| P1 | 10.1–10.2 | Questions_23_5, Q1–Q7 | Testing self-learning systems in unknown or dangerous scenarios, autonomy handover, virtual test environments, simulators, simulation benefits | Red | Understand when and why VTEs are used | Create examples for hazardous scenario testing and VTE benefits | VTE summary sheet |
| P1 | 11.1–11.6.2 | Questions_23_5, Q8–Q23 | AI for testing, defect triage, test generation, test oracle problem in test generation, regression optimization, defect prediction, visual testing, GUI testing | Red | Understand how AI supports testing activities | Build a map of AI-for-testing use cases | Chapter 11 AI-for-testing map |

---

## Recovery Order

Use this order for the next study cycle.

| Order | Area | Reason |
|---:|---|---|
| 1 | Chapter 9 | High exam relevance and many similar techniques that are easy to confuse. |
| 2 | Chapter 8 | Contains core AI testing challenges: self-learning, autonomy, probabilistic behaviour, explainability and quality characteristics. |
| 3 | Chapter 5 | Metrics are highly testable and useful across many scenarios. |
| 4 | Chapters 3 and 4 | ML workflow and data quality are foundational for later chapters. |
| 5 | Chapter 7 | Connects AI components with test levels, documentation, concept drift and risk. |
| 6 | Chapters 10 and 11 | Covers advanced scenarios: VTEs and AI used as a testing tool. |
| 7 | Chapters 1 and 2 | Important for terminology and conceptual questions. |
| 8 | Chapter 6 | Needs enough understanding for neural-network-specific questions, but should not consume too much time. |

---

## Weekly Revision Plan

### Monday

Focus: Chapter 9 – AI-specific test techniques.

Tasks:

- Review adversarial testing vs data poisoning.
- Review pairwise testing vs exhaustive testing.
- Review back-to-back testing vs A/B testing vs metamorphic testing.
- Answer 10 practice questions from Chapter 9.

Expected output:

- Technique comparison table.

### Tuesday

Focus: Chapter 8 – testing challenges of AI-based systems.

Tasks:

- Review self-learning systems.
- Review autonomy testing.
- Review probabilistic systems and sophisticated expected results.
- Review explainability and LIME.

Expected output:

- Chapter 8 concept map.

### Wednesday

Focus: Chapter 5 – metrics.

Tasks:

- Practise Accuracy, Precision, Recall and F1-score.
- Review ROC and AUC.
- Review when each metric is appropriate.
- Answer scenario-based metric questions.

Expected output:

- Metrics decision table.

### Thursday

Focus: Chapters 3 and 4 – ML workflow and data.

Tasks:

- Review supervised, unsupervised and reinforcement learning.
- Review ML workflow steps.
- Review data preparation, pre-processing, augmentation and labelling.
- Review dataset split and cross-validation.

Expected output:

- ML workflow and data preparation summary.

### Friday

Focus: Chapter 7 – testing AI-based systems.

Tasks:

- Review input data testing.
- Review ML model testing.
- Review component integration and system testing.
- Review automation bias, complacency bias and documentation.
- Review concept drift.

Expected output:

- AI testing levels map.

### Weekend

Focus: Mixed revision.

Tasks:

- Re-answer failed questions.
- Update the results tracker.
- Create a wrong-answer log.
- Identify next week’s P0 topics.

Expected output:

- Updated matrix and wrong-answer log.

---

## Results Tracker

Fill this table after each practice attempt.

| Date | Source | Syllabus area | Correct | Total | Score | Status | Main mistakes | Next action |
|---|---|---|---:|---:|---:|---|---|---|
| YYYY-MM-DD | Questions_63_1 | 1.1–1.9 |  | 45 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_63_1 | 2.1–2.8 |  | 18 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_36_2 | 3.1–3.5 |  | 20 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_36_2 | 4.1–4.5.1 |  | 16 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_38_3 | 5.1–5.5 |  | 15 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_38_3 | 6.1–6.2 |  | 8 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_38_3 | 7.1–7.7 |  | 15 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_45_4 | 8.1–8.8 |  | 26 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_45_4 | 9.1.1–9.7 |  | 19 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_23_5 | 10.1–10.2 |  | 7 |  | Red/Amber/Green |  |  |
| YYYY-MM-DD | Questions_23_5 | 11.1–11.6.2 |  | 16 |  | Red/Amber/Green |  |  |

---

## Wrong-Answer Log Template

Use this template for each failed question.

```text
Question:
Syllabus area:
My answer:
Correct answer:
Why I missed it:
Concept to review:
Exam trap:
Short rule to remember:
```

---

## Exam Trap Categories

Use these categories when analysing wrong answers.

| Trap category | Meaning | Example |
|---|---|---|
| Similar terms | Confusing close concepts | Precision vs Recall; Back-to-back vs A/B testing |
| Wrong problem type | Applying a metric or technique to the wrong context | Using R-squared for classification |
| Keyword trap | Choosing an answer based on one familiar word | Seeing “AI” and ignoring the scenario |
| Overgeneralisation | Choosing a statement that sounds broadly true but is not syllabus-specific | “AI always improves accuracy” |
| Missing risk perspective | Ignoring the risk behind the scenario | False negatives in cancer detection require Recall |
| Ignoring operational context | Forgetting the system environment or autonomy level | Testing autonomy only in safe conditions |

---

## Short Rules to Remember

- Accuracy = percentage of all correct classifications.
- Precision = confidence that predicted positives are really positive.
- Recall = ability to find actual positives.
- F1-score = balance between Precision and Recall.
- AUC/ROC = classification discrimination across thresholds.
- R-squared = regression fit.
- Metamorphic testing = change input and check expected relation.
- Back-to-back testing = same input, compare systems or versions.
- A/B testing = compare variants through user or operational behaviour.
- Pairwise testing = reduce combinations while covering value pairs.
- Adversarial testing = manipulate valid inputs to fool the model.
- Data poisoning = manipulate training data.
- VTE = simulate complex, dangerous, expensive or impossible scenarios.
- Defect prediction = predict defect-prone areas to prioritise testing.
- Regression optimization = select, reduce or prioritise regression tests.
- Concept drift = operational environment changes while the model does not.
- Automation bias = humans over-trust AI decisions.
- Complacency bias = humans monitor AI less carefully because they expect it to work.

---

## Definition of Done for This Recovery Cycle

This recovery cycle is complete when:

- Each syllabus area has been attempted again.
- Each area has at least 65%.
- P0 areas have at least 75%.
- At least three areas have reached 80% or more.
- All wrong answers have been classified by concept and trap category.
- Chapters 8 and 9 have dedicated summary sheets.

