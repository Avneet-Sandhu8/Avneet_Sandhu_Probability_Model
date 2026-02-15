# Avneet_Sandhu_Probability_Model
# Assignment 1 – Probability Density Function
**Roll Number:** 102303289

## Overview
Analysis of NO2 column from India Air Quality dataset with custom probability density function estimation.

## Parameters Calculation
Based on roll number 102303289:
- `r mod 7 = 3` → `a = 0.05 × 3 = 0.15`
- `r mod 5 = 4` → `b = 0.3 × (4 + 1) = 1.5`

## Transformation Applied
```
z = x + 0.15 × sin(1.5x)
```

## Estimated PDF Parameters
- **μ (mean):** 25.814687
- **λ (lambda):** 0.00146123
- **c (constant):** 0.02156673

Where:
- σ² = variance(z)
- λ = 1 / (2σ²)
- c = 1 / √(2πσ²)

## Dataset
India Air Quality Dataset - NO2 column
