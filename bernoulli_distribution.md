# 📊 Day X — Bernoulli Distribution

## 📌 Overview

Bernoulli Distribution is the **simplest probability distribution** used to model a **single experiment with only two possible outcomes**:

* Success (1)
* Failure (0)

👉 It is widely used in **binary classification problems** in machine learning.

---

## 📐 Formula

P(X = x) = p^x (1 - p)^(1 - x)

Where:

* x ∈ {0,1}
* p = Probability of success
* 1 - p = Probability of failure

---

## 🧠 Key Concepts

### 1. Binary Outcome

* Only two outcomes: **0 or 1**
* Examples:

  * Coin toss → Head (1), Tail (0)
  * Email → Spam (1), Not Spam (0)

---

### 2. Mean (Expected Value)

E(X) = p

👉 Average outcome equals probability of success

---

### 3. Variance

Var(X) = p(1 - p)

👉 Measures spread of outcomes

---

## 🧮 Example

Let:

* p = 0.7

Then:

* P(X = 1) = 0.7
* P(X = 0) = 0.3

Mean:
E(X) = 0.7

Variance:
Var(X) = 0.7 × 0.3 = 0.21

---

## ⚙️ Applications in Machine Learning

* Binary classification (Yes/No problems)
* Spam detection
* Medical diagnosis (disease / no disease)
* Bernoulli Naive Bayes

---

## 🔗 Relation to Other Concepts

* Based on Probability Basics
* Used in Naive Bayes Algorithm
* Extended to Binomial Distribution (multiple trials)

---

## ⚠️ Limitations

* Works only for:

  * Single trial
  * Binary outcomes

---

## 💡 Key Insight

Bernoulli Distribution is the **foundation of binary decision-making models** in statistics and machine learning.

---

## 🚀 Next Step

Learn **Binomial Distribution** (multiple Bernoulli trials)

