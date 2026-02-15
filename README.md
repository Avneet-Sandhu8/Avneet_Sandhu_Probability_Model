# Avneet_Sandhu_Probability_Model

## Assignment 1 – Probability Density Function
**Roll Number:** 102303289  
**Student Name:** Avneet Sandhu

---


## Overview
This assignment analyzes the **NO2 column** from the **India Air Quality dataset** and estimates parameters for a custom probability density function (PDF) based on roll number 102303289.

---

## Methodology

### Step 1: Parameter Calculation
The parameters `a` and `b` are calculated using the roll number:
- **a = 0.05 × (r mod 7)**
- **b = 0.3 × (r mod 5 + 1)**

### Step 2: Data Transformation
Apply the transformation formula to the NO2 data:
```
z = x + a × sin(b × x)
```

### Step 3: PDF Parameter Estimation
Calculate the following parameters:
- **μ (mean)** = mean(z)
- **σ² (variance)** = variance(z)
- **λ (lambda)** = 1 / (2σ²)
- **c (constant)** = 1 / √(2πσ²)

---

## Parameters Calculation

Based on roll number **102303289**:

### Calculations:
- `r mod 7 = 3` → **a = 0.05 × 3 = 0.15**
- `r mod 5 = 4` → **b = 0.3 × (4 + 1) = 1.5**

---

## Transformation Applied

```python
z = x + 0.15 × sin(1.5x)
```

Where:
- `x` = Original NO2 values
- `z` = Transformed values
- `a` = 0.15
- `b` = 1.5

---

## Estimated PDF Parameters

| Parameter | Formula | Value |
|-----------|---------|-------|
| **μ (mean)** | mean(z) | **25.814687** |
| **σ² (variance)** | variance(z) | *342.013* |
| **λ (lambda)** | 1 / (2σ²) | **0.00146123** |
| **c (constant)** | 1 / √(2πσ²) | **0.02156673** |

### Formula Definitions:
- σ² = variance(z)
- λ = 1 / (2σ²)
- c = 1 / √(2πσ²)

---

## Results

### Result Table

| Metric | Value |
|--------|-------|
| Roll Number | 102303289 |
| Parameter a | 0.15 |
| Parameter b | 1.5 |
| Mean (μ) | 25.814687 |
| Lambda (λ) | 0.00146123 |
| Constant (c) | 0.02156673 |

### Interpretation
The estimated probability density function follows a Gaussian-like distribution centered around **μ = 25.81** with decay rate controlled by **λ = 0.00146**.

---

## Dataset

**Source:** India Air Quality Dataset  
**Column Used:** NO2 (Nitrogen Dioxide)  
**Data Processing:**
- Removed NaN values
- Applied transformation
- Computed statistical parameters

---

