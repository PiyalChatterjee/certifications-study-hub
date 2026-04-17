# Quiz 1: AI Concepts & Machine Learning Fundamentals

**Instructions:** Answer all 25 questions. Mark your answers, then scroll to the bottom for scoring & explanations.

---

## Questions

### **Q1: Relationship Between AI, ML, and Deep Learning**
A company wants to build a system that learns to recognize objects in images without being explicitly programmed. Which statement best describes this?

A) This is AI but not ML
B) This is ML but not AI  
C) This is both AI and ML (correct)
D) This is only Deep Learning, not AI or ML  

---

### **Q2: Types of Learning - Spam Detection**
An email system learns to filter spam by analyzing 10,000 emails labeled as "spam" or "not spam." What type of learning is this?

A) Unsupervised Learning  
B) Supervised Learning (correct)
C) Reinforcement Learning  
D) Semi-supervised Learning  

---

### **Q3: Types of Learning - Customer Segmentation**
A retail company wants to discover hidden customer groups based on purchase history (no predefined categories). What approach should they use?

A) Supervised Learning  
B) Unsupervised Learning (correct)
C) Reinforcement Learning  
D) Transfer Learning  

---

### **Q4: Choosing an Algorithm**
You need to predict house prices based on square footage, bedrooms, and location. Which algorithm is most appropriate?

A) K-Means Clustering  
B) Linear Regression (correct)
C) Logistic Regression  
D) Decision Tree (for classification only)  

---

### **Q5: Choosing an Algorithm**
A bank wants to classify loan applications as "approved" or "denied" based on applicant data. Which algorithm fits best?

A) Linear Regression  
B) Logistic Regression (correct)
C) K-Means Clustering  
D) Random Forest (ensemble only)  

---

### **Q6: Classification vs. Regression**
Which of these is a regression problem?

A) Predicting if a customer will churn (leave)  
B) Predicting the stock price next month (correct)
C) Categorizing emails as important or spam
D) Identifying disease types from medical scans  

---

### **Q7: Overfitting Scenario**
A model achieves 99% accuracy on training data but only 65% accuracy on test data. What is happening?

A) Underfitting — the model is too simple  
B) Overfitting — the model has memorized training data (correct)
C) The model is perfectly balanced  
D) The training set is too large  

---

### **Q8: Fixing Underfitting**
A model performs poorly on both training and test data (60% accuracy). What could improve performance?

A) Use more data  
B) Use a simpler model  
C) Use more complex features or a more complex model (correct)
D) Reduce training time  

---

### **Q9: Data Split Best Practice**
When training a machine learning model, what is the recommended split for training and test data?

A) 50% training, 50% testing  
B) 70-80% training, 10-15% validation, 10-15% testing (correct)
C) 90% training, 10% testing  
D) 99% training, 1% testing  

---

### **Q10: Evaluation Metrics - Precision vs. Recall**
In a medical diagnosis system, recall is more important than precision because:

A) We want to minimize false positives (healthy people flagged as sick)
B) We want to catch all sick patients, even if some healthy people are flagged  (correct)
C) Recall is always more important than precision  
D) Precision and recall are the same thing  

---

### **Q11: Evaluation Metric Scenario**
A cancer detection model flags 100 patients as having cancer. Of these, 95 are actually sick. What is the precision?

A) 95% (correct)
B) 90%  
C) 5%  
D) Cannot be calculated from this information  

---

### **Q12: F1-Score**
When should you use F1-Score instead of Accuracy?

A) When you have perfectly balanced classes  
B) When you have imbalanced classes or need balance between precision and recall (correct)
C) When predicting continuous values  
D) F1-Score should always be used over Accuracy  

---

### **Q13: ML in Business - Use Case**
Which of these is NOT a typical business use case for Machine Learning?

A) Personalized product recommendations  
B) Predicting customer churn  
C) Automating manual data entry  
D) Replacing all human decision-making in hiring (correct)

---

### **Q14: ML Challenges**
A model trained on images of cats in sunny outdoor settings performs poorly on cats indoors. What is the primary issue?

A) The model has too many parameters  
B) The training data doesn't represent the real-world variety the model will encounter (correct)
C) The model is overfitting  
D) Unsupervised learning was used instead of supervised  

---

### **Q15: Responsible AI - Bias**
A loan approval model trained on historical data (which favored male applicants) now approves loans at different rates by gender. What is this an example of?

A) High accuracy  
B) Model bias (reflecting biased historical patterns) (correct)
C) Underfitting  
D) Reinforcement Learning failure  

---

### **Q16: Neural Networks**
When is Deep Learning (neural networks) preferred over simpler algorithms?

A) Always — neural networks are always better  
B) For simple, structured data with clear relationships  
C) For complex, unstructured data like images, audio, and text (correct)
D) Never — neural networks are outdated  

---

### **Q17: Random Forest Algorithm**
What is an advantage of Random Forest over a single Decision Tree?

A) Faster training time  
B) Reduced overfitting and better generalization (correct)
C) Requires less data  
D) Simpler to interpret  

---

### **Q18: Real-World Scenario - E-commerce**
An online retailer wants to predict which products customers are likely to buy next. Should they use supervised or unsupervised learning?

A) Supervised Learning — they have past purchase history (labels)  (correct)
B) Unsupervised Learning — they want to discover patterns
C) Reinforcement Learning — the algorithm learns from customer interactions  
D) All three equally  

---

### **Q19: Confusion Matrix Understanding**
True Positive = Model predicted "yes" and was correct  
False Positive = Model predicted "yes" but was wrong  
False Negative = Model predicted "no" but was wrong  
True Negative = Model predicted "no" and was correct

A model predicts "spam" for 90 emails. 80 are actually spam, 10 are not. How many True Positives and False Positives?

A) TP=90, FP=0  
B) TP=80, FP=10 (correct)
C) TP=10, FP=80  
D) Cannot be determined  

---

### **Q20: Model Selection Scenario**
Your company has a small dataset (500 rows) and limited computing resources. Which would you avoid?

A) Logistic Regression
B) K-Means Clustering  
C) Deep Neural Networks  (correct)
D) Decision Trees  

---

### **Q21: Feature Engineering**
Why is feature engineering important in ML?

A) It guarantees perfect accuracy  
B) It reduces computational cost only  
C) The quality of features directly impacts model performance (correct)
D) It is only needed for Deep Learning  

---

### **Q22: Cross-Validation**
Why is cross-validation used in machine learning?

A) To make models faster  
B) To reduce overfitting and get a more reliable estimate of model performance (correct)
C) To reduce the need for labeled data  
D) It is not commonly used  

---

### **Q23: Class Imbalance Problem**
In a fraud detection dataset, 99% of transactions are legitimate and 1% are fraudulent. If your model predicts "legitimate" for all transactions, accuracy is 99%. Is this a good model?

A) Yes — 99% accuracy is excellent  
B) No — high accuracy can be misleading with imbalanced data; it's not catching fraud  (correct)
C) Yes if you use F1-Score instead
D) No — the dataset is too small  

---

### **Q24: Generalization**
A model that performs well on training data but poorly on new, unseen data has poor:

A) Efficiency
B) Generalization  (correct)
C) Feature selection  
D) Data quality  

---

### **Q25: ML Workflow Order**
What is the correct order in a typical ML workflow?

A) Train → Evaluate → Preprocess Data → Collect Data → Deploy  
B) Collect Data → Preprocess Data → Train → Evaluate → Deploy (correct)
C) Train → Collect Data → Preprocess → Evaluate → Deploy  
D) Evaluate → Train → Deploy → Collect Data  

---

---

## Answer Key & Explanations

| Q | Answer | Explanation |
|---|--------|-------------|
| 1 | C | Learning from images without explicit programming = ML. ML is a subset of AI. |
| 2 | B | Labeled data (spam/not spam) = Supervised Learning. |
| 3 | B | Finding hidden groups without predefined labels = Unsupervised Learning (Clustering). |
| 4 | B | Predicting continuous values (price) = Regression → Linear Regression. |
| 5 | B | Binary classification (approve/deny) = Logistic Regression. |
| 6 | B | Predicting a continuous value (stock price) = Regression. Others are classification. |
| 7 | B | High train accuracy, low test accuracy = Overfitting (memorized training data). |
| 8 | C | Poor on both = Too simple. Add features or complexity to improve. |
| 9 | B | Industry standard: ~70-80% train, 10-15% validation, 10-15% test. |
| 10 | B | In medical diagnosis, missing a sick patient (low recall) is worse than false alarms. |
| 11 | A | Precision = TP / (TP + FP) = 95 / (95 + 5) = 95%. |
| 12 | B | F1-Score balances precision & recall; essential for imbalanced datasets. |
| 13 | D | ML assists human decision-making, doesn't replace all human judgment responsibly. |
| 14 | B | Model trained on sunny outdoor cats fails indoors = poor training data representation. |
| 15 | B | Model reflects biased historical patterns = Algorithmic Bias. |
| 16 | C | Neural networks excel with complex, unstructured data (images, audio, text). |
| 17 | B | Random Forest = ensemble of trees → reduces overfitting, better generalization. |
| 18 | A | Past purchase history = labeled data → Supervised Learning for prediction. |
| 19 | B | 80 correctly predicted as spam = TP; 10 incorrectly predicted as spam = FP. |
| 20 | C | Deep Neural Networks need large datasets & significant compute. Best avoided here. |
| 21 | C | Good features = better models. Feature engineering is critical. |
| 22 | B | Cross-validation provides reliable performance estimates and reduces overfitting. |
| 23 | B | Class imbalance: high accuracy is misleading. Use Precision, Recall, F1-Score. |
| 24 | B | Poor on unseen data = poor Generalization. |
| 25 | B | Correct workflow: Collect → Preprocess → Train → Evaluate → Deploy. |

---

## Scoring Guide

| Score | Assessment |
|-------|------------|
| 23–25 (92–100%) | Excellent! Ready for Azure AI Services. |
| 20–22 (80–91%) | Strong foundation. Review weak questions before moving forward. |
| 17–19 (68–79%) | Good start. Review core concepts (Q1–10) before continuing. |
| 16 or below (< 64%) | Revisit 01-ai-concepts-ml.md, focus on Types of Learning & Evaluation Metrics. |

---

## What to Do After Quiz

**If you scored 80%+:** ✅ Move to Azure AI Services notes (02-azure-ai-services.md)

**If you scored below 80%:** Review these topics:
- Types of Learning (Supervised vs. Unsupervised)
- Overfitting vs. Underfitting
- Evaluation Metrics (Precision, Recall, F1-Score)
- Class Imbalance & why Accuracy alone is misleading

---

**Your Score: _____ / 25 (_____%)**

**Date Taken: April 17, 2026**

**Areas to Review:** [Write weak areas here after taking quiz]

