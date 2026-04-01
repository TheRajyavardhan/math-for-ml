# Day 7: Naive Bayes Algorithm

## 📌 What is Naive Bayes?

Naive Bayes is a **probabilistic classification algorithm** based on Bayes’ Theorem.
It is used to predict the **most likely class** given some features.

---

## 📌 Core Formula

P(Class | Features) ∝ P(Class) × P(Features | Class)

---

## 📌 Key Idea

Naive Bayes assumes:

* All features are **independent** of each other
* This assumption is **not always true**, but simplifies computation

---

## 📌 Steps of Naive Bayes

### 1. Calculate Prior Probability

* P(Class)
* Example:

  * P(Spam) = 0.6
  * P(Not Spam) = 0.4

---

### 2. Calculate Likelihood

* P(Feature | Class)
* Example:

  * P(win | Spam)
  * P(money | Spam)

---

### 3. Compute Score

For each class:

Score = P(Class) × P(feature1 | Class) × P(feature2 | Class)

---

### 4. Compare Scores

* Higher score → Selected class

---

## 📌 Full Example

### Training Data

| Email | win | money | Class    |
| ----- | --- | ----- | -------- |
| 1     | Yes | Yes   | Spam     |
| 2     | Yes | No    | Spam     |
| 3     | No  | Yes   | Spam     |
| 4     | No  | No    | Not Spam |
| 5     | No  | Yes   | Not Spam |

---

### Prior

* P(Spam) = 3/5 = 0.6
* P(NotSpam) = 2/5 = 0.4

---

### Likelihood

* P(win | Spam) = 2/3

* P(money | Spam) = 2/3

* P(win | NotSpam) = 0/2 = 0

* P(money | NotSpam) = 1/2

---

### Prediction

For email: **"win money"**

Spam score:
0.6 × (2/3) × (2/3) ≈ 0.269

Not Spam score:
0.4 × 0 × 0.5 = 0

---

### Result

Final Classification → **Spam**

---

## 📌 Important Problem

### Zero Probability Problem

If any probability = 0:

→ Entire result becomes 0

---

## 📌 Solution

Use **Laplace Smoothing**:

(Add 1 to each count to avoid zero probability)

---

## 📌 Advantages

* Simple and fast
* Works well on small datasets
* Highly effective in text classification

---

## 📌 Disadvantages

* Assumes feature independence (not realistic)
* Zero probability issue without smoothing

---

## 📌 Applications

* Spam detection
* Sentiment analysis
* Document classification
* Medical diagnosis

---

## 📌 Summary

Naive Bayes works by:

* Calculating probabilities
* Multiplying them
* Choosing the highest result

👉 Simple, fast, and powerful algorithm for classification.
