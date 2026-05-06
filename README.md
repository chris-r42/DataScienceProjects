# DataScienceProjects

A growing portfolio of self-directed machine learning and data science projects. Each top-level folder is a self-contained project — some are finished, some are works in progress, and some are just getting started. Most are exploratory: I pick a dataset I find interesting, work through cleaning and EDA, and build a model from there.

**Stack:** Python, pandas, NumPy, scikit-learn, seaborn, matplotlib, plotly, Jupyter.

---

## Projects

### Mobile_Price — Mobile phone price classification
**Status:** Complete · **Accuracy:** 93%

Classifies phones into one of four price ranges from 20 hardware specs (RAM, battery, pixel dimensions, etc.). Built a logistic regression baseline with a `px_area = px_height * px_width` engineered feature, scaled inputs with `StandardScaler`, and validated with a held-out split before predicting on the Kaggle test set.

### spaceship-titanic — Kaggle Spaceship Titanic
**Status:** Working baseline · **Accuracy:** 76%

Binary classification of whether passengers were "transported." Split into a cleaning notebook and a model notebook. Engineered `GroupSize`, `IsAlone`, and `TotalSpent`, one-hot encoded `HomePlanet`/`Destination`, and trained a logistic regression. Next step: try tree-based models to push past the linear ceiling.

### LoL_data — League of Legends match outcome prediction
**Status:** In progress (long-running)

Working through a 51k-match dataset (Riot game data, 61 columns) with the eventual goal of predicting which team wins. Currently focused on EDA and feature engineering — built composite `t1_objectives` / `t2_objectives` columns, split first-blood into per-team flags, and explored the blue-side advantage in the data (blue wins ~58% when getting first blood vs. ~40% for red, which led to a deeper look at why). Modeling phase planned next. Long-term scope includes multiple sub-questions beyond just the winner.

### breast_cancer_classification
**Status:** Not started

Placeholder for a classification project on the sklearn breast cancer dataset. Will be picked up after F1data.

### F1data — Formula 1 race winner prediction (upcoming)
**Status:** Starting soon

Next active project. Plan is to use the `fastf1` library to pull race telemetry, qualifying results, and driver/constructor history, then build a model to predict race winners. Likely to start with classical ML (logistic regression / gradient boosting) before considering anything fancier.

---

## About me

Computer science student exploring ML/data science through hands-on projects. The goal of this repo is to keep a public record of what I've actually built and what I'm currently learning, rather than just course exercises.
