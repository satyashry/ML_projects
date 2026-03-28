## Day 1 — Linear Regression

### Dataset
- **California Housing** (built into sklearn)
- 20,640 houses, 8 features
- Task: predict house prices


### Model
- Linear Regression (sklearn)

### Metrics
| Metric | California Housing |
|--------|-------------------|
| MAE    | 0.53              | 
| MSE    | 0.56              | 
| R²     | 0.57              | 

### What I Learned
- Linear regression finds best line y = mx + b through data
- m (coef_) = slope — how much y changes per feature
- b (intercept_) = base value when all features = 0
- MAE = average error in real units
- MSE = squares errors — punishes large mistakes heavily
- R² = how much better model is vs lazy baseline (always predicting mean)
- How gradient descent finds best m and b
- Feature scaling with StandardScaler