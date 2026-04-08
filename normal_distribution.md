# 📊 Day X — Normal Distribution (Gaussian Distribution)

## 📌 Overview

Normal Distribution is a **probability distribution** that describes how data is spread around the mean.

👉 It forms a **bell-shaped curve**  
👉 Widely used in statistics and machine learning  

---

## 📐 Formula

f(x) = (1 / (σ √(2π))) * e^(-(x - μ)² / (2σ²))

Where:
- μ = Mean (center of distribution)
- σ = Standard Deviation (spread)

---

## 🧠 Key Properties

### 1. Symmetry
- Distribution is perfectly symmetric around the mean  
- Left side = Right side  

---

### 2. Mean = Median = Mode
- All three are equal in a perfect normal distribution  

---

### 3. Empirical Rule (68–95–99.7 Rule)

| Range | Percentage of Data |
|------|------------------|
| μ ± 1σ | 68% |
| μ ± 2σ | 95% |
| μ ± 3σ | 99.7% |

👉 Most data lies close to the mean  

---

## 🔄 Standard Normal Distribution

When data is standardized:

z = (x - μ) / σ

- Mean becomes **0**
- Standard deviation becomes **1**

👉 This is called **Z-score normalization**

---

## 🎯 Why It Matters in Machine Learning

- Many models assume normal distribution  
- Used in:
  - Gaussian Naive Bayes  
  - Statistical analysis  
  - Error modeling  

---

## ⚠️ Limitations

- Not all data follows normal distribution  
- Real-world data can be:
  - Skewed  
  - Heavy-tailed  
  - Multi-modal  

---

## 💡 Intuition

> Normal Distribution tells:
> - Where most values lie  
> - How rare or extreme a value is  

---

## 🚀 Key Takeaway

- Mean → center  
- Standard deviation → spread  
- Most data lies near the mean  

👉 Understanding this is **critical for probability, statistics, and ML**

---
