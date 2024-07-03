# Causal Feature Selection in Large Multivariate Time Series (MTS) for Forecasting Problems

## Project Overview

This project focuses on analyzing large multivariate time series (MTS) data for forecasting problems. The main objectives are to investigate various feature selection and prediction algorithms, evaluate their impact on forecasting performance, and explore the relationships between variables through experimental results.

## Objectives

- Determine the best combination of feature selection and prediction algorithms.
- Identify the most relevant variables and their causal relationships.
- Assess the influence of hyperparameters on algorithm performance.

## Datasets

- **VARsmall**: 10 features (6 relevant), VAR process, 3500 timestamps.
- **7ts2h**: 7 features (2 relevant), non-linear process, 3500 timestamps.

## Feature Selection Algorithms

### MRMR (Maximum Relevance Minimum Redundancy)

Selects features that maximize relevance to the target variable while minimizing redundancy among them.

### RReliefF

Evaluates features based on their ability to distinguish between different target values, adjusting weights to identify the most informative features.

## Prediction Algorithms

### Temporal Fusion Transformer (TFT)

Uses attention mechanisms to capture temporal relationships between variables, generating single-step predictions.

### DeepAR

Uses RNNs to model MTS data, generating probability distributions for future predictions.

## Experiments and Results

- **Feature Selection Impact**: Significant improvements in prediction accuracy with MRMR and RReliefF compared to no selection.
- **Hyperparameter Influence**: Highlighted the necessity of careful tuning for each target variable.
- **Stability Analysis**: Showed diverse stability profiles across different target variables, suggesting a need for individualized optimization.
- **Optimization Approaches**: Target-specific optimization significantly improved model performance.

## Conclusion

Feature selection and hyperparameter optimization play a critical role in forecasting multivariate time series data. MRMR and RReliefF effectively enhance prediction accuracy, while tailored hyperparameter tuning is essential for optimal performance.

## References

For further details on the algorithms and methodologies used, please refer to the project report included in this repository.

