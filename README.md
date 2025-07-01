# skew-normal-stock-returns
This project demonstrates the application of skew-normal distributions in finance, specifically for modeling stock returns that exhibit asymmetry. The skew-normal distribution extends the normal distribution by adding a shape parameter α that controls skewness while maintaining normal-like tail behavior.

# Skew-Normal Stock Returns

Interactive educational tool for fitting normal and skew-normal distributions to stock returns data. This repository provides course materials and practical implementation for understanding the skew-normal distribution in financial modeling.

## 🎯 Key Features

- **Interactive Visualization**: Web-based application showing PDF curves for different shape parameters
- **Mathematical Implementation**: Complete formulation of skew-normal PDF and skewness calculations
- **Educational Content**: Course materials explaining the theoretical foundation
- **Practical Application**: Tools for fitting distributions to financial data

## 📈 The Skew-Normal Distribution

The skew-normal distribution is particularly useful for financial returns because:
- Addresses asymmetry in return distributions
- Maintains normal-like tail behavior (no excess kurtosis)
- Suitable when data has no more outliers than normal distribution
- **Limitation**: Cannot address heavy-tail problems (high kurtosis)

### Mathematical Formulation

**PDF Formula:**
```math
f(x) = \frac{2}{\sigma} \cdot \phi\left(\frac{x-\mu}{\sigma}\right) \cdot \Phi\left(\alpha\frac{x-\mu}{\sigma}\right)
**Parameters:**
- μ: location parameter
- σ: scale parameter  
- α: shape parameter (controls skewness)

**Skewness:**
\text{skewness} = \frac{(4-\pi) \cdot \left(\alpha\sqrt{\frac{\pi}{2}}\right)^2}{2\left(1-\frac{2\alpha^2}{\pi}\right)^{3/2}}
