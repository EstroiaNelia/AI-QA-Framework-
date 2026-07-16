# CT-AI Answer Key – Chapters 3–4

Suggested repository path:

```text
study-journal/study-packs/answer-keys/CT-AI_Answer_Key_Chapters_3-4.md
```

## Scope

Source practice set: `Questions_36_2.docx`  
Covered questions: 1 to 36  
Covered syllabus areas in the practice set: 3.1 to 4.5.1

## Notes

- The answers are written in English, by full meaning rather than only by option letter.
- The rationale is syllabus-oriented and focuses on why the answer is correct.
- Some practice questions use older CT-AI section numbering. The concepts remain useful for revision, but the current CT-AI syllabus v2.0 has a different chapter structure.
- This block focuses mainly on machine learning forms, the ML workflow, data preparation, datasets, data quality, and labelling.

---

## Question 1

**Question:** Which of the following is not a category of ML algorithms?

**Correct answer:**  
Semi-supervised learning is not one of the three main ML algorithm categories emphasized in the CT-AI syllabus.

**Syllabus rationale:**  
The syllabus categorizes ML algorithms into supervised learning, unsupervised learning, and reinforcement learning. Semi-supervised learning exists as a machine learning approach in broader ML literature, but in this syllabus context the three main categories are supervised, unsupervised, and reinforcement learning.

---

## Question 2

**Question:** What is the purpose of supervised learning?

**Correct answer:**  
Supervised learning uses labelled data to train a model to map inputs to known outputs. In a classification context, this means classifying input data into predefined classes.

**Syllabus rationale:**  
In supervised learning, each training example has an expected output label. The model learns from these labelled examples and can then predict classes or numerical values for new data. In this question, the expected focus is classification into predefined classes.

---

## Question 3

**Question:** What is the purpose of unsupervised learning?

**Correct answer:**  
The purpose of unsupervised learning is to identify similarities, structures, or patterns in input data points without using predefined output labels.

**Syllabus rationale:**  
Unsupervised learning works with unlabelled data. It is commonly used for clustering similar data points or identifying associations between data items.

---

## Question 4

**Question:** What is the key characteristic of reinforcement learning?

**Correct answer:**  
Reinforcement learning learns from experience by interacting with an environment.

**Syllabus rationale:**  
In reinforcement learning, an agent interacts with its environment and receives rewards or penalties based on the outcome of its actions. The model improves by learning which actions lead to better results.

---

## Question 5

**Question:** What is the purpose of understanding the objectives in the machine learning workflow?

**Correct answer:**  
The purpose is to align the machine learning work with business priorities.

**Syllabus rationale:**  
The ML workflow starts by understanding and agreeing the purpose of the ML model with stakeholders. This ensures that acceptance criteria and performance metrics are aligned with business goals.

---

## Question 6

**Question:** During the “Understand the Objectives” phase, which action should a retail company take to align an AI-based recommendation system with business priorities?

**Correct answer:**  
The team should define clear acceptance criteria and functional performance metrics with stakeholders to measure the success of the recommendation system.

**Syllabus rationale:**  
The “Understand the Objectives” phase is about clarifying the business purpose of the model, agreeing what success means, and defining measurable acceptance criteria. Collecting data, selecting algorithms, and training models happen later.

---

## Question 7

**Question:** Based on what should the framework be selected for AI development?

**Correct answer:**  
The AI development framework should be selected based on the available data, the objectives, and the acceptance criteria.

**Syllabus rationale:**  
Framework selection should be driven by the needs of the ML solution. The type and amount of available data, the model objectives, and the agreed acceptance criteria influence which development framework is appropriate.

---

## Question 8

**Question:** What is the purpose of data preparation in the machine learning workflow?

**Correct answer:**  
The purpose of data preparation is to clean and modify data so that it is suitable for model training, evaluation, and testing.

**Syllabus rationale:**  
Data preparation transforms raw data into a usable format. It includes activities such as data acquisition, preprocessing, cleaning, transformation, feature engineering, and preparation of data for ML use.

---

## Question 9

**Question:** What are model hyperparameters?

**Correct answer:**  
Model hyperparameters are parameters set before or during training that influence the structure or training behaviour of the model.

**Syllabus rationale:**  
Hyperparameters are not learned directly from the training data in the same way as model parameters. They control how the model is built or trained, such as the number of layers in a neural network, the depth of a decision tree, or the number of training iterations.

---

## Question 10

**Question:** What is the purpose of model evaluation and tuning?

**Correct answer:**  
The purpose is to assess the model against agreed performance metrics and adjust the model settings to improve its performance.

**Syllabus rationale:**  
During evaluation, the model is assessed using validation data and agreed ML functional performance metrics. During tuning, model or algorithm hyperparameters are adjusted and the model is retrained to improve performance.

---

## Question 11

**Question:** What is the final step in the machine learning workflow?

**Correct answer:**  
The final step is to monitor and tune the model.

**Syllabus rationale:**  
After deployment and use, the model must continue to be monitored. Monitoring helps identify degradation, drift, or changing operational conditions, and may trigger further tuning or retraining.

---

## Question 12

**Question:** During the “Test the Model” phase of a real-time fraud detection ML system, which step is crucial to validate that the model performs well in real-world conditions?

**Correct answer:**  
The model should be tested against an independent test dataset, and the performance metrics should be compared with those obtained during the evaluation phase.

**Syllabus rationale:**  
The independent test dataset is used after model generation and tuning to verify that the agreed ML functional performance criteria are met. If test performance is significantly worse than evaluation performance, this may indicate poor generalization.

---

## Question 13

**Question:** Which activity is not part of the machine learning workflow?

**Correct answer:**  
Integrating the model with non-ML parts of the system is not part of the core ML workflow.

**Syllabus rationale:**  
The ML workflow focuses on activities such as understanding objectives, selecting and building the algorithm, preparing and testing data, training, evaluating, tuning, testing, deploying, using, and monitoring the model. Integration with non-ML system components belongs to the broader system development and integration context.

---

## Question 14

**Question:** Which statement is correct about model tuning?

**Correct answer:**  
Hyperparameter tuning changes settings that affect the model or training process, such as the number of neurons in a neural network or the number of training iterations.

**Syllabus rationale:**  
Tuning uses evaluation results to adjust model hyperparameters and algorithm hyperparameters. These settings influence the structure of the model and the way training is performed.

---

## Question 15

**Question:** What is necessary for supervised learning?

**Correct answer:**  
Properly labelled data is necessary for supervised learning.

**Syllabus rationale:**  
Supervised learning requires training examples where the expected output is known. These labels allow the model to learn the relationship between input data and output results.

---

## Question 16

**Question:** What type of ML approach is suitable for finding co-occurring data items?

**Correct answer:**  
Association is suitable for finding co-occurring data items.

**Syllabus rationale:**  
Association is an unsupervised learning approach used to identify relationships or dependencies among data attributes, such as products that are frequently bought together.

---

## Question 17

**Question:** What factor should not, according to the syllabus context, be considered when selecting an ML algorithm, model settings, and model hyperparameters?

**Correct answer:**  
Previous experience should not be the main factor for selecting the ML algorithm, model settings, and model hyperparameters.

**Syllabus rationale:**  
The selection should be based on the required functionality, objectives, acceptance criteria, available data, characteristics of the input data, performance needs, and constraints. Previous experience may be useful background information, but it should not override the actual problem and data characteristics.

---

## Question 18

**Question:** Why is the amount of data available an important factor in selecting an ML model?

**Correct answer:**  
The amount of available data is important because it affects the accuracy and reliability of the model.

**Syllabus rationale:**  
Some ML models require more data than others to learn reliable patterns. If there is too little data, the model may not generalize well and may produce inaccurate predictions.

---

## Question 19

**Question:** For a transportation company that needs real-time predictions and high accuracy for vehicle maintenance, which factors should be prioritized when selecting the ML algorithm?

**Correct answer:**  
The company should choose an algorithm known for high accuracy and fast prediction, even if it requires more memory and slower training times.

**Syllabus rationale:**  
The scenario prioritizes real-time predictions and high accuracy. Training time is less critical than inference speed and prediction quality in an operational predictive maintenance use case.

---

## Question 20

**Question:** What is underfitting in machine learning?

**Correct answer:**  
Underfitting occurs when the model is not sophisticated enough to fit the patterns in the data.

**Syllabus rationale:**  
An underfitted model is too simple or insufficiently trained to capture the underlying patterns in the data. It usually performs poorly on both training data and test data.

---

## Question 21

**Question:** Which activity in the ML workflow is probably the most resource-intensive?

**Correct answer:**  
Data preparation is probably the most resource-intensive activity in the ML workflow.

**Syllabus rationale:**  
Data preparation often consumes a significant proportion of the ML development effort because it includes acquiring, cleaning, transforming, validating, and preparing data for model training and prediction.

---

## Question 22

**Question:** Which activity is not part of the data preparation process?

**Correct answer:**  
Model selection and building is not part of the data preparation process.

**Syllabus rationale:**  
Data preparation includes activities such as data acquisition, data preprocessing, data cleaning, transformation, augmentation, sampling, and feature engineering. Model selection and building belongs to the model generation part of the workflow.

---

## Question 23

**Question:** What is the purpose of data preprocessing in the machine learning workflow?

**Correct answer:**  
The purpose of data preprocessing is to change the format of the data and handle missing values.

**Syllabus rationale:**  
Data preprocessing includes cleaning data, imputing missing values, transforming formats, scaling, normalization, anonymization, and preparing raw data for ML use.

---

## Question 24

**Question:** What is the purpose of data augmentation?

**Correct answer:**  
The purpose of data augmentation is to increase the number of samples in a dataset.

**Syllabus rationale:**  
Data augmentation creates additional data samples, often by transforming existing data or generating synthetic data. This can improve model training and robustness when suitable.

---

## Question 25

**Question:** What is the purpose of feature selection in data preparation?

**Correct answer:**  
Feature selection aims to reduce overall training time and help prevent overfitting by selecting the most relevant features.

**Syllabus rationale:**  
Feature selection keeps the features that contribute most to model performance and removes irrelevant or redundant features. This can reduce noise, improve generalization, and reduce computational cost.

---

## Question 26

**Question:** In a customer churn ML model with numerical, categorical, and time-series data, what should be prioritized during data preprocessing?

**Correct answer:**  
The team should conduct data imputation to replace missing values with estimated values and apply data transformation techniques such as scaling and normalization.

**Syllabus rationale:**  
The scenario asks about data preprocessing. Imputation, scaling, normalization, and format transformation are preprocessing activities that improve data consistency and suitability for the model.

---

## Question 27

**Question:** What is the purpose of performing data preparation steps?

**Correct answer:**  
The purpose is to produce a dataset that is suitable for creating a classification model.

**Syllabus rationale:**  
Data preparation transforms raw data into a usable dataset for model development. In this question, the target use is creating a classification model.

---

## Question 28

**Question:** What are the three sets of equivalent data required to develop an ML model?

**Correct answer:**  
The three sets are the training dataset, validation dataset, and test dataset.

**Syllabus rationale:**  
Training data is used to train the model. Validation data is used to evaluate and tune it during model development. Test data is kept independent and used to assess the final model.

---

## Question 29

**Question:** What is the purpose of keeping the test dataset separate and not using it during training?

**Correct answer:**  
The purpose is to ensure that the developed model is not influenced by the test data.

**Syllabus rationale:**  
The test dataset must remain independent so it can provide an unbiased assessment of the model’s performance on unseen data. Using it during training would create data leakage and inflate performance estimates.

---

## Question 30

**Question:** Which step is necessary before training and testing a classification model using supervised learning with datasets?

**Correct answer:**  
The data must be split into training, validation, and test datasets.

**Syllabus rationale:**  
Before supervised model training and testing, the available labelled data should be separated into appropriate datasets. This supports training, tuning, and independent final testing.

---

## Question 31

**Question:** For a pharmaceutical company with scarce data, which data splitting strategy should be adopted?

**Correct answer:**  
The team should combine the training and validation datasets and use K-fold cross-validation to generate multiple split combinations for training and tuning the model, while keeping the test dataset separate.

**Syllabus rationale:**  
When data is scarce, K-fold cross-validation helps use the available training and validation data more efficiently. However, the test dataset should still remain separate to provide an independent final evaluation.

---

## Question 32

**Question:** What is an example of wrong data in a dataset?

**Correct answer:**  
Data entered incorrectly is an example of wrong data.

**Syllabus rationale:**  
Wrong data refers to data values that are incorrect. Missing data, insufficient data, and obsolete data are different data quality problems.

---

## Question 33

**Question:** What can cause a biased model in machine learning?

**Correct answer:**  
Unfair data can cause a biased model.

**Syllabus rationale:**  
If the data used for training is unfair, unrepresentative, or reflects inappropriate historical bias, the model can learn and reproduce that bias.

---

## Question 34

**Question:** What type of defect can be caused by data privacy and security restrictions?

**Correct answer:**  
Data privacy and security restrictions can cause reduced accuracy.

**Syllabus rationale:**  
Privacy and security restrictions may limit access to relevant data or require data to be anonymized or removed. This can reduce the amount or quality of available training data and negatively affect model accuracy.

---

## Question 35

**Question:** What is data labelling?

**Correct answer:**  
Data labelling is the process of enriching unlabelled data by adding labels for use in supervised learning.

**Syllabus rationale:**  
Supervised learning requires labelled data. Labelling provides the expected outputs or classes that the model uses during training.

---

## Question 36

**Question:** How is AI-assisted data labelling different from other approaches?

**Correct answer:**  
In AI-assisted data labelling, AI-based tools recognize and annotate data, and a human confirms or modifies the results.

**Syllabus rationale:**  
AI-assisted labelling combines automated annotation with human review. This differs from internal, outsourced, or crowdsourced labelling because the AI tool proposes labels and humans validate or correct them.

---

## Quick revision rules

- Supervised learning uses labelled data.
- Unsupervised learning finds patterns in unlabelled data.
- Reinforcement learning learns by interacting with an environment and receiving rewards or penalties.
- The ML workflow starts with understanding objectives and acceptance criteria.
- Data preparation is usually one of the most resource-intensive ML activities.
- Hyperparameters are set before or during training and influence model structure or training behaviour.
- Model evaluation uses validation data; final model testing uses independent test data.
- Keep the test dataset separate to avoid data leakage.
- Underfitting means the model is too simple to capture the patterns in the data.
- Data preprocessing includes cleaning, missing value handling, transformation, scaling, and normalization.
- Data augmentation increases the number of samples.
- Feature selection removes irrelevant or redundant features.
- Data labelling adds labels to unlabelled data for supervised learning.
- AI-assisted labelling uses AI to propose annotations and humans to confirm or correct them.
