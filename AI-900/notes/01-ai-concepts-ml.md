# 01: AI Concepts and Machine Learning Fundamentals (Quiz-Ready)

This note is designed to fully cover Quiz 1 level questions without needing another source.

---

## 1) AI, ML, and Deep Learning

- Artificial Intelligence (AI): broad field of building systems that perform tasks requiring human-like intelligence.
- Machine Learning (ML): subset of AI where models learn patterns from data.
- Deep Learning (DL): subset of ML using multi-layer neural networks.

Think of the hierarchy as:
- AI includes ML.
- ML includes DL.

Exam shortcut:
- If a system learns from data, it is ML and therefore AI.

---

## 2) Types of Machine Learning

### Supervised learning
- Trains on labeled data (input plus known output).
- Used for prediction and classification.
- Examples: spam vs not spam, loan approve vs deny, price prediction.

### Unsupervised learning
- Trains on unlabeled data to discover hidden patterns.
- Used for clustering and segmentation.
- Examples: customer grouping, anomaly pattern discovery.

### Reinforcement learning
- Learns via actions, rewards, and penalties.
- Common in games, robotics, dynamic control.
- Less emphasized in AI-900 compared to supervised and unsupervised learning.

Decision rule:
- Has labels? Supervised.
- No labels and you want patterns/groups? Unsupervised.
- Agent learning by reward loops? Reinforcement.

---

## 3) Classification vs Regression vs Clustering

### Classification
- Predicts a category label.
- Output is discrete.
- Examples: fraud/not fraud, churn/not churn, disease class.

### Regression
- Predicts a numeric value.
- Output is continuous.
- Examples: house price, demand forecast, stock value.

### Clustering
- Groups similar items without labels.
- Example: customer segmentation.

Quick test:
- If answer is a number (price, amount, time), it is usually regression.
- If answer is a class/category, it is classification.

---

## 4) Common Algorithms and When to Use Them

| Algorithm | Task Type | Typical Use |
|---|---|---|
| Linear Regression | Regression | Predict continuous values |
| Logistic Regression | Classification | Binary or multiclass classification |
| Decision Tree | Classification/Regression | Interpretable rule-based modeling |
| Random Forest | Classification/Regression | Better generalization than single tree |
| K-Means | Unsupervised | Clustering similar records |
| Neural Networks | Multiple | Complex unstructured patterns (image/audio/text) |

Important exam distinctions:
- Linear Regression: for numeric output.
- Logistic Regression: for class output.
- Random Forest: reduces overfitting risk compared to one tree.
- Deep neural networks: powerful, but often need more data and compute.

---

## 5) Data Splits and Validation

Common split guideline:
- Training: 70-80%
- Validation: 10-15%
- Test: 10-15%

Purpose:
- Training: learn patterns.
- Validation: tune hyperparameters/model choices.
- Test: final unbiased performance check.

Why cross-validation is used:
- Repeats training/validation over multiple folds.
- Produces more reliable performance estimates.
- Helps detect unstable models and reduce overfitting risk.

---

## 6) Overfitting, Underfitting, and Generalization

### Overfitting
- High training score, much lower test score.
- Model memorizes training data noise.

Reduce overfitting by:
- Getting more diverse data.
- Simplifying model.
- Regularization.
- Better feature selection.

### Underfitting
- Low training score and low test score.
- Model too simple to learn true pattern.

Reduce underfitting by:
- Adding useful features.
- Increasing model capacity.
- Training longer when appropriate.

### Generalization
- Ability to perform well on unseen data.
- Good model: train and test performance are both strong and reasonably close.

---

## 7) Evaluation Metrics (Must Know)

### Confusion matrix terms
- True Positive (TP): predicted positive, actually positive.
- False Positive (FP): predicted positive, actually negative.
- True Negative (TN): predicted negative, actually negative.
- False Negative (FN): predicted negative, actually positive.

### Core classification metrics
- Accuracy = (TP + TN) / (TP + TN + FP + FN)
- Precision = TP / (TP + FP)
- Recall = TP / (TP + FN)
- F1-score = 2 x (Precision x Recall) / (Precision + Recall)

Interpretation:
- Precision asks: of predicted positives, how many were correct?
- Recall asks: of actual positives, how many did we find?
- F1 balances precision and recall.

When each matters:
- High recall priority: missing a positive is costly (for example, disease screening).
- High precision priority: false alarms are costly (for example, expensive manual review).
- Imbalanced classes: do not rely on accuracy alone; use precision, recall, and F1.

### Regression metrics
- MAE: average absolute error.
- MSE: average squared error.
- RMSE: square root of MSE; same unit as target variable.

---

## 8) Class Imbalance (Frequent Exam Trap)

Example:
- Fraud data with 99% non-fraud and 1% fraud.
- Predicting everything as non-fraud gives 99% accuracy but fails business goal.

What to do:
- Use precision, recall, F1, and confusion matrix.
- Focus on minority class detection performance.

---

## 9) Feature Engineering and Data Quality

Feature engineering:
- Creating/selecting meaningful input variables.
- Strong features can dramatically improve model quality.

Data quality issues that hurt models:
- Missing values
- Noisy labels
- Biased sampling
- Non-representative training data

Exam pattern:
- If model fails in a new environment, often training data is not representative.

---

## 10) Business and Responsible AI Context

Business value of ML:
- Better decisions, automation, personalization, forecasting, risk detection.

Common constraints:
- Limited data, limited compute, explainability requirements.

Responsible AI concerns:
- Bias and fairness: historical bias can be learned by models.
- Transparency: stakeholders should understand model impact.
- Accountability: humans remain responsible for decisions.

Exam-safe principle:
- AI should support human decision-making, not remove human accountability in high-impact domains.

---

## 11) Model Choice Under Constraints

If dataset is small and compute is limited:
- Prefer simpler models first (logistic regression, decision trees, basic ensembles).
- Avoid deep neural networks unless clearly justified.

If data is unstructured and large (images/audio/text):
- Neural networks are often strong candidates.

---

## 12) End-to-End ML Workflow (Order Matters)

1. Collect data
2. Preprocess/clean/prepare features
3. Train model
4. Evaluate and validate
5. Deploy
6. Monitor and retrain

Common mistake in exam questions:
- Evaluating before proper preprocessing or before train/validation split.

---

## 13) Quiz Mapping: What to Review for Each Question Type

- Q1-Q3: AI/ML hierarchy and learning types.
- Q4-Q6: task-to-algorithm matching and regression vs classification.
- Q7-Q9 and Q24: overfitting, underfitting, split strategy, generalization.
- Q10-Q12 and Q19 and Q23: confusion matrix, precision/recall/F1, imbalance traps.
- Q13-Q15: business use and responsible AI bias.
- Q16-Q17 and Q20: model selection trade-offs.
- Q21-Q22: feature engineering and cross-validation purpose.
- Q25: workflow sequence.

---

## 14) One-Page Rapid Revision

- Labels available -> Supervised.
- No labels, find groups -> Unsupervised.
- Reward loop agent -> Reinforcement.
- Numeric output -> Regression.
- Category output -> Classification.
- High train, low test -> Overfitting.
- Low train, low test -> Underfitting.
- Imbalanced data -> accuracy can mislead.
- Precision: correctness of positive predictions.
- Recall: coverage of actual positives.
- F1: balance of precision and recall.
- Reliable process: split data, validate, test once at end.

---

## Optional Deep-Dive Citations (Only if You Want More)

- Microsoft Learn AI-900 collection:
  - https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/
- Azure AI Fundamentals skills outline:
  - https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900
- scikit-learn model evaluation guide:
  - https://scikit-learn.org/stable/modules/model_evaluation.html
- scikit-learn cross-validation guide:
  - https://scikit-learn.org/stable/modules/cross_validation.html
- Responsible AI principles (Microsoft):
  - https://www.microsoft.com/ai/responsible-ai
