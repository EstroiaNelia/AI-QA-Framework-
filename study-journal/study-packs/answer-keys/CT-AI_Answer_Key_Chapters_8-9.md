# CT-AI Answer Key – Chapters 8–9

Suggested repository path:

```text
study-journal/study-packs/answer-keys/CT-AI_Answer_Key_Chapters_8-9.md
```

## Scope

Source practice set: `Questions_45_4.docx`  
Covered questions: 1 to 45  
Covered syllabus areas in the practice set: 8.1 to 9.7

## Notes

- The answers are written in English, by full meaning rather than only by option letter.
- The rationale is syllabus-oriented and focuses on why the answer is correct.
- Some practice questions use older CT-AI section numbering. The current CT-AI syllabus v2.0 reorganizes several topics. The concepts remain useful for revision.
- This block is high priority because it covers several weak areas: self-learning systems, autonomy, bias, probabilistic systems, explainability, adversarial testing, data poisoning, combinatorial testing, back-to-back testing, A/B testing, metamorphic testing, and experience-based testing.

---

## Question 1

**Question:** What is a challenge related to the test environment when testing self-learning systems?

**Correct answer:**  
A complex test environment is a challenge when testing self-learning systems.

**Syllabus rationale:**  
Self-learning systems may change their behaviour over time and may need to be tested under many operational conditions. This makes the test environment more complex, because it may need to represent dynamic, high-risk, or changing real-world situations.

---

## Question 2

**Question:** What challenge arises when testing self-learning systems regarding unexpected changes in their behaviour?

**Correct answer:**  
A key challenge is insufficient testing time to manually execute new tests after each change.

**Syllabus rationale:**  
Self-learning systems can change their behaviour after learning or adaptation. If every behavioural change requires retesting, manual testing may not be feasible. This creates a need for automated and repeatable tests that can be run when the system changes.

---

## Question 3

**Question:** How might the challenge of insufficient testing time be mitigated when testing self-learning systems?

**Correct answer:**  
The challenge can be mitigated by writing tests that can be run automatically when the system changes itself.

**Syllabus rationale:**  
Automated tests help support repeated testing when a self-learning system changes behaviour. This is important because manual re-execution after every system change may be too slow or impractical.

---

## Question 4

**Question:** What is a significant challenge in testing self-learning systems related to resource requirements?

**Correct answer:**  
A significant challenge is specifying the resources permitted for self-learning or adaptation.

**Syllabus rationale:**  
Self-learning and adaptation may consume resources such as time, processing capacity, memory, data, or energy. The allowed resource limits should be specified so that testing can verify whether the system remains within acceptable operational constraints.

---

## Question 5

**Question:** Which scenario best illustrates an appropriate testing strategy for a self-learning smart home AI that may make unexpected changes?

**Correct answer:**  
The company should create dynamic tests that adapt based on observed AI behaviour changes and continuously monitor for unexpected system adaptations.

**Syllabus rationale:**  
Self-learning systems require more than static one-time testing. Testing should account for behavioural changes, monitor adaptations, and include tests that remain relevant as the system evolves.

---

## Question 6

**Question:** Which option is not a requirement for testing the autonomy of AI-based systems?

**Correct answer:**  
Testing the system’s ability to perform tasks with human support only is not a requirement for testing autonomy.

**Syllabus rationale:**  
Autonomy testing focuses on whether the system can operate independently when it should, whether it requests human intervention when required, and whether it avoids unnecessary human intervention. Testing only human-supported operation does not test autonomy.

---

## Question 7

**Question:** What approach can help generate the necessary conditions for testing the autonomy of AI-based systems?

**Correct answer:**  
Boundary value analysis applied to the operating environment can help generate the necessary conditions.

**Syllabus rationale:**  
Autonomy often depends on operational limits and environmental conditions. Boundary value analysis can be applied to these conditions to test behaviour near the limits where the system should continue autonomously or relinquish control.

---

## Question 8

**Question:** Why is obtaining additional information about input data important when testing for bias?

**Correct answer:**  
Additional information is important because it helps identify hidden variables that may cause bias, supports accurate correlation analysis between attributes and results, and may provide demographic data for analysis.

**Syllabus rationale:**  
Bias may not be visible from the main input features alone. Additional information can reveal hidden relationships, proxy variables, or demographic patterns that influence model outputs unfairly.

---

## Question 9

**Question:** What method can detect bias by examining the correlation between input data attributes and system outputs at a local level?

**Correct answer:**  
LIME, or Local Interpretable Model-Agnostic Explanations, can be used.

**Syllabus rationale:**  
LIME explains individual model predictions by perturbing inputs and observing changes in outputs. This can help identify local relationships between input attributes and model decisions, including potential bias.

---

## Question 10

**Question:** What activity during the ML workflow is crucial for identifying whether algorithmic bias is present in an ML model?

**Correct answer:**  
Evaluation and tuning activities are crucial for identifying algorithmic bias.

**Syllabus rationale:**  
Algorithmic bias can be detected by analysing model behaviour during evaluation and tuning. This includes checking whether the model performs differently across groups or whether the algorithm produces biased outcomes even when the data appears acceptable.

---

## Question 11

**Question:** Which approach best identifies and mitigates algorithmic and sample bias in a healthcare ML system?

**Correct answer:**  
The company should analyse the model during training, evaluation, and tuning to detect algorithmic bias, and review the source of the training data to identify sample bias.

**Syllabus rationale:**  
Algorithmic bias and sample bias have different causes. Algorithmic bias is related to model behaviour and training decisions. Sample bias is related to the data source, representativeness, and data collection process. Both must be tested.

---

## Question 12

**Question:** Why is it necessary to run tests multiple times for probabilistic systems?

**Correct answer:**  
Tests must be run multiple times to generate statistically valid test results.

**Syllabus rationale:**  
Probabilistic systems may produce different valid outputs for the same input. Multiple executions provide enough evidence to assess whether the system behaviour is statistically acceptable.

---

## Question 13

**Question:** Which challenge is associated with testing probabilistic AI-based systems?

**Correct answer:**  
A key challenge is stating exact values for expected test results.

**Syllabus rationale:**  
Probabilistic systems may not produce one deterministic expected output. Instead of exact expected values, testers may need ranges, tolerances, confidence levels, or statistical acceptance criteria.

---

## Question 14

**Question:** What is a potential solution for dealing with the non-deterministic nature of probabilistic AI-based systems during testing?

**Correct answer:**  
A potential solution is defining more sophisticated expected results.

**Syllabus rationale:**  
For probabilistic systems, expected results may need to be expressed using tolerances, statistical distributions, acceptable ranges, or confidence intervals rather than exact deterministic values.

---

## Question 15

**Question:** How should a financial institution test a probabilistic AI system for predicting stock prices when the same inputs may produce different valid outcomes?

**Correct answer:**  
The institution should run each scenario multiple times and define expected results with tolerances, such as accepting results within a defined percentage range of the optimal solution.

**Syllabus rationale:**  
Probabilistic AI systems may produce variable but still acceptable outputs. Multiple runs and tolerance-based expected results provide a more suitable test approach than requiring one exact value.

---

## Question 16

**Question:** What challenge arises when the internal structure of an AI-based system is too complex for humans to understand?

**Correct answer:**  
This can create or intensify the test oracle problem.

**Syllabus rationale:**  
When humans cannot understand how the system reaches its outputs, it becomes harder to determine whether a result is correct. This is closely linked to the test oracle problem.

---

## Question 17

**Question:** How does interaction between AI components affect testing?

**Correct answer:**  
The interaction between AI components makes it challenging to comprehend and verify the system.

**Syllabus rationale:**  
AI-based systems may include several interacting AI and non-AI components. Their combined behaviour can be complex, non-transparent, and difficult to predict, which increases testing difficulty.

---

## Question 18

**Question:** Which method can provide model explainability in a model-agnostic manner?

**Correct answer:**  
The LIME method can provide model explainability in a model-agnostic manner.

**Syllabus rationale:**  
LIME is model-agnostic because it can be applied to different types of ML models without needing access to their internal implementation. It explains individual predictions by analysing how input perturbations affect outputs.

---

## Question 19

**Question:** What makes test design challenging when implementation information is not available?

**Correct answer:**  
It becomes difficult to determine expected results.

**Syllabus rationale:**  
When testers lack information about the system implementation, behaviour, or decision logic, it is harder to define meaningful test cases and expected outcomes.

---

## Question 20

**Question:** Which method is primarily used to understand explainability in ML models by applying perturbations to test data?

**Correct answer:**  
The LIME method is primarily used.

**Syllabus rationale:**  
LIME applies perturbations to input data and observes how the model output changes. This supports local explanation of individual predictions.

---

## Question 21

**Question:** How can testers address low explainability in an AI-based credit scoring system to meet transparency requirements?

**Correct answer:**  
Testers should conduct exploratory testing to understand input-output relationships and use methods such as LIME to provide visual or local explanations of model decisions.

**Syllabus rationale:**  
Low explainability can be addressed by using testing and explanation techniques that reveal how inputs affect outputs. For regulated systems such as credit scoring, explanations support transparency, auditability, and trust.

---

## Question 22

**Question:** What is a significant challenge associated with the correctness of software behaviour in AI-based systems?

**Correct answer:**  
A significant challenge is the subjectivity of correctness assessment.

**Syllabus rationale:**  
For some AI-based systems, correctness may not be absolute. Different human experts may judge outputs differently, and acceptable behaviour may depend on context, uncertainty, or interpretation.

---

## Question 23

**Question:** Which option is not a quality characteristic for an AI-based system?

**Correct answer:**  
Scalability is not listed as a top-level quality characteristic in the same way as functional suitability, performance efficiency, and compatibility.

**Syllabus rationale:**  
Functional suitability, performance efficiency, and compatibility are recognized software quality characteristics. Scalability may be relevant in practice, but in this question it is not the intended quality characteristic.

---

## Question 24

**Question:** What is one aspect to consider when evaluating the adaptability of a system?

**Correct answer:**  
One aspect is the time it takes for the system to adapt to a change in its environment.

**Syllabus rationale:**  
Adaptability concerns how well the system adjusts to environmental changes. Evaluation should consider whether it continues to meet requirements, how long adaptation takes, and what resources are used.

---

## Question 25

**Question:** How can interpretability and explainability of a system be checked?

**Correct answer:**  
They can be checked by questioning system users or people with a similar background.

**Syllabus rationale:**  
Interpretability and explainability depend on whether intended users can understand the system’s outputs and explanations. User-based evaluation helps determine whether explanations are meaningful to the target audience.

---

## Question 26

**Question:** What tests should be performed to assess adaptability and flexibility in an autonomous driving system?

**Correct answer:**  
To evaluate adaptability, the company should check whether the system continues to meet functional and non-functional requirements when it adapts to environmental changes, and measure the resources and time used for adaptation. To evaluate flexibility, the company should verify how the system handles contexts outside its initial specification through automated regression testing, and measure the resources and time needed to manage new contexts.

**Syllabus rationale:**  
Adaptability concerns changes in the system’s environment and whether the system can adjust appropriately. Flexibility concerns the system’s ability to cope with new contexts or situations. Both should be evaluated against requirements, resources, and time.

---

## Question 27

**Question:** What is an adversarial attack?

**Correct answer:**  
An adversarial attack modifies valid inputs to cause incorrect predictions by the trained model.

**Syllabus rationale:**  
In adversarial attacks, the input may still appear valid or normal to humans, but is deliberately modified to mislead the model into making an incorrect prediction.

---

## Question 28

**Question:** What is the purpose of adversarial testing?

**Correct answer:**  
The purpose of adversarial testing is to identify vulnerabilities in the trained model.

**Syllabus rationale:**  
Adversarial testing evaluates whether the model can be fooled by manipulated inputs. It is used to assess robustness and security weaknesses.

---

## Question 29

**Question:** What is the purpose of a data poisoning attack?

**Correct answer:**  
The purpose is to manipulate the training data for future intrusions or future incorrect model behaviour.

**Syllabus rationale:**  
Data poisoning attacks compromise the data used to train or update the model. The attacker influences the model’s future behaviour by corrupting the training data.

---

## Question 30

**Question:** Why is exhaustive testing not feasible for AI-based systems with a high number of parameters?

**Correct answer:**  
Exhaustive testing is not feasible because it would result in an extremely large, and potentially infinite, number of tests.

**Syllabus rationale:**  
AI-based systems may have many input parameters, continuous values, and environmental conditions. Testing every possible combination is not practical, so sampling or combinatorial techniques are needed.

---

## Question 31

**Question:** Which combinatorial testing technique is most widely used in practice?

**Correct answer:**  
Pairwise testing is the most widely used combinatorial testing technique in practice.

**Syllabus rationale:**  
Pairwise testing reduces the number of test combinations while ensuring that every pair of parameter values is covered at least once.

---

## Question 32

**Question:** What is back-to-back testing also known as?

**Correct answer:**  
Back-to-back testing is also known as pseudo-oracle testing in this syllabus context.

**Syllabus rationale:**  
Back-to-back testing uses an alternative implementation, model, or system as a pseudo-oracle. The same inputs are executed against the system under test and the pseudo-oracle, and differences in outputs are analysed.

**Review note:**  
In broader testing literature, back-to-back testing may also be associated with comparison testing or differential testing. For the CT-AI practice context, the pseudo-oracle terminology is especially important.

---

## Question 33

**Question:** Why should there be no common software between the pseudo-oracle and the system under test?

**Correct answer:**  
There should be no common software because the test results could match when both systems contain the same defect.

**Syllabus rationale:**  
If the pseudo-oracle and the system under test share software, frameworks, algorithms, or implementation assumptions, the same defect may exist in both. This would reduce the ability of back-to-back testing to reveal defects.

---

## Question 34

**Question:** What best practices should a fintech company follow when using back-to-back testing for an AI-based fraud detection system?

**Correct answer:**  
The company should use an alternative version of the system developed by a different team on a different platform, ensure that there is no common software between the pseudo-oracle and the system under test, allow the pseudo-oracle to operate without the same non-functional constraints as the system under test, and use different frameworks, algorithms, and model settings where possible.

**Syllabus rationale:**  
Back-to-back testing is stronger when the pseudo-oracle is independent from the system under test. Independence reduces the risk of shared defects and helps make output discrepancies more meaningful.

---

## Question 35

**Question:** A/B testing is a method used to do what?

**Correct answer:**  
A/B testing is used to compare the response of two variants of a program.

**Syllabus rationale:**  
In A/B testing, two or more variants are compared using defined metrics, often with users or operational traffic. It is commonly used to determine which variant performs better in practice.

---

## Question 36

**Question:** What is one major difference between A/B testing and back-to-back testing?

**Correct answer:**  
A/B testing compares two variants of the same system, while back-to-back testing is mainly used to detect defects by comparing outputs with a pseudo-oracle or alternative implementation.

**Syllabus rationale:**  
A/B testing is typically concerned with comparing the effect or performance of variants, often in an operational or user-facing setting. Back-to-back testing compares outputs for the same inputs to identify discrepancies that may indicate defects.

---

## Question 37

**Question:** What is the purpose of metamorphic testing?

**Correct answer:**  
The purpose of metamorphic testing is to generate follow-up test cases based on a source test case that has passed.

**Syllabus rationale:**  
Metamorphic testing uses metamorphic relations to generate follow-up tests. It is especially useful when the exact expected result is difficult to determine, but expected relationships between inputs and outputs are known.

---

## Question 38

**Question:** Which option is not a characteristic of metamorphic testing?

**Correct answer:**  
It is not a characteristic of metamorphic testing that the expected results of follow-up test cases are described in terms of absolute values.

**Syllabus rationale:**  
In metamorphic testing, expected results are normally expressed as relationships between source and follow-up outputs, not as exact absolute expected values.

---

## Question 39

**Question:** How can metamorphic testing be useful when generating expected results is problematic?

**Correct answer:**  
It can generate test cases that create a set of outputs where the relationships between the outputs can be checked for validity.

**Syllabus rationale:**  
Metamorphic testing avoids the need for one exact expected output. Instead, it checks whether the outputs of related tests satisfy known metamorphic relations.

---

## Question 40

**Question:** Which approach correctly applies metamorphic testing to an AI-based image recognition system?

**Correct answer:**  
The team should generate follow-up test cases by modifying source images according to valid metamorphic relations, such as rotation or brightness changes, predict the expected results based on the properties of image recognition, and compare the predicted classifications with the system outputs.

**Syllabus rationale:**  
Metamorphic testing requires meaningful metamorphic relations. For image recognition, certain transformations should not change the class. The tester checks whether the model behaves consistently under those transformations.

---

## Question 41

**Question:** What are the three types of experience-based testing?

**Correct answer:**  
The three types are error guessing, exploratory testing, and checklist-based testing.

**Syllabus rationale:**  
Experience-based testing relies on the knowledge, intuition, and experience of testers, domain experts, or users. The main examples are error guessing, exploratory testing, and checklist-based testing.

---

## Question 42

**Question:** What is the purpose of exploratory testing in the context of AI-based systems?

**Correct answer:**  
The purpose of exploratory testing is to generate and execute tests in an iterative manner.

**Syllabus rationale:**  
Exploratory testing combines test learning, design, and execution. In AI-based systems, it can help investigate uncertain behaviour, unexpected outputs, and risks not fully covered by predefined systematic tests.

---

## Question 43

**Question:** What is the purpose of Exploratory Data Analysis in AI-based systems?

**Correct answer:**  
The purpose of Exploratory Data Analysis is to examine data for patterns, relationships, trends, and outliers.

**Syllabus rationale:**  
EDA helps testers and data scientists understand the data before or during model development. It supports identification of anomalies, relationships, missing values, outliers, and potential data quality or bias issues.

---

## Question 44

**Question:** Which test technique is suitable for mitigating the test oracle problem in AI-based components?

**Correct answer:**  
Back-to-back testing, A/B testing, and metamorphic testing can all help mitigate the test oracle problem.

**Syllabus rationale:**  
When exact expected results are difficult to define, testers may use alternative oracle approaches. Back-to-back testing uses a pseudo-oracle, A/B testing compares variants using outcome metrics, and metamorphic testing checks expected relationships between source and follow-up tests.

---

## Question 45

**Question:** Which test technique is often appropriate for complex AI-based systems with multiple parameters?

**Correct answer:**  
Pairwise testing is often appropriate for complex AI-based systems with multiple parameters.

**Syllabus rationale:**  
Pairwise testing reduces the number of combinations while still covering all pairs of parameter values. This is useful when exhaustive testing is not feasible due to many parameters or configurations.

---

## Quick revision rules

- Self-learning systems need monitoring and automated regression because behaviour can change.
- Autonomy testing checks when the system should operate alone and when it should hand control to a human.
- Bias testing may require additional data about sensitive or hidden attributes.
- LIME is model-agnostic and explains local predictions using input perturbations.
- Probabilistic systems need repeated runs and statistical or tolerance-based expected results.
- Complexity and lack of explainability can intensify the test oracle problem.
- Adversarial testing manipulates valid inputs to fool the trained model.
- Data poisoning manipulates training data.
- Exhaustive testing is impractical when there are many parameters or continuous values.
- Pairwise testing is the most common combinatorial testing technique.
- Back-to-back testing uses a pseudo-oracle or alternative implementation.
- A/B testing compares variants using user or operational behaviour.
- Metamorphic testing uses source tests, follow-up tests, and metamorphic relations.
- Experience-based testing includes error guessing, exploratory testing, and checklist-based testing.
- EDA examines data for patterns, relationships, trends, and outliers.
