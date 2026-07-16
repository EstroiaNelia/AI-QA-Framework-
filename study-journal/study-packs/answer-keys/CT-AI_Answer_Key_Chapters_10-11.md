# CT-AI Answer Key – Chapters 10–11

Suggested repository path:

```text
study-journal/study-packs/answer-keys/CT-AI_Answer_Key_Chapters_10-11.md
```

## Scope

Source practice set: `Questions_23_5.docx`  
Covered questions: 1 to 23  
Covered syllabus areas in the practice set: 10.1 to 11.6.2

## Notes

- The answers are written in English, by full meaning rather than only by option letter.
- The rationale is syllabus-oriented and focuses on why the answer is correct.
- Some practice questions use older CT-AI section numbering. The current CT-AI syllabus v2.0 reorganizes several topics. The concepts remain useful for revision.
- This block focuses mainly on virtual test environments, testing autonomy, AI for testing, defect triage, test generation, regression test optimization, defect prediction, and AI-based GUI/visual testing.

---

## Question 1

**Question:** An AI-powered fraud detection system is designed to adapt to new fraud patterns over time. The testing team wants to ensure that the system can handle unknown threats. What is the best way to test this system?

**Correct answer:**  
The best way is to introduce new and unpredictable fraud patterns.

**Syllabus rationale:**  
A system that adapts to new fraud patterns must be tested against scenarios that go beyond historical data. Using only past fraud cases would not provide sufficient evidence that the system can handle unknown or emerging threats.

---

## Question 2

**Question:** A self-driving car must decide when to hand control back to a human driver in dangerous situations. How should this be tested?

**Correct answer:**  
Testers should simulate extreme conditions to check whether the system hands control back to the human driver when appropriate.

**Syllabus rationale:**  
Autonomy testing must verify both independent operation and correct relinquishing of control. Dangerous or boundary conditions are especially important because they test whether the system recognizes when human intervention is needed.

---

## Question 3

**Question:** Which test environment setup best addresses the challenges of testing an autonomous drone operating in hazardous environments?

**Correct answer:**  
The best setup is a test environment that includes a variety of hazardous conditions, such as simulated storms, extreme temperatures, and variable terrain, and includes scenarios where the drone must decide whether to continue autonomously or cede control to a human operator.

**Syllabus rationale:**  
Testing autonomy requires realistic and challenging operational conditions, including cases near or beyond the limits of autonomous operation. The test environment must check both autonomous behaviour and correct handover to humans.

---

## Question 4

**Question:** Which virtual test environment is a simulator for generic mobile robot simulation?

**Correct answer:**  
Morse is a simulator for generic mobile robot simulation.

**Syllabus rationale:**  
Morse is used as a virtual test environment for mobile robotics. It supports simulation of robots and their interactions with environments.

---

## Question 5

**Question:** Which virtual test environment is designed to train embodied agents in photo-realistic 3D environments?

**Correct answer:**  
AI Habitat is designed to train embodied agents in photo-realistic 3D environments.

**Syllabus rationale:**  
AI Habitat provides simulation environments for embodied AI agents that need to navigate and act in realistic 3D scenes.

---

## Question 6

**Question:** What advantage does a virtual test environment offer in testing dangerous scenarios for AI-based systems?

**Correct answer:**  
A virtual test environment helps ensure the safety of humans involved in testing.

**Syllabus rationale:**  
Dangerous scenarios may be unsafe, expensive, or impractical to reproduce in the real world. Virtual test environments allow these scenarios to be tested without exposing humans to the same level of risk.

---

## Question 7

**Question:** Which benefit of using a virtual test environment is highlighted for testing extreme scenarios for AI-based systems?

**Correct answer:**  
A virtual test environment allows testers to simulate scenarios that are expensive or impossible to reproduce in reality.

**Syllabus rationale:**  
Extreme scenarios may be rare, dangerous, costly, or impossible to create physically. Simulation makes it possible to test those conditions in a controlled way.

---

## Question 8

**Question:** Which AI technology can be used to analyse and predict possible system failures using Bayesian techniques?

**Correct answer:**  
Fuzzy logic and probabilistic methods can be used to analyse and predict possible system failures using Bayesian techniques.

**Syllabus rationale:**  
Bayesian techniques are probabilistic methods. They can support reasoning under uncertainty, prediction of failures, and analysis of likely outcomes.

---

## Question 9

**Question:** Which AI technology can be used to solve optimization problems using a computational search of potentially large and complex search spaces?

**Correct answer:**  
Computational search and optimization techniques can be used to solve optimization problems in large and complex search spaces.

**Syllabus rationale:**  
Search and optimization techniques are used when there are many possible solutions and the goal is to find a good or optimal solution according to defined criteria.

---

## Question 10

**Question:** What role can machine learning models play in defect triage or analysis?

**Correct answer:**  
Machine learning models can identify critical defects based on their features.

**Syllabus rationale:**  
ML can analyse defect attributes, text, severity patterns, historical outcomes, and other features to support triage decisions such as priority, severity, or criticality.

---

## Question 11

**Question:** How can AI support defect triage or analysis in software development?

**Correct answer:**  
AI can support defect triage or analysis by categorizing defects and identifying duplicates.

**Syllabus rationale:**  
AI can analyse defect reports, classify them, identify similar or duplicate defects, and support prioritisation or routing decisions.

---

## Question 12

**Question:** What are the bases for generating tests using AI?

**Correct answer:**  
AI can generate tests based on source code, user interface, and test models.

**Syllabus rationale:**  
AI-based test generation may use different sources of information, including code, models, and user interfaces. These inputs can help generate candidate test cases or test paths.

---

## Question 13

**Question:** What is the test oracle problem in AI-based test generation?

**Correct answer:**  
The test oracle problem is that AI-based tools may generate test data or test cases but do not necessarily know what the expected results should be for that data.

**Syllabus rationale:**  
Generating test inputs is not the same as knowing the correct output. The test oracle problem remains relevant because a generated test case still needs an expected result or a mechanism to determine whether the result is correct.

---

## Question 14

**Question:** How can an AI-based tool optimize a regression test suite?

**Correct answer:**  
An AI-based tool can optimize a regression test suite by analysing previous test results, associated defects, and recent changes.

**Syllabus rationale:**  
Regression test optimization can use historical execution data, defect data, change information, and coverage information to select, prioritize, or reduce regression tests.

---

## Question 15

**Question:** What is the purpose of defect prediction?

**Correct answer:**  
The purpose of defect prediction is to prioritize testing based on the predicted number or likelihood of defects.

**Syllabus rationale:**  
Defect prediction helps teams focus test effort on areas that are more likely to contain defects. This supports risk-based testing and better allocation of limited test resources.

---

## Question 16

**Question:** Which metrics have been found to be the best predictors for defect prediction?

**Correct answer:**  
A combination of source code metrics and process metrics has been found to be the best predictor for defect prediction.

**Syllabus rationale:**  
Source code metrics describe properties of the code, such as size or complexity. Process metrics describe how the code has changed, such as change frequency or defect history. Combining both types generally provides stronger defect prediction than using only one type.

---

## Question 17

**Question:** What is a primary drawback of traditional scripted test automation using capture/playback with actual coordinates or software-defined objects?

**Correct answer:**  
A primary drawback is high sensitivity to interface changes, code changes, and platform changes.

**Syllabus rationale:**  
Capture/playback scripts can become brittle when the user interface or underlying object identification changes. This creates high maintenance effort and unstable automated tests.

---

## Question 18

**Question:** What are the drawbacks of using a capture/playback approach for scripted test automation?

**Correct answer:**  
The drawbacks include sensitivity to interface changes, code changes, and platform changes.

**Syllabus rationale:**  
Capture/playback approaches often depend on recorded actions, coordinates, object identifiers, or implementation details. When these change, scripts may fail even if the user-visible functionality still works.

---

## Question 19

**Question:** What is one advantage of using visual testing over traditional GUI-based testing?

**Correct answer:**  
Visual testing can be independent from the underlying technology.

**Syllabus rationale:**  
Visual testing analyses the appearance of the user interface, often through screenshots or image recognition. Because it focuses on the visual output, it can be less dependent on the implementation technology, object identifiers, or internal GUI structure.

---

## Question 20

**Question:** How does AI contribute to reducing the brittleness of the capture/playback approach in test automation?

**Correct answer:**  
AI can use historical data to choose stable identification criteria for GUI objects.

**Syllabus rationale:**  
AI-based test automation tools can learn which object identification attributes are more stable over time and can adjust locator strategies. This helps reduce brittleness when the UI changes.

---

## Question 21

**Question:** Which aspect of AI-based computer vision is highlighted as a potential tool for identifying issues with the visual appearance of a GUI?

**Correct answer:**  
AI-based computer vision can compare screenshots to detect unintended layout changes.

**Syllabus rationale:**  
Computer vision can be used in GUI testing to detect visual differences, layout regressions, rendering issues, or unintended changes in the appearance of the interface.

---

## Question 22

**Question:** What is one specific capability of AI-based regression testing tools?

**Correct answer:**  
AI-based regression testing tools can advise whether detected UI changes are acceptable to users.

**Syllabus rationale:**  
Some AI-based visual regression tools can assess whether visual differences are significant or acceptable, helping testers distinguish meaningful defects from harmless visual changes.

---

## Question 23

**Question:** What primary advantage do ML models provide in determining the acceptability of user interface screens?

**Correct answer:**  
ML models can automatically identify incorrectly rendered elements, inaccessible objects, and other visual issues.

**Syllabus rationale:**  
ML models can support GUI and visual testing by detecting visual anomalies, rendering problems, inaccessible elements, and other UI issues across platforms and devices. This can reduce manual inspection effort, although it does not eliminate the need for human judgement.

---

## Quick revision rules

- Test unknown threats with new and unpredictable scenarios, not only historical data.
- Autonomy testing must check both independent operation and correct handover to humans.
- Virtual test environments are useful for dangerous, rare, expensive, or impossible real-world scenarios.
- Morse is associated with generic mobile robot simulation.
- AI Habitat is associated with photo-realistic 3D environments for embodied agents.
- Bayesian techniques belong to probabilistic methods.
- Computational search and optimization techniques solve large search-space problems.
- AI can support defect triage by classifying, prioritising, and detecting duplicate defects.
- AI-based test generation still faces the test oracle problem.
- Regression test optimization uses history, defects, and recent changes to select or prioritize tests.
- Defect prediction supports risk-based testing by identifying defect-prone areas.
- Capture/playback automation is brittle because it is sensitive to UI, code, and platform changes.
- Visual testing is less dependent on the underlying implementation technology.
- AI can reduce locator brittleness by learning stable object identification criteria.
- Computer vision can detect unintended GUI layout or rendering changes.
