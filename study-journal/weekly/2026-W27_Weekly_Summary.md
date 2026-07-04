# Weekly Summary – 2026-W27

## Period

2026-07-01 to 2026-07-03

## Context

This was the first study week for the ISTQB Certified Tester AI Testing (CT-AI) certification.

The week focused on understanding the foundations of AI-based systems, the main differences between traditional software testing and AI testing, and the specific challenges introduced by machine learning models, data quality, probabilistic behaviour and continuous monitoring.

Since this was a partial week, the summary consolidates three daily study notes.

---

## Main Achievements

- Started the structured preparation for the ISTQB CT-AI certification.
- Reviewed the foundations of Artificial Intelligence and Machine Learning.
- Identified key differences between traditional software systems and AI-based systems.
- Studied the Machine Learning workflow, including data preparation, training, validation, testing and monitoring.
- Reviewed the role of data quality in AI systems.
- Studied the Confusion Matrix and the main classification metrics.
- Identified Accuracy limitations in imbalanced datasets.
- Started the study of AI-specific testing challenges and techniques.
- Identified Chapter 7 as one of the most difficult areas and a priority for further study.

---

## Key Concepts Learned

### AI and Machine Learning Foundations

- AI systems may behave in a probabilistic, adaptive and non-deterministic way.
- Machine Learning models learn patterns from data instead of following only explicitly programmed rules.
- The quality of an ML model depends strongly on the quality, representativeness and integrity of the data.
- Training, validation and test datasets must be clearly separated.
- Poor data quality may introduce risks such as bias, overfitting, underfitting, leakage and unreliable predictions.

### Classification Metrics

- A Confusion Matrix helps analyse classification results through:
  - True Positives (TP)
  - True Negatives (TN)
  - False Positives (FP)
  - False Negatives (FN)

- Main metrics studied:
  - Accuracy
  - Precision
  - Recall
  - Specificity
  - F1-Score

- Accuracy can be misleading when classes are imbalanced.
- Precision and Recall should be selected according to the risk of false positives and false negatives.

### AI Testing Challenges

- AI testing is more complex than traditional testing because expected results may be difficult to define.
- The Test Oracle Problem is a central challenge in AI-based systems.
- Concept Drift can cause model performance degradation over time.
- Bias, explainability, robustness, transparency and ethical considerations are relevant quality factors.
- Continuous monitoring is essential after deployment.

### AI-Specific Testing Techniques

The following techniques were introduced and require further consolidation:

- Input Data Testing
- ML Model Testing
- Metamorphic Testing
- Back-to-Back Testing
- A/B Testing
- Pairwise Testing
- Statistical Testing
- Adversarial Testing
- Experience-Based Testing

### AI Security and Operational Risks

- Adversarial attacks may manipulate inputs to mislead the model.
- Data poisoning may compromise the training data.
- Monitoring and data validation are important mitigation strategies.

### AI for Testing

AI can also support software testing activities, such as:

- Defect prediction
- Intelligent incident analysis
- Automatic test case generation
- Regression test optimization
- GUI testing using Machine Learning and Computer Vision

---

## Decisions Made

- Continue using daily notes as the primary study log.
- Create weekly summaries to consolidate learning and track progress.
- Use the weekly summary to identify weak areas and plan the following week.
- Prioritise understanding before memorisation.
- Focus next on Chapter 7, since it was the most difficult area in the first week.
- Keep the AI QA Framework connection secondary and only document it when it adds value.

---

## Open Questions

The following concepts need further study and practical examples:

### AI and ML Foundations

- Overfitting
- Underfitting
- Concept Drift
- Leakage
- Supervised Learning
- Unsupervised Learning
- Embedding format
- Labeled data
- Unlabeled data
- Tuning
- Labeling methods

### Metrics and Evaluation

- Benchmark suites
- Performance benchmark metrics
- Balanced datasets
- Imbalanced datasets
- F1-Score
- AUC
- LLM evaluations
- RAGAS

### AI Testing Techniques

- Test data challenges
- Input Data Testing
- ML Model Testing
- Test Oracle Problem
- Metamorphic Testing
- Back-to-Back Testing
- A/B Testing
- Pairwise Testing
- Statistical Testing
- Adversarial Testing
- Virtual Test Environments (VTEs)

### AI Risks and Monitoring

- Automation Bias
- Explainable AI (XAI)
- Bias Detection
- Data Poisoning
- Regression Test Optimization
- Defect Prediction

---

## Difficult Areas

Chapter 7 was identified as the most challenging area of the syllabus so far.

The main difficulty is not only understanding each technique individually, but knowing when and why each technique should be applied in AI testing.

Priority areas:

1. Test Oracle Problem
2. Metamorphic Testing
3. Back-to-Back Testing
4. A/B Testing
5. Adversarial Testing
6. VTEs
7. Defect Prediction
8. Regression Test Optimization

---

## Priorities for the Following Week

- Review the Test Oracle Problem with practical examples.
- Study Metamorphic Testing in depth.
- Compare Metamorphic Testing with Back-to-Back Testing.
- Clarify the difference between traditional test automation and AI-specific test techniques.
- Practise classification metrics using simple examples.
- Review imbalanced datasets and the limitations of Accuracy.
- Create short revision cards for the most difficult concepts.
- Repeat quiz questions related to Chapter 7 after consolidation.

---

## Link to the AI QA Framework

Potential future links to the AI QA Framework:

- Data quality controls for AI systems.
- Checklist for dataset separation: training, validation and test data.
- Risk catalogue for AI systems, including bias, concept drift, leakage and data poisoning.
- Model evaluation criteria based on classification and regression metrics.
- Guidance for selecting AI-specific testing techniques.
- Monitoring strategy for models in production.

These ideas should not be expanded yet. The current priority remains CT-AI exam preparation.

---

## End-of-Week Reflection

The first week established the foundations for CT-AI study.

The main takeaway is that testing AI systems requires a broader view than traditional software testing. It is necessary to consider data, model behaviour, metrics, monitoring, explainability, bias, robustness and security.

The next week should focus on turning the most difficult concepts into practical, exam-ready knowledge.
