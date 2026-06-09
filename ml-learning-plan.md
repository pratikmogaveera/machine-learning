# ML Learning Plan

**Goal:** Learn ML to analyse mutual fund options & build FPL teams  
**Time commitment:** ~1 hour/day on weekdays, 2–3 hours on weekends  
**Prerequisites:** Basic stats (mean, probability, distributions) ✅

---

## Phase 0: Statistics Refresh (Week 1)

### Watch (StatQuest — "Statistics Fundamentals" playlist)

> Playlist: https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9

#### Watched ✅
- [x] 1. StatQuest: Histograms, Clearly Explained
- [x] 2. The Main Ideas behind Probability Distributions
- [x] 3. The Normal Distribution, Clearly Explained!!!
- [x] 4. The mean, the median, and the mode.
- [x] 5. The Exponential Distribution
- [x] 6. Population and Estimated Parameters, Clearly Explained!!!
- [x] 7. Calculating the Mean, Variance and Standard Deviation, Clearly Explained!!!
- [x] 8. What is a (mathematical) model?
- [x] 9. Hypothesis Testing and The Null Hypothesis, Clearly Explained!!!
- [x] 10. Alternative Hypotheses: Main Ideas!!!
- [x] 11. p-values: What they are and how to interpret them
- [x] 12. Fisher's Exact Test and the Hypergeometric Distribution
- [x] 13. How to calculate p-values
- [x] 14. p-hacking: What it is and how to avoid it!
- [x] 18. Covariance, Clearly Explained!!!
- [x] 19. Pearson's Correlation, Clearly Explained!!!

#### Currently watching 👈
- [ ] 15. False Discovery Rates, FDR, clearly explained

#### Must watch (core for ML foundations)
- [ ] 16. Statistical Power, Clearly Explained!!!
- [ ] 20. Conditional Probabilities, Clearly Explained!!!
- [ ] 21. Bayes' Theorem, Clearly Explained!!!!
- [ ] 24. The Binomial Distribution and Test, Clearly Explained!!!
- [ ] 25. The Central Limit Theorem, Clearly Explained!!!
- [ ] 28. Standard Deviation vs Standard Error, Clearly Explained!!!
- [ ] 30. Bootstrapping Main Ideas!!!
- [ ] 34. Logs (logarithms), Clearly Explained!!!
- [ ] 35. Confidence Intervals, Clearly Explained!!!
- [ ] 36. R-squared, Clearly Explained!!!
- [ ] 37. The Essence of Linear Regression
- [ ] 38. The Main Ideas of Fitting a Line to Data
- [ ] 40. Linear Regression, Clearly Explained!!!
- [ ] 42. Multiple Regression, Clearly Explained!!!
- [ ] 54. In Statistics, Probability is not Likelihood.
- [ ] 55. Maximum Likelihood, clearly explained!!!
- [ ] 59. Odds and Log(Odds), Clearly Explained!!!
- [ ] 62. Why Dividing By N Underestimates the Variance

#### Optional (nice to have, not blocking)
- [ ] 17. Power Analysis, Clearly Explained!!!
- [ ] 22. Expected Values, Main Ideas!!!
- [ ] 29. The standard error, Clearly Explained!!!
- [ ] 31. Using Bootstrapping to Calculate p-values!!!
- [ ] 39. Lowess and Loess, Clearly Explained!!!
- [ ] 51. Quantiles and Percentiles, Clearly Explained!!!
- [ ] 52. Quantile-Quantile Plots (QQ plots), Clearly Explained!!!
- [ ] 56. Maximum Likelihood for the Exponential Distribution
- [ ] 57. Maximum Likelihood for the Binomial Distribution
- [ ] 58. Maximum Likelihood For the Normal Distribution
- [ ] 60. Odds Ratios and Log(Odds Ratios), Clearly Explained!!!

#### Skip (not relevant to ML learning path)
Videos 4, 5, 23, 26, 27, 32, 33, 41, 43, 44, 45, 46, 47, 48, 49, 50, 53, 61

### Do
- [ ] Compute mean, std, correlation on any dataset using pandas/numpy
- [ ] Plot distributions with matplotlib/seaborn

---

## Phase 1: ML Foundations (Week 2–3)

### Watch (StatQuest)
- [ ] [A Gentle Introduction to Machine Learning](https://www.youtube.com/watch?v=Gv9_4yMHFhI)
- [ ] [Cross Validation](https://www.youtube.com/watch?v=fSytzGwwBVw)
- [ ] [The Bias-Variance Tradeoff](https://www.youtube.com/watch?v=EuBBz3bI-aA)
- [ ] [Gradient Descent](https://www.youtube.com/watch?v=sDv4f4s2SB8)
- [ ] [R-squared](https://www.youtube.com/watch?v=2AQKCEpau0s)
- [ ] [P-values](https://www.youtube.com/watch?v=vemZtEM63GY)

### Do
- [ ] Set up Python environment (Jupyter + pandas + numpy + matplotlib + scikit-learn)
- [ ] Practice: Load a CSV, explore data with pandas (.describe(), .corr(), .plot())
- [ ] Pull FPL API data and explore it in a notebook (`https://fantasy.premierleague.com/api/bootstrap-static/`)

---

## Phase 2: Linear & Logistic Regression (Week 3–4)

### Watch (StatQuest — "Linear Regression and Linear Models" playlist)
- [ ] Linear Regression (all parts)
- [ ] Multiple Regression
- [ ] Regularization (Ridge, Lasso, Elastic Net)

### Watch (StatQuest — "Logistic Regression" playlist)
- [ ] Logistic Regression (all parts)
- [ ] Confusion Matrix
- [ ] Sensitivity & Specificity
- [ ] ROC & AUC

### Do
- [ ] **Mini project:** Predict FPL player points using linear regression (features: form, minutes, fixture difficulty)
- [ ] Evaluate with R-squared, MAE
- [ ] **Mini project:** Classify players as "pick" vs "avoid" using logistic regression
- [ ] Evaluate with confusion matrix, AUC

---

## Phase 3: Tree-Based Models (Week 5–6)

### Watch (StatQuest)
- [ ] [Decision Trees](https://www.youtube.com/watch?v=_L39rN6gz7Y)
- [ ] [Random Forests](https://www.youtube.com/watch?v=J4Wdy0Wc_xQ)
- [ ] [AdaBoost](https://www.youtube.com/watch?v=LsK-xG1cLYA)
- [ ] [Gradient Boost](https://www.youtube.com/watch?v=3CC4N4z3GJc)
- [ ] [XGBoost](https://www.youtube.com/watch?v=OtD8wVaFm6E) (all parts)

### Do
- [ ] **FPL v2:** Rebuild points predictor with Random Forest & XGBoost
- [ ] Compare performance vs linear regression
- [ ] Use feature importance to understand what drives points
- [ ] Learn hyperparameter tuning (GridSearchCV)

---

## Phase 4: Hands-On Course (Week 7)

### Watch
- [ ] freeCodeCamp: "Machine Learning with Python and Scikit-Learn" (18hr course)
  - Watch sections on topics you've already learned as revision
  - Focus on new practical patterns (pipelines, preprocessing, feature engineering)

---

## Phase 5: Build the Projects (Week 8–10)

### Project A: FPL Team Optimizer
- [ ] Fetch current season data from FPL API
- [ ] Feature engineering: form, xG, xA, fixture difficulty, home/away, bonus
- [ ] Train XGBoost model to predict next GW points
- [ ] Use linear programming (PuLP) to select optimal squad under budget + position constraints
- [ ] Backtest: simulate past GWs, compare vs your actual team

### Project B: Mutual Fund Analyzer
- [ ] Collect NAV data from AMFI API (`https://www.amfiindia.com/spages/NAVAll.txt`)
- [ ] Calculate features: 1Y/3Y/5Y returns, Sharpe ratio, max drawdown, expense ratio, volatility
- [ ] Cluster funds by risk-return profile (K-Means)
- [ ] Rank funds within category using trained model
- [ ] Compare model picks vs category toppers on forward returns

---

## Key Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost pulp jupyter
```

---

## Resources

| Resource | Use For |
|----------|---------|
| [StatQuest YouTube](https://www.youtube.com/c/joshstarmer) | Conceptual understanding |
| [freeCodeCamp sklearn course](https://www.freecodecamp.org/news/machine-learning-with-python-and-scikit-learn/) | Practical implementation |
| [Krish Naik - ML in 6 hours](https://www.youtube.com/c/KrishNaik) | Quick revision |
| [scikit-learn docs](https://scikit-learn.org/stable/) | Reference |
| [Kaggle](https://www.kaggle.com/) | Datasets + notebooks to learn from |

---

## Rules for Myself
1. Understand the "why" before coding the "how"
2. One concept at a time — don't binge without practicing
3. Every algorithm learned = applied to FPL or MF data that same week
4. Track experiments in notebooks, compare model versions
5. Don't touch deep learning until Phase 5 projects are working well
