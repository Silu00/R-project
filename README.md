# R-project
This project explores how to predict the **usable floor area (PUZ)** of buildings using regression and machine learning models. 
I wanted to compare different models (linear and ML-based) to find the most accurate way to predict PUZ using data like footprint, height, garage size, etc.

##Used methods:
- **Linear Regression**- baseline model (R² ≈ 0.70)
- **LASSO, Ridge, Elastic Net**- regularized regressions to avoid overfitting
- **XGBoost**- tree-based model, great at capturing nonlinearities
- **Neural Networks**- tested simple architectures for complex patterns

##Used data:
- 200 training + 20 validation samples
- Target: `puz` (usable floor area in m²)
- Features: `pz`, `wys`, `wys2`, `gar`, `gar2`, `kot`, `h_kol`, `kond`, `nach`

##Key summary: 
- **LASSO** gave the best prediction results (lowest RMSE)
- **XGBoost** also performed very well
- **Neural networks** showed potential but needed tuning

##Used tools:
- **R** with: `glmnet`, `xgboost`, `caret`, `ggplot2`
