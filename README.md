# Regression Learners: Decision Trees, Random Trees, and Ensemble Methods

## Project Overview  
This project involved building and evaluating multiple supervised learning models using Classification and Regression Tree (CART) principles. Implemented in pure Python with NumPy, the models include a standard Decision Tree (DTLearner), a Random Tree (RTLearner), a Bagged Ensemble (BagLearner), and a stacked ensemble referred to as InsaneLearner. The goal was to predict continuous values using multivariate data, with a focus on model design, data preprocessing, performance evaluation, and modular, testable code.

**Languages/Tools Used:** Python, NumPy, Matplotlib  
**Key Concepts:** Supervised Machine Learning, Decision Trees, Ensemble Learning, Bootstrap Aggregation (Bagging), Regression, Model Evaluation

---

## Project Objectives
- Build object-oriented implementations of four regression learners from scratch:
  - `DTLearner` (classic decision tree)
  - `RTLearner` (randomized decision tree)
  - `BagLearner` (ensemble of trees using bootstrap aggregation)
  - `InsaneLearner` (stacked ensemble of bagged learners)
- Predict target values (e.g., market index returns) from multivariate input features
- Handle data cleansing, splitting, and evaluation internally
- Visualize performance comparisons through properly labeled charts
- Adhere to strict performance, formatting, and structural constraints

---

## Technical Highlights
- Learners implemented using recursive tree construction stored in NumPy arrays (no node-based trees)
- Feature selection in `DTLearner` based on highest absolute correlation with target variable
- `RTLearner` selects features randomly, simulating randomness in decision-making
- `BagLearner` creates multiple bootstrap samples and aggregates predictions from base learners
- `InsaneLearner` composes 20 `BagLearners`, each with 20 learners—demonstrating stacked ensembles
- Training/testing datasets are randomly split (60/40) with reproducibility preserved
- All output (charts, stats) produced through `testlearner.py`, ensuring separation of concerns

---

## Value & Learning Outcomes
- Developed core understanding of tree-based regression models and ensemble learning  
- Built scalable, reusable learner classes with well-defined APIs  
- Learned to evaluate model accuracy using metrics like correlation between actual and predicted values  
- Improved performance-conscious programming by meeting runtime constraints  
- Practiced clean experiment logging, charting, and result reporting in a centralized script  

---

## Sample Experiment  
**Dataset:** Istanbul.csv  
**Objective:** Predict MSCI Emerging Markets (EM) index using other index returns  
**Evaluation Metric:** Correlation between predicted and actual EM returns  
**Experiment Performed In:** `testlearner.py` using randomized 60/40 train/test split  

---

## Repository Access  
Due to academic policy, the full implementation—including code, generated results, and experiment scripts—is stored in a private GitHub repository. **Access available upon request.**
