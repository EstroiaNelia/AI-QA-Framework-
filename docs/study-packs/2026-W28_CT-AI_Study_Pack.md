# CT-AI Study Pack – 2026-W28

## Focus of the Week

Chapter 7 – AI-Specific Testing Techniques

## Purpose

This Study Pack is designed to consolidate the most difficult concepts identified during the first week of CT-AI preparation.

The main goal is to understand when and why specific AI testing techniques are used, especially when traditional expected results are difficult to define.

---

## Weekly Study Plan

### Monday

Study the Test Oracle Problem.

### Tuesday

Study Metamorphic Testing.

### Wednesday

Study Back-to-Back Testing and A/B Testing.

### Thursday

Study Adversarial Testing and Data Poisoning.

### Friday

Study Virtual Test Environments, Defect Prediction and Regression Test Optimization.

### Weekend

Review flashcards, answer practice questions and repeat quiz questions related to Chapter 7.

---

# 1. Test Oracle Problem

## Definition

A test oracle is a mechanism used to determine whether the result of a test is correct.

The Test Oracle Problem occurs when it is difficult or impossible to determine the expected result of a test.

## Simple explanation

In traditional software testing, the expected result is often clear.

Example:

Input:

```text
2 + 2
```

Expected result:

```text
4
```

In AI systems, the expected result may not be obvious.

Example:

Input:

```text
Image of an animal
```

Model output:

```text
Cat, with 78% confidence
```

Questions:

- Is the answer correct?
- Is 78% confidence enough?
- What if the image is ambiguous?
- What if another model predicts "lynx"?
- What if a human expert disagrees?

This is the Test Oracle Problem.

## Why it matters in AI Testing

AI systems often produce probabilistic outputs. They may not always return the same type of clear, deterministic answer as traditional software.

This makes it harder to define a simple expected result.

## Typical solutions

When the exact expected result is difficult to define, testers may use:

- Metamorphic Testing
- Back-to-Back Testing
- A/B Testing
- Statistical Testing
- Benchmark datasets
- Human expert review
- Thresholds and acceptance criteria
- Comparison with a reference model

## Exam clue

If the question says that the expected result is difficult to determine, think about:

```text
Test Oracle Problem
```

---

# 2. Metamorphic Testing

## Definition

Metamorphic Testing is a technique used when the exact expected result is unknown, but relationships between inputs and outputs are known.

These relationships are called metamorphic relations.

## Simple explanation

Sometimes we do not know the exact answer, but we know how the answer should behave if we change the input.

## Example 1 – Image classification

Original input:

```text
Image of a cat
```

Model output:

```text
Cat
```

Modified input:

```text
Same image, slightly brighter
```

Expected relation:

```text
The model should still classify it as a cat.
```

We do not need to know the exact confidence score, but we expect the classification to remain stable.

## Example 2 – Route recommendation

Original input:

```text
Calculate route from A to B
```

Modified input:

```text
Calculate route from A to B with one irrelevant road renamed
```

Expected relation:

```text
The route should not change significantly.
```

## Example 3 – Search engine

Original input:

```text
Search for "hotels in Lisbon"
```

Modified input:

```text
Search for "hotels in Lisboa"
```

Expected relation:

```text
The results should be similar.
```

## Why it matters

Metamorphic Testing is useful because many AI systems do not have one exact expected output.

Instead of checking one expected result, we check whether the model behaves consistently when inputs are changed in controlled ways.

## Exam clue

If the question says:

```text
The exact expected result is unknown, but relationships between inputs and outputs can be checked.
```

The answer is probably:

```text
Metamorphic Testing
```

---

# 3. Back-to-Back Testing

## Definition

Back-to-Back Testing compares the outputs of two or more systems, models or versions using the same inputs.

## Simple explanation

The same input is executed against different models or versions. The results are compared.

## Example

Input:

```text
Customer support ticket
```

Model A output:

```text
High priority
```

Model B output:

```text
Critical
```

The tester analyses the difference and decides whether it is acceptable.

## Typical use cases

Back-to-Back Testing is useful when:

- comparing an old model with a new model;
- validating a new implementation against a reference implementation;
- comparing models from different vendors;
- checking whether a new model version introduces regressions.

## Difference from Metamorphic Testing

Metamorphic Testing changes the input and checks expected relationships.

Back-to-Back Testing keeps the input the same and compares different systems or versions.

## Exam clue

If the question mentions comparison between two models, two versions or two implementations, think about:

```text
Back-to-Back Testing
```

---

# 4. A/B Testing

## Definition

A/B Testing compares two or more variants in a real or controlled environment to determine which performs better.

## Simple explanation

A group of users receives version A. Another group receives version B. The results are compared using defined metrics.

## Example

An e-commerce platform wants to test a new recommendation model.

Version A:

```text
Current recommendation model
```

Version B:

```text
New AI-based recommendation model
```

Metrics:

- click-through rate;
- conversion rate;
- revenue;
- user engagement;
- complaint rate.

## Why it matters

A/B Testing is useful to validate whether a model performs better in practice, with real users or realistic operational data.

## Risks

A/B Testing must be carefully controlled because users may be exposed to a weaker, biased or risky model.

## Difference from Back-to-Back Testing

Back-to-Back Testing compares outputs for the same test inputs.

A/B Testing compares variants through user behaviour or operational metrics.

## Exam clue

If the question mentions real users, production traffic, variants A and B, or business metrics, think about:

```text
A/B Testing
```

---

# 5. Pairwise Testing

## Definition

Pairwise Testing is a combinatorial testing technique where combinations of input parameters are selected so that every pair of values is tested at least once.

## Simple explanation

Instead of testing all possible combinations, Pairwise Testing reduces the number of tests while still covering relevant interactions between pairs of variables.

## Example

A model is tested with these parameters:

```text
Browser: Chrome, Edge, Firefox
Device: Desktop, Mobile
Language: Portuguese, English
User type: New, Returning
```

Testing all combinations may be expensive.

Pairwise Testing reduces the number of combinations while still covering all pairs.

## Why it matters in AI Testing

AI systems may have many input variables, configurations and environmental conditions. Pairwise Testing helps reduce test effort.

## Exam clue

If the question mentions reducing combinations while maintaining coverage of parameter interactions, think about:

```text
Pairwise Testing
```

---

# 6. Statistical Testing

## Definition

Statistical Testing evaluates the behaviour of a system using statistical methods, distributions, confidence levels or thresholds.

## Simple explanation

Instead of checking one individual result, Statistical Testing analyses patterns across many results.

## Example

A fraud detection model is tested with 10,000 transactions.

The tester does not check each prediction manually. Instead, the tester analyses:

- Precision;
- Recall;
- false positive rate;
- false negative rate;
- confidence intervals;
- distribution of predictions.

## Why it matters

AI models are often evaluated statistically because their behaviour is probabilistic.

## Exam clue

If the question mentions statistical significance, distributions, confidence levels or large sample evaluation, think about:

```text
Statistical Testing
```

---

# 7. Adversarial Testing

## Definition

Adversarial Testing evaluates how a model behaves when inputs are intentionally manipulated to mislead it.

## Simple explanation

The tester tries to trick the model.

## Example 1 – Image recognition

A small perturbation is added to an image.

To a human, the image still looks like a stop sign.

The model classifies it as:

```text
Speed limit sign
```

## Example 2 – Spam detection

An attacker changes the wording of a spam email slightly to avoid detection.

Original:

```text
Win money now
```

Modified:

```text
W1n m0ney n0w
```

The model may fail to classify it as spam.

## Why it matters

AI systems can be vulnerable to manipulated inputs. Adversarial Testing helps assess robustness and security.

## Exam clue

If the question mentions manipulated inputs designed to fool the model, think about:

```text
Adversarial Testing
```

---

# 8. Data Poisoning

## Definition

Data Poisoning is an attack where training data is intentionally corrupted to influence the behaviour of a model.

## Simple explanation

The attacker does not attack the model directly at prediction time. Instead, the attacker compromises the data used to train the model.

## Example

A recommendation model is trained using product reviews.

An attacker adds many fake positive reviews for a low-quality product.

The model learns that the product should be recommended more often.

## Difference from Adversarial Attack

Adversarial attacks usually manipulate the input at prediction time.

Data poisoning manipulates the training data before or during model training.

## Exam clue

If the question mentions corrupted or manipulated training data, think about:

```text
Data Poisoning
```

---

# 9. Virtual Test Environments

## Definition

A Virtual Test Environment is a simulated environment used to test AI-based systems under controlled or complex conditions.

## Simple explanation

Instead of testing only in the real world, testers use simulations.

## Example

An autonomous vehicle is tested in a virtual city.

The test environment can simulate:

- rain;
- fog;
- night driving;
- pedestrians;
- unexpected obstacles;
- dangerous road conditions.

## Why it matters

Some AI systems are difficult, expensive or unsafe to test only in real environments.

Virtual Test Environments allow testers to create repeatable and controlled scenarios.

## Exam clue

If the question mentions simulation, controlled scenarios, safety-critical systems or virtual environments, think about:

```text
Virtual Test Environments
```

---

# 10. Defect Prediction

## Definition

Defect Prediction uses AI or ML techniques to predict which parts of a system are more likely to contain defects.

## Simple explanation

The AI supports testing by helping testers decide where to focus.

## Example

A model analyses historical defect data and identifies that a specific module has a high probability of defects.

The test team gives higher priority to that module.

## Data that may be used

- historical defects;
- code complexity;
- change frequency;
- developer activity;
- previous incidents;
- test results.

## Why it matters

Defect Prediction helps improve test prioritisation and risk-based testing.

## Exam clue

If the question mentions predicting defect-prone areas, think about:

```text
Defect Prediction
```

---

# 11. Regression Test Optimization

## Definition

Regression Test Optimization uses techniques, sometimes AI-based, to select, prioritise or reduce regression tests.

## Simple explanation

The goal is to run the most relevant regression tests first or avoid running unnecessary tests.

## Example

After a code change, an AI-based tool analyses previous executions and decides:

- which tests are most likely to fail;
- which tests cover the changed area;
- which tests should run first;
- which tests can be skipped with low risk.

## Why it matters

Regression test suites can become large and expensive. Optimization helps save time while maintaining confidence.

## Exam clue

If the question mentions selecting, prioritising or reducing regression tests, think about:

```text
Regression Test Optimization
```

---

# Technique Comparison Table

| Situation | Most likely technique |
|---|---|
| Expected result is difficult to define | Test Oracle Problem |
| Exact expected output is unknown, but relations are known | Metamorphic Testing |
| Same input is compared across two models or versions | Back-to-Back Testing |
| Two variants are compared with users or operational metrics | A/B Testing |
| Test combinations need to be reduced | Pairwise Testing |
| Behaviour is evaluated across many results | Statistical Testing |
| Inputs are manipulated to fool the model | Adversarial Testing |
| Training data is corrupted | Data Poisoning |
| Dangerous or complex scenarios are simulated | Virtual Test Environment |
| AI predicts where defects are likely to occur | Defect Prediction |
| AI selects or prioritises regression tests | Regression Test Optimization |

---

# Common Exam Traps

## Trap 1

Question:

```text
The expected output is unknown, but the tester knows that changing the input in a specific way should not significantly change the output.
```

Correct concept:

```text
Metamorphic Testing
```

Not:

```text
Back-to-Back Testing
```

Reason:

The input is changed and a relation is checked.

## Trap 2

Question:

```text
The same input is executed against the current model and the new model, and the outputs are compared.
```

Correct concept:

```text
Back-to-Back Testing
```

Not:

```text
Metamorphic Testing
```

Reason:

The input is the same. The models or versions are different.

## Trap 3

Question:

```text
A new recommendation algorithm is shown to 10% of users and compared with the existing algorithm.
```

Correct concept:

```text
A/B Testing
```

Reason:

The comparison uses different variants and user behaviour.

## Trap 4

Question:

```text
Small changes are added to an image so that a model misclassifies it.
```

Correct concept:

```text
Adversarial Testing
```

Reason:

The input is intentionally manipulated to mislead the model.

## Trap 5

Question:

```text
Incorrect samples are inserted into the training data to influence the model.
```

Correct concept:

```text
Data Poisoning
```

Reason:

The attack affects the training data.

---

# Practical QA Examples

## Example 1 – Support ticket prioritisation

AI system:

```text
Classifies support tickets as Low, Medium, High or Critical.
```

Relevant risks:

- Critical tickets may be classified as High.
- Similar tickets may receive inconsistent classifications.
- Training data may reflect historical bias.
- New types of incidents may cause concept drift.

Relevant techniques:

- ML Model Testing
- Back-to-Back Testing
- Metamorphic Testing
- Bias Detection
- Continuous Monitoring

## Example 2 – Fraud detection

AI system:

```text
Classifies financial transactions as fraudulent or non-fraudulent.
```

Relevant risks:

- High false negatives may allow fraud.
- High false positives may block legitimate users.
- Fraud patterns may change over time.
- Attackers may adapt to the model.

Relevant techniques:

- Confusion Matrix
- Precision
- Recall
- F1-Score
- Adversarial Testing
- Concept Drift Monitoring

## Example 3 – Recommendation system

AI system:

```text
Recommends products to users.
```

Relevant risks:

- Biased recommendations.
- Poor recommendations for new users.
- Manipulated reviews.
- Performance degradation over time.

Relevant techniques:

- A/B Testing
- Statistical Testing
- Data Poisoning checks
- Monitoring
- Bias Detection

---

# Mini Flashcards

## Flashcard 1

Q: What is a test oracle?

A: A mechanism used to determine whether the result of a test is correct.

## Flashcard 2

Q: What is the Test Oracle Problem?

A: The difficulty of determining the expected result of a test.

## Flashcard 3

Q: Why is the Test Oracle Problem common in AI systems?

A: Because AI systems often produce probabilistic, complex or non-deterministic outputs.

## Flashcard 4

Q: What is Metamorphic Testing?

A: A testing technique that checks expected relationships between inputs and outputs when the exact expected result is unknown.

## Flashcard 5

Q: What is Back-to-Back Testing?

A: A technique that compares outputs from different models, versions or systems using the same inputs.

## Flashcard 6

Q: What is A/B Testing?

A: A technique that compares variants using real or controlled user behaviour and defined metrics.

## Flashcard 7

Q: What is Adversarial Testing?

A: Testing that evaluates whether manipulated inputs can mislead a model.

## Flashcard 8

Q: What is Data Poisoning?

A: An attack where training data is corrupted to influence model behaviour.

## Flashcard 9

Q: What is a Virtual Test Environment?

A: A simulated environment used to test AI systems under controlled or complex scenarios.

## Flashcard 10

Q: What is Defect Prediction?

A: The use of AI or ML to predict which parts of a system are more likely to contain defects.

## Flashcard 11

Q: What is Regression Test Optimization?

A: The selection, prioritisation or reduction of regression tests to improve efficiency.

---

# Practice Questions

## Question 1

A tester cannot determine the exact expected output of an AI model. However, the tester knows that rotating an image slightly should not change its classification.

Which technique is most appropriate?

A. Back-to-Back Testing  
B. Metamorphic Testing  
C. A/B Testing  
D. Regression Test Optimization  

Correct answer:

```text
B. Metamorphic Testing
```

Reason:

The exact expected output is unknown, but an expected relationship between input and output exists.

---

## Question 2

The same dataset is executed against two versions of a model. The outputs are compared to identify behavioural differences.

Which technique is being used?

A. Back-to-Back Testing  
B. Pairwise Testing  
C. Adversarial Testing  
D. Data Poisoning  

Correct answer:

```text
A. Back-to-Back Testing
```

Reason:

The same inputs are compared across two versions.

---

## Question 3

A model is tested with inputs that have been intentionally modified to mislead it.

Which type of testing is this?

A. Statistical Testing  
B. A/B Testing  
C. Adversarial Testing  
D. Defect Prediction  

Correct answer:

```text
C. Adversarial Testing
```

Reason:

The goal is to assess whether manipulated inputs can fool the model.

---

## Question 4

An attacker inserts incorrect examples into the training data so that the model learns incorrect behaviour.

Which risk does this describe?

A. Concept Drift  
B. Data Poisoning  
C. Automation Bias  
D. Underfitting  

Correct answer:

```text
B. Data Poisoning
```

Reason:

The training data is intentionally corrupted.

---

## Question 5

A company releases a new recommendation model to 20% of users and compares conversion rate against the current model.

Which technique is being used?

A. Pairwise Testing  
B. Back-to-Back Testing  
C. A/B Testing  
D. Metamorphic Testing  

Correct answer:

```text
C. A/B Testing
```

Reason:

Different variants are compared using user behaviour and business metrics.

---

## Question 6

An autonomous driving system is tested in a simulated city with rain, fog and pedestrians.

Which test environment is being used?

A. Virtual Test Environment  
B. Back-to-Back Testing  
C. Benchmark Suite  
D. Human Oracle  

Correct answer:

```text
A. Virtual Test Environment
```

Reason:

The system is being tested in a simulated controlled environment.

---

## Question 7

An AI tool analyses historical defect data and identifies modules that are more likely to fail.

Which activity does this describe?

A. Defect Prediction  
B. Data Poisoning  
C. Metamorphic Testing  
D. Adversarial Testing  

Correct answer:

```text
A. Defect Prediction
```

Reason:

AI is being used to predict defect-prone areas.

---

## Question 8

An AI-based tool selects which regression tests should run first after a code change.

Which activity does this describe?

A. A/B Testing  
B. Regression Test Optimization  
C. Pairwise Testing  
D. Concept Drift  

Correct answer:

```text
B. Regression Test Optimization
```

Reason:

The regression suite is being selected or prioritised.

---

## Question 9

A tester wants to reduce the number of test combinations while ensuring that every pair of parameter values is covered at least once.

Which technique is most appropriate?

A. Pairwise Testing  
B. Statistical Testing  
C. Back-to-Back Testing  
D. Test Oracle Problem  

Correct answer:

```text
A. Pairwise Testing
```

Reason:

Pairwise Testing reduces combinations while maintaining coverage of value pairs.

---

## Question 10

A model is evaluated across thousands of predictions using Precision, Recall, F1-Score and confidence intervals.

Which approach is being used?

A. Statistical Testing  
B. A/B Testing  
C. Data Poisoning  
D. Virtual Test Environment  

Correct answer:

```text
A. Statistical Testing
```

Reason:

The model is being evaluated using aggregate statistical evidence.

---

# End-of-Week Self-Assessment

Use this checklist at the end of the week.

## I can explain

- [ ] What the Test Oracle Problem is.
- [ ] Why the Test Oracle Problem is common in AI systems.
- [ ] What Metamorphic Testing is.
- [ ] How Metamorphic Testing differs from Back-to-Back Testing.
- [ ] When A/B Testing is appropriate.
- [ ] What Adversarial Testing checks.
- [ ] The difference between Adversarial Testing and Data Poisoning.
- [ ] What a Virtual Test Environment is.
- [ ] How AI can support Defect Prediction.
- [ ] How AI can support Regression Test Optimization.

## I can identify the right technique

- [ ] Unknown expected result with known relations: Metamorphic Testing.
- [ ] Comparing two model versions: Back-to-Back Testing.
- [ ] Comparing variants with users: A/B Testing.
- [ ] Reducing parameter combinations: Pairwise Testing.
- [ ] Manipulated inputs: Adversarial Testing.
- [ ] Corrupted training data: Data Poisoning.
- [ ] Simulated scenarios: Virtual Test Environment.
- [ ] Predicting defect-prone areas: Defect Prediction.
- [ ] Selecting regression tests: Regression Test Optimization.

---

# Link to the AI QA Framework

Possible future framework elements:

- Oracle strategy for AI systems.
- Catalogue of AI-specific testing techniques.
- Checklist for selecting testing techniques.
- Risk catalogue for adversarial attacks and data poisoning.
- Monitoring strategy for production models.
- Guidance for regression test optimization using AI.

These items should remain secondary for now. The priority is CT-AI exam preparation.

---

# Final Revision Notes

The most important distinction for this week is:

```text
Metamorphic Testing changes the input and checks expected relationships.
Back-to-Back Testing keeps the input and compares different systems or versions.
A/B Testing compares variants using user or operational behaviour.
Adversarial Testing tries to fool the model.
Data Poisoning corrupts the training data.
```

This distinction is likely to be useful in exam questions.
