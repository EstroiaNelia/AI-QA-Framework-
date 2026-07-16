# CT-AI Answer Key – Chapters 5–7

Suggested repository path:

```text
study-journal/study-packs/answer-keys/CT-AI_Answer_Key_Chapters_5-7.md
```

## Scope

Source practice set: `Questions_38_3.docx`  
Covered questions: 1 to 38  
Covered syllabus areas in the practice set: 5.1 to 7.7

## Notes

- The answers are written in English, by full meaning rather than only by option letter.
- The rationale is syllabus-oriented and focuses on why the answer is correct.
- Some practice questions use older CT-AI section numbering. The current CT-AI syllabus v2.0 reorganizes several topics. The concepts remain useful for revision.
- This block focuses mainly on ML functional performance metrics, neural networks, neural network coverage, AI-specific test levels, documentation, automation/complacency bias, and concept drift.

---

## Question 1

**Question:** What does the accuracy metric measure?

**Correct answer:**  
Accuracy measures the percentage of all classifications that are correct.

**Syllabus rationale:**  
Accuracy considers both correctly predicted positives and correctly predicted negatives. It is calculated as the proportion of all correct classifications among all classifications.

---

## Question 2

**Question:** What does a low F1-score suggest?

**Correct answer:**  
A low F1-score suggests that the model has poor combined performance for precision and recall, especially for the positive class.

**Syllabus rationale:**  
The F1-score is the harmonic mean of precision and recall. If the F1-score is low, at least one of these two metrics is low. This usually indicates that the model is not handling positive predictions well, either because it misses positives or because many predicted positives are wrong.

---

## Question 3

**Question:** Which metric is used to measure the ability of a binary classifier as its discrimination threshold is varied?

**Correct answer:**  
The Receiver Operating Characteristic curve, or ROC curve, is used to evaluate a binary classifier as the discrimination threshold is varied.

**Syllabus rationale:**  
The ROC curve shows how the true positive rate and false positive rate change at different classification thresholds. It is used for supervised binary classification problems.

---

## Question 4

**Question:** What does a higher AUC value indicate in a classifier?

**Correct answer:**  
A higher AUC value indicates better predictive performance and better separability between classes.

**Syllabus rationale:**  
AUC, the area under the ROC curve, summarizes the classifier’s ability to distinguish between positive and negative classes. A higher AUC generally means stronger discrimination.

---

## Question 5

**Question:** Which metric measures how well a regression model fits the dependent variable in supervised regression models?

**Correct answer:**  
R-squared measures how well a regression model fits the dependent variable.

**Syllabus rationale:**  
R-squared is used in regression problems to indicate how much of the variation in the dependent variable is explained by the model.

---

## Question 6

**Question:** Which metrics and approaches should a fraud detection team prioritize to evaluate a binary classifier’s ability to distinguish between fraudulent and non-fraudulent transactions?

**Correct answer:**  
The team should use the ROC curve and AUC to assess the model’s ability to distinguish between fraudulent and non-fraudulent transactions.

**Syllabus rationale:**  
Fraud detection is a supervised binary classification problem. ROC and AUC are appropriate when the goal is to evaluate the classifier’s discrimination ability across different thresholds.

---

## Question 7

**Question:** What do ML functional performance metrics measure?

**Correct answer:**  
ML functional performance metrics measure the functionality of the model.

**Syllabus rationale:**  
ML functional performance metrics evaluate how well the ML model performs its intended prediction, classification, or regression task. They are not general non-functional quality characteristics.

---

## Question 8

**Question:** ML functional performance metrics are calculated based on what?

**Correct answer:**  
They are calculated based on correctly labelled data.

**Syllabus rationale:**  
To calculate metrics such as accuracy, precision, recall, and F1-score, the actual expected labels must be known. Without correct labels, model predictions cannot be meaningfully compared with expected results.

---

## Question 9

**Question:** Which ML functional performance metric is most suitable when the cost of false positives is high and confidence in positive outcomes needs to be high?

**Correct answer:**  
Precision is the most suitable metric.

**Syllabus rationale:**  
Precision measures the proportion of predicted positives that are actually positive. It is important when false positives are costly and the team needs high confidence that positive predictions are correct.

---

## Question 10

**Question:** When is a high recall score important?

**Correct answer:**  
A high recall score is important when actual positive cases should not be missed.

**Syllabus rationale:**  
Recall measures the proportion of actual positives that are correctly identified. It is especially important when false negatives are dangerous or costly.

---

## Question 11

**Question:** Which metric should be prioritized if the goal is to minimize false negatives, such as in cancer detection?

**Correct answer:**  
Recall should be prioritized.

**Syllabus rationale:**  
In cancer detection, missing an actual positive case can have serious consequences. Recall focuses on detecting as many actual positives as possible and therefore minimizes false negatives.

---

## Question 12

**Question:** In which scenario would the F1-score metric be most useful?

**Correct answer:**  
F1-score is most useful when precision and recall both matter and a balance between them is needed, especially when the expected classes are imbalanced.

**Syllabus rationale:**  
F1-score combines precision and recall into a single metric. It is useful when a model must avoid both false positives and false negatives and when accuracy alone may be misleading due to class imbalance.

**Review note:**  
The answer options in the practice question are not perfectly phrased. The key rule to remember is: use F1-score when both precision and recall are important.

---

## Question 13

**Question:** For which type of problem is AUC for the ROC curve most applicable?

**Correct answer:**  
AUC for the ROC curve is most applicable to supervised classification problems.

**Syllabus rationale:**  
ROC and AUC are used to evaluate the discrimination ability of classifiers, especially binary classifiers, across decision thresholds.

---

## Question 14

**Question:** A hospital wants to identify as many true positive cases of a rare aggressive cancer as possible, even if this means having some false positives. Which metric should it prioritize?

**Correct answer:**  
The hospital should prioritize recall because recall ensures that the model identifies as many true positive cases as possible, even at the expense of some false positives.

**Syllabus rationale:**  
The main risk in this scenario is a false negative, meaning a patient with cancer is missed. Recall is the metric that focuses on minimizing missed positives.

---

## Question 15

**Question:** Which organization provides ML benchmark suites for software frameworks, AI-specific processors, and ML cloud platforms?

**Correct answer:**  
MLCommons provides ML benchmark suites for software frameworks, AI-specific processors, and ML cloud platforms.

**Syllabus rationale:**  
MLCommons develops ML benchmark suites, such as MLPerf, which are used to compare ML systems, hardware, frameworks, and cloud platforms.

---

## Question 16

**Question:** What is the purpose of artificial neural networks?

**Correct answer:**  
Artificial neural networks are intended to mimic aspects of how the human brain processes information.

**Syllabus rationale:**  
Artificial neural networks are inspired by networks of neurons. They process inputs through connected artificial neurons and can learn patterns from data.

---

## Question 17

**Question:** What is the single-layer perceptron?

**Correct answer:**  
A single-layer perceptron is a simple neural network with one layer and one neuron.

**Syllabus rationale:**  
A perceptron is one of the simplest forms of artificial neural network. It takes inputs, applies weights and a bias, and produces an output through an activation function.

---

## Question 18

**Question:** What are deep neural networks?

**Correct answer:**  
Deep neural networks are neural networks with several layers.

**Syllabus rationale:**  
A neural network is considered deep when it has multiple layers, especially hidden layers, between the input and output layers.

---

## Question 19

**Question:** What is the range of activation values in artificial neural networks?

**Correct answer:**  
Activation values can range from negative infinity to positive infinity before an activation function constrains or transforms them.

**Syllabus rationale:**  
The raw activation value of a neuron is computed from weighted inputs and bias. Depending on the activation function, the output may then be transformed to a smaller range, such as 0 to 1 or -1 to +1. In this question, the best answer is the unrestricted activation value range.

---

## Question 20

**Question:** A deep neural network consistently misclassifies dogs as cats. What adjustment should the company consider?

**Correct answer:**  
The company should increase the amount of labelled training data, especially examples of both cats and dogs, to improve the network’s ability to learn the differences between the two classes.

**Syllabus rationale:**  
If a model consistently confuses two similar classes, one likely cause is that the training data does not provide enough representative examples for the model to learn the distinction. Improving labelled training data can improve classification performance.

---

## Question 21

**Question:** Which statement is true about achieving white-box test coverage criteria for neural networks?

**Correct answer:**  
Traditional white-box test coverage provides little value when measuring the coverage of neural networks.

**Syllabus rationale:**  
Neural networks require specialized coverage measures, such as neuron coverage and related measures. Traditional structural code coverage does not adequately describe how the neural network behaves internally.

---

## Question 22

**Question:** Which coverage measure requires each neuron in the neural network to achieve an activation value greater than zero?

**Correct answer:**  
Neuron coverage requires each neuron to be activated, commonly meaning that each neuron achieves an activation value greater than zero at least once.

**Syllabus rationale:**  
Neuron coverage is a neural-network-specific coverage measure. It checks whether individual neurons have been activated during testing.

---

## Question 23

**Question:** What is the purpose of the Sign-Sign coverage measure?

**Correct answer:**  
Sign-Sign coverage considers pairs of neurons in adjacent layers.

**Syllabus rationale:**  
Sign-Sign coverage is a neural network coverage measure that focuses on relationships between neurons in adjacent layers, especially whether changes in neuron activation signs propagate between connected neurons.

---

## Question 24

**Question:** Why are system requirements and design specifications important for both AI-based systems and conventional systems?

**Correct answer:**  
They provide a basis for testers to check system behaviour.

**Syllabus rationale:**  
Testing requires a basis for determining whether the system behaves as expected. Requirements and design specifications help define expected behaviour, acceptance criteria, and test conditions.

---

## Question 25

**Question:** What distinguishes the testing of AI components from conventional software testing?

**Correct answer:**  
Testing AI components includes specialized test levels and activities for handling input data and ML models.

**Syllabus rationale:**  
AI-based systems require conventional testing, but they also introduce AI-specific concerns such as input data testing, model testing, ML functional performance testing, data quality, and bias-related testing.

---

## Question 26

**Question:** What is the primary objective of input data testing in AI-based systems?

**Correct answer:**  
The primary objective is to ensure the highest practical quality of the data used for training and prediction.

**Syllabus rationale:**  
The behaviour of ML systems depends heavily on data. Input data testing focuses on data quality, representativeness, constraints, labelling, and suitability for training, validation, testing, and operational prediction.

---

## Question 27

**Question:** What distinguishes component integration testing in AI-based systems from conventional integration testing?

**Correct answer:**  
It ensures the accurate interaction between system components, including both AI and non-AI components.

**Syllabus rationale:**  
AI-based systems usually combine ML components with conventional software components. Integration testing must check that these components interact correctly.

---

## Question 28

**Question:** What distinguishes system testing in AI-based systems from conventional system testing?

**Correct answer:**  
System testing in AI-based systems checks that ML functional performance criteria are still met when the AI model is integrated into the complete system.

**Syllabus rationale:**  
A model may perform well in isolation but behave differently when integrated into the full system. System testing must evaluate the complete AI-based system, not only the model.

---

## Question 29

**Question:** What is the purpose of system testing for an autonomous delivery drone system using ML for route optimization and obstacle detection?

**Correct answer:**  
The purpose is to ensure that the complete drone system, including both AI and non-AI components, performs as expected in a representative test environment.

**Syllabus rationale:**  
System testing evaluates the complete integrated system against requirements and acceptance criteria. For an autonomous drone, this includes ML components, sensors, control logic, non-AI software, and interactions among them.

---

## Question 30

**Question:** How can defects in data acquisition and data preprocessing be masked?

**Correct answer:**  
They can be masked by using the same implementation as the data scientists.

**Syllabus rationale:**  
If testers use the same implementation or assumptions as the development/data science team, common defects may not be detected. Independent checks help reveal defects in data acquisition and preprocessing.

---

## Question 31

**Question:** Which two forms of bias are associated with humans being too trusting of AI-based systems in decision-making?

**Correct answer:**  
Automation bias and complacency bias are associated with humans being too trusting of AI-based systems.

**Syllabus rationale:**  
Automation bias occurs when humans over-rely on automated outputs. Complacency bias occurs when humans reduce vigilance because they expect the system to work correctly.

---

## Question 32

**Question:** What are the potential consequences of automation bias and complacency bias?

**Correct answer:**  
They can lead to decreased decision-making accuracy and potential system failures.

**Syllabus rationale:**  
When humans trust AI outputs too much or monitor systems less carefully, they may fail to identify incorrect recommendations, warnings, or decisions. This can reduce decision quality and create failures.

---

## Question 33

**Question:** Which item is not typically included in the documentation of an AI component?

**Correct answer:**  
Implementation details of the operating environment are not usually part of the AI component documentation itself.

**Syllabus rationale:**  
AI component documentation typically includes general information, design information, assumptions, technical decisions, model information, data information, and dataset-related details. The wider operating environment may be documented elsewhere at system level.

---

## Question 34

**Question:** Why is clear documentation important for testing AI-based systems?

**Correct answer:**  
Clear documentation provides transparency on the implementation of the system.

**Syllabus rationale:**  
AI-based systems can be difficult to understand and test without sufficient documentation. Documentation supports transparency, review, risk analysis, test design, and interpretation of model behaviour.

---

## Question 35

**Question:** Which documentation aspect is most beneficial for ensuring that testing covers adaptability to changing traffic conditions in an AI-driven traffic management system?

**Correct answer:**  
Specification of the operating environment is most beneficial.

**Syllabus rationale:**  
Adaptability is about how the system behaves when its operational environment changes. To test this properly, testers need to understand the expected operating environment and relevant environmental variations.

---

## Question 36

**Question:** What aspect of the system should be clearly understood when testing for functional correctness of untrustworthy inputs?

**Correct answer:**  
The source of input data and associated metadata should be clearly understood.

**Syllabus rationale:**  
When testing behaviour with potentially untrustworthy inputs, testers need to know where input data comes from, how it was collected, and which metadata describes its origin and quality. This helps identify input-related risks and design meaningful tests.

**Review note:**  
This question is wording-sensitive. For general functional correctness, the system purpose and functional requirements are essential. In this specific question, the wording emphasizes untrustworthy inputs, so input source and metadata are the most relevant answer.

---

## Question 37

**Question:** What is concept drift in the context of AI models?

**Correct answer:**  
Concept drift occurs when the operational reality or the relationship between input data and the correct output changes while the model itself has not changed.

**Syllabus rationale:**  
Concept drift means that the model’s learned patterns no longer reflect the current reality. The model may degrade because the meaning of the data or the relationship between inputs and outputs has changed over time.

---

## Question 38

**Question:** What is the purpose of testing in an AI-based system?

**Correct answer:**  
The purpose is to mitigate risks through specialized testing, including risks specific to AI components.

**Syllabus rationale:**  
AI-based systems require conventional testing plus specialized testing to address AI-specific risks, such as data quality, model behaviour, non-determinism, bias, concept drift, robustness, and integration of AI and non-AI components.

---

## Quick revision rules

- Accuracy = percentage of all correct classifications.
- Precision = confidence that predicted positives are actually positive.
- Recall = ability to find actual positives.
- F1-score = balance between precision and recall.
- ROC/AUC = classifier discrimination across thresholds.
- R-squared = regression fit.
- Use Recall when false negatives are dangerous.
- Use Precision when false positives are costly.
- Use F1-score when both precision and recall matter.
- Neural networks require neural-network-specific coverage, not only traditional code coverage.
- Neuron coverage checks whether neurons are activated.
- AI component testing includes input data and model-specific testing.
- System testing checks the complete AI-based system, not just the ML model.
- Automation bias = humans over-trust AI outputs.
- Complacency bias = humans monitor less carefully because they expect the AI to work.
- Concept drift = the real-world relationship changes while the model remains unchanged.
