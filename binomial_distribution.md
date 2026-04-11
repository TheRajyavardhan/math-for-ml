# 📊 Day X — Binomial Distribution

## 📌 Overview

Binomial Distribution models the number of **successes** in a fixed number of **independent trials**, where each trial has only two possible outcomes:

- Success (1)  
- Failure (0)  

👉 It is an extension of the Bernoulli Distribution (single trial → multiple trials)

---

## 📐 Formula

P(X = k) = (nCk) * p^k * (1 - p)^(n - k)

Where:

- n = Number of trials  
- k = Number of successes  
- p = Probability of success  
- (1 − p) = Probability of failure  
- nCk = Number of combinations  

---

## 🧠 Key Concepts

### 1. Multiple Trials
- Same experiment repeated n times  
- Each trial is independent  

### 2. Binary Outcome
- Only two outcomes:
  - Success
  - Failure  

### 3. Fixed Probability
- Probability of success (p) remains constant  

---

## 🧮 Example

### Problem:
Toss a fair coin 5 times.  
Find probability of getting exactly 3 heads.

### Solution:

- n = 5  
- k = 3  
- p = 0.5  

P(X = 3) = 5C3 * (0.5)^3 * (0.5)^2  
= 10 * (0.5)^5  
= 10 / 32  
= 0.3125  

---

## 📊 Mean and Variance

- Mean (Expected Value):  
  E(X) = n * p  

- Variance:  
  Var(X) = n * p * (1 - p)  

---

## ⚙️ Conditions for Binomial Distribution

1. Number of trials is fixed (n)  
2. Trials are independent  
3. Only two outcomes exist  
4. Probability remains constant  

---

## 🎯 Real-Life Examples

- Number of students passing an exam  
- Number of defective products in a batch  
- Number of successful sales calls  
- Number of heads in multiple coin tosses  

---

## 🔗 Relation to Other Concepts

- Bernoulli Distribution → Single trial  
- Binomial Distribution → Multiple trials  

👉 Binomial = sum of independent Bernoulli trials  

---

## ⚠️ Limitations

Not applicable if:
- Probability changes  
- Trials are dependent  

---

## ⚙️ Applications in Machine Learning

- Binary classification  
- A/B testing  
- Spam detection  
- Success/failure modeling  

---

## 💡 Key Insight

Binomial Distribution answers:  
"How many successes will occur in multiple trials?"

---

## 🚀 Next Step

👉 Poisson Distribution
