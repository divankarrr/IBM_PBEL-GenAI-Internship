# Day 07 Notes

## 1. Artificial Intelligence

Artificial Intelligence (AI) enables machines to perform tasks that normally require human intelligence.

Examples:

- Chatbots
- Self-driving cars
- Recommendation systems

---

## 2. Machine Learning

Machine Learning is a subset of AI where machines learn patterns from data without being explicitly programmed.

Workflow:

Data

↓

Training

↓

Model

↓

Prediction

---

## 3. Types of Machine Learning

### Supervised Learning

Uses labeled data.

Examples:

- Linear Regression
- Logistic Regression
- Decision Tree
- Random Forest
- SVM

Applications:

- House Price Prediction
- Spam Detection
- Disease Prediction

---

### Unsupervised Learning

Uses unlabeled data.

Examples:

- K-Means Clustering
- Hierarchical Clustering
- PCA

Applications:

- Customer Segmentation
- Market Basket Analysis
- Anomaly Detection

---

## 4. Linear Regression

Used to predict continuous values.

Equation:

y = mx + c

Where:

- y = Prediction
- m = Slope
- c = Intercept

Goal:

Find the best-fit line that minimizes prediction error.

---

## 5. Cost Function

Measures how wrong the model predictions are.

Common Cost Function:

Mean Squared Error (MSE)

Lower Cost = Better Model

---

## 6. Gradient Descent

Optimization algorithm used to minimize the cost function.

Types:

### Batch Gradient Descent

Uses the entire dataset.

Advantages:

- Stable

Disadvantages:

- Slow for large datasets

---

### Stochastic Gradient Descent (SGD)

Uses one training example at a time.

Advantages:

- Faster

Disadvantages:

- More fluctuations

---

### Mini-Batch Gradient Descent

Uses small batches of data.

Most commonly used in Deep Learning.

---

## 7. Evaluation Metrics

### MAE

Average absolute prediction error.

### MSE

Average squared error.

### RMSE

Square root of MSE.

### R² Score

Measures how well the regression model explains the data.

Range:

0 to 1

Higher is better.

---

## 8. Model Performance

### Underfitting

Model is too simple.

High Bias

Low Variance

---

### Overfitting

Model memorizes training data.

Low Bias

High Variance

Poor performance on unseen data.

---

## 9. Bias-Variance Tradeoff

Good models balance:

- Low Bias
- Low Variance

---

## 10. Regularization

Used to reduce overfitting.

### L1 Regularization (Lasso)

- Removes less important features.
- Produces sparse models.

---

### L2 Regularization (Ridge)

- Reduces weight values.
- Keeps all features.

---

## 11. Machine Learning vs Deep Learning

| Machine Learning | Deep Learning |
|------------------|---------------|
| Manual feature engineering | Automatic feature learning |
| Works well on smaller datasets | Requires large datasets |
| Faster training | Computationally intensive |
| Simpler models | Neural Networks |

---

## 12. Key Takeaways

✔ Machine Learning is the foundation of Deep Learning.

✔ Gradient Descent is the most important optimization algorithm.

✔ Overfitting can be controlled using Regularization.

✔ Model evaluation metrics help compare regression models.

✔ Understanding ML concepts is essential before learning Neural Networks.
