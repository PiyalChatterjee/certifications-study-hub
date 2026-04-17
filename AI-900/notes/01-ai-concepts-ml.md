# 01: AI Concepts & Machine Learning Fundamentals

## What is AI?

### Definition
**Artificial Intelligence** is the simulation of human intelligence processes by machines, especially computer systems.

### AI vs. Machine Learning (ML)
- **AI** = Broad field of creating intelligent machines (includes everything)
- **ML** = Subset of AI focused on learning from data without explicit programming
- **Deep Learning** = Subset of ML using neural networks

```
┌─────────────────┐
│       AI        │
│  ┌───────────┐  │
│  │     ML    │  │
│  │ ┌─────────┤  │
│  │ │ DL      │  │
│  │ └─────────┤  │
│  └───────────┘  │
└─────────────────┘
```

---

## Machine Learning Concepts

### Types of ML

#### 1. **Supervised Learning**
- Model learns from labeled data (input-output pairs)
- **Use cases:** Prediction, classification
- **Examples:**
  - Email spam detection
  - House price prediction
  - Image classification

#### 2. **Unsupervised Learning**
- Model learns from unlabeled data to find patterns
- **Use cases:** Clustering, pattern discovery
- **Examples:**
  - Customer segmentation
  - Anomaly detection
  - Data clustering

#### 3. **Reinforcement Learning**
- Model learns by trial and error with rewards/penalties
- **Use cases:** Game playing, autonomous systems
- **Examples:**
  - Game AI (chess, Go)
  - Robotics navigation
  - Recommendation systems

---

### Common ML Algorithms

| Algorithm | Type | Use Case |
|-----------|------|----------|
| Linear Regression | Supervised | Predict continuous values |
| Logistic Regression | Supervised | Binary/multi-class classification |
| Decision Trees | Supervised | Classification & regression |
| Random Forest | Supervised | Ensemble method for accuracy |
| K-Means | Unsupervised | Clustering data |
| Neural Networks | Supervised/Unsupervised | Complex pattern recognition |
| Support Vector Machines (SVM) | Supervised | Classification |

---

## Key ML Concepts for AI-900

### Training vs. Testing
- **Training set:** Used to teach the model (70-80% of data)
- **Validation set:** Used to tune the model (10-15% of data)
- **Test set:** Used to evaluate final performance (10-15% of data)

### Overfitting & Underfitting

| Overfitting | Underfitting | Optimal |
|-------------|--------------|---------|
| Model memorizes training data | Model is too simple | Balanced fit |
| High training accuracy, low test accuracy | Low accuracy on both | Good train & test accuracy |
| **Solution:** More data, regularization, simpler model | **Solution:** More features, complex model | ✅ |

### Model Evaluation Metrics

#### Classification Metrics
- **Accuracy:** Correct predictions / Total predictions
- **Precision:** True positives / (True positives + False positives)
  - "Of all predictions we made as positive, how many were correct?"
- **Recall:** True positives / (True positives + False negatives)
  - "Of all actual positives, how many did we catch?"
- **F1-Score:** Harmonic mean of precision & recall (balanced metric)

#### Regression Metrics
- **Mean Squared Error (MSE):** Average squared difference from actual values
- **Root Mean Squared Error (RMSE):** Square root of MSE
- **Mean Absolute Error (MAE):** Average absolute difference

---

## AI & ML in Business Context

### Why Companies Use AI/ML
✅ Automation of repetitive tasks  
✅ Better predictions & decision-making  
✅ Cost reduction  
✅ Personalization & customer insights  
✅ Identifying patterns at scale  

### Challenges
❌ Data quality & quantity  
❌ Model bias & fairness  
❌ Interpretability ("black box" problem)  
❌ Computational resources  
❌ Ethical concerns  

---

## Exam Tips for This Topic

1. **Understand the difference** between supervised/unsupervised/reinforcement learning
2. **Know when to use which algorithm** (classification vs regression vs clustering)
3. **Recognize overfitting scenarios** and solutions
4. **Understand evaluation metrics** — especially precision vs recall
5. **Real-world context:** Given a business problem, identify the right ML approach
6. **Responsible AI concepts:** Be aware of bias, fairness, and ethical considerations

---

## Quick Reference

**When to use Supervised Learning?**
→ You have labeled data and want to predict/classify

**When to use Unsupervised Learning?**
→ You want to discover patterns or group similar items

**When to use Reinforcement Learning?**
→ You have an agent learning through interaction (rare in AI-900)

**Accuracy isn't enough because...**
→ In imbalanced datasets, high accuracy can be misleading. Use precision/recall/F1-score instead.
