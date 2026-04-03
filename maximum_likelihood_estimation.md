# Maximum Likelihood Estimation (MLE)

## 🔹 Definition

Maximum Likelihood Estimation (MLE) is a method to estimate model parameters by **maximizing the likelihood of observed data**.

> It selects parameter values that make the observed data most probable.

---

## 🔹 Problem Setup

Given:

* Data: x₁, x₂, ..., xₙ
* Model with parameters: θ

Goal:

θ* = argmax P(data | θ)

---

## 🔹 Likelihood Function

For independent observations:

L(θ) = Π P(xᵢ | θ)

* Measures how well parameters explain data
* Larger value → better fit

---

## 🔹 Log-Likelihood

log L(θ) = Σ log P(xᵢ | θ)

### Advantages:

* Converts multiplication → addition
* Easier to differentiate
* Same maximum

---

## 🔹 Example 1: Coin Toss

Data: H, H, T, H
Let θ = P(Head)

L(θ) = θ³ (1 − θ)

Result:

θ* = 0.75

---

## 🔹 Example 2: Gaussian Distribution

P(x | μ, σ) = (1 / √(2πσ²)) * e^(-(x − μ)² / (2σ²))

MLE estimates:

μ* = (1/n) Σ xᵢ

σ* = √[(1/n) Σ (xᵢ − μ)²]

---

## 🔹 Interpretation

* Data is fixed
* Parameters are variable
* Likelihood measures how well parameters explain data

> MLE finds the best-fitting model.

---

## 🔹 Probability vs Likelihood

| Concept     | Expression | Meaning |                               |
| ----------- | ---------- | ------- | ----------------------------- |
| Probability | P(x        | θ)      | Data varies, parameters fixed |
| Likelihood  | L(θ        | x)      | Data fixed, parameters vary   |

---

## 🔹 Key Insight

Maximize Likelihood ≡ Minimize Negative Log-Likelihood

This leads to:

* Mean Squared Error (MSE)
* Cross-Entropy Loss

---

## 🔹 Applications

* Linear Regression
* Logistic Regression
* Naive Bayes
* Neural Networks

---

## 🔹 Summary

> MLE finds parameter values that make observed data least surprising.

---
