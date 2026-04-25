## Alpha Signal Stack with Volatility Forecasting
## Author

Carlos Arturo Rubiano Passos  
Quantitative Economist | Econometrics, Machine Learning & Macro-Financial Modeling  
GitHub: https://github.com/carlosrubiano2026  
LinkedIn: https://www.linkedin.com/in/TU-LINK
## Key Features

- Alpha stacking with multiple expert models
- Walk-forward validation framework
- Meta-label gating based on confidence thresholds
- Volatility forecasting and risk scaling
- Deployment-style signal construction
This project develops a stacked machine learning framework for crypto market signal generation using 4-hour market data.

The system combines alpha prediction, walk-forward validation, meta-label gating, volatility forecasting, and risk-scaled position sizing into a deployment-style signal artifact.

## Objective

To build a research-grade predictive pipeline for crypto trading signals, focusing on:

- Directional alpha prediction
- Out-of-fold stacking
- Walk-forward validation
- Meta-label gate modeling
- Volatility forecasting
- Risk-adjusted signal integration

## Methodology

The notebook is organized into sequential modeling blocks:

1. Load and validate a stack-ready research dataset
2. Build task-specific modeling samples for alpha, gate, volatility, and tail-risk layers
3. Construct chronological walk-forward folds
4. Define an alpha expert library using multiple feature families and model classes
5. Train base alpha experts and generate out-of-fold predictions
6. Train an alpha meta-model using stacked expert predictions
7. Build a meta-label gate based on alpha confidence and cost-adjusted hurdles
8. Train and evaluate the gate model against a naive confidence baseline
9. Build a volatility forecasting sample with HAR-style persistence features
10. Train volatility models and compare them using QLIKE, RMSE, and MAE
11. Integrate alpha, confidence, volatility forecasts, and risk scaling into a final signal artifact

## Models

The project uses:

- Logistic Regression
- Random Forest
- Extra Trees
- HistGradientBoosting
- Stacked meta-models
- HAR-style volatility benchmarks
- Walk-forward out-of-fold validation

## Key Technical Features

- Strict chronological validation
- Out-of-fold prediction architecture
- Alpha stacking
- Meta-labeling logic
- Volatility modeling on log-volatility targets
- QLIKE-aware volatility evaluation
- Risk-scaled desired position construction
- Deployment-style signal output

## Tools

- Python
- pandas
- NumPy
- scikit-learn
- statsmodels-style time-series logic
- Matplotlib

## Repository Structure

```text
crypto-alpha-stacking-volatility-forecasting/
├── notebooks/
│   └── crypto_alpha_stack_v2.ipynb
├── README.md
└── requirements.txt
