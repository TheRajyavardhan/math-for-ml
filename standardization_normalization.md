# 📊 Data Scaling in Machine Learning: Normalization vs Standardization

## 📌 Overview

In machine learning, features often have different scales.  
For example:
- Age → 0 to 100
- Salary → 10,000 to 1,000,000

This creates imbalance.

👉 **Solution:** Scale the data

---

# 🟢 1. Normalization (Min-Max Scaling)

## 📐 Formula

x' = (x - min) / (max - min)

## 📘 Explanation

- Transforms values into range **[0, 1]**
- Maintains relative distances between values

## 🧮 Example

Dataset: [10, 20, 30, 40, 50]

- min = 10  
- max = 50  

For x = 30:

x' = (30 - 10) / (50 - 10) = 20/40 = 0.5

## ⚠️ Limitation

- Highly sensitive to **outliers**

Example:
[10, 20, 30, 40, 1000]

→ Most values collapse near 0

---

# 🔵 2. Standardization (Z-Score Scaling)

## 📐 Formula

z = (x - μ) / σ

Where:
- μ = mean
- σ = standard deviation

## 📘 Explanation

- Mean becomes **0**
- Standard deviation becomes **1**
- Values represent **distance from mean**

## 🧮 Example

Dataset: [10, 20, 30, 40, 50]

- Mean (μ) = 30  
- Std Dev (σ) ≈ 14.14  

For x = 50:

z = (50 - 30) / 14.14 ≈ 1.41

👉 Interpretation:
- Value is **1.41 standard deviations above mean**

---

# 🧠 Interpretation of Z-Score

| Z-Score | Meaning |
|--------|--------|
| 0 | Exactly average |
| +0.5 | Slightly above average |
| +1 | Above average |
| +2 | Very high (rare) |
| -1 | Below average |

---

# ⚔️ Normalization vs Standardization

| Feature | Normalization | Standardization |
|--------|-------------|----------------|
| Range | 0 to 1 | No fixed range |
| Uses Mean/Std | ❌ | ✅ |
| Outliers | Sensitive | More robust |
| Interpretation | Relative position | Distance from mean |

---

# 🧠 When to Use What

## Use Normalization when:
- Data needs bounded range
- Neural Networks
- Image processing

## Use Standardization when:
- Most ML models
- Data has outliers
- Statistical interpretation needed

---

# 🔥 Key Insight

- **Normalization** → "Where does this value lie between min and max?"
- **Standardization** → "How far is this value from the average?"

---

# 🚀 Conclusion

> Good models require well-scaled data.

- Normalization is simple but sensitive  
- Standardization is more robust and widely used  

👉 In practice:
**Standardization is the default choice in machine learning**

---
