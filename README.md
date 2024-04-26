DESCRIPTION OF THE PROJECT
Background
These data were aggregated from a number of sources including the American Community Survey (census.gov), clinicaltrials.gov, and cancer.gov.

Goal
The goal is to build a predictive model to predict "TARGET_deathRate".

Data Dictionary
TARGET_deathRate: Dependent variable. Mean per capita (100,000) cancer mortalities(a)

avgAnnCount: Mean number of reported cases of cancer diagnosed annually(a)

avgDeathsPerYear: Mean number of reported mortalities due to cancer(a)

incidenceRate: Mean per capita (100,000) cancer diagnoses(a)

medianIncome: Median income per county (b)

popEst2015: Population of county (b)

povertyPercent: Percent of populace in poverty (b)

studyPerCap: Per capita number of cancer-related clinical trials per county (a)

binnedInc: Median income per capita binned by decile (b)

MedianAge: Median age of county residents (b)

MedianAgeMale: Median age of male county residents (b)

MedianAgeFemale: Median age of female county residents (b)

Geography: County name (b)

AvgHouseholdSize: Mean household size of county (b)

PercentMarried: Percent of county residents who are married (b)

PctNoHS18_24: Percent of county residents ages 18-24 highest education attained: less than high school (b)

PctHS18_24: Percent of county residents ages 18-24 highest education attained: high school diploma (b)

PctSomeCol18_24: Percent of county residents ages 18-24 highest education attained: some college (b)

PctBachDeg18_24: Percent of county residents ages 18-24 highest education attained: bachelor's degree (b)

PctHS25_Over: Percent of county residents ages 25 and over highest education attained: high school diploma (b)

PctBachDeg25_Over: Percent of county residents ages 25 and over highest education attained: bachelor's degree (b)

PctEmployed16_Over: Percent of county residents ages 16 and over employed (b)

PctUnemployed16_Over: Percent of county residents ages 16 and over unemployed (b)

PctPrivateCoverage: Percent of county residents with private health coverage (b)

PctPrivateCoverageAlone: Percent of county residents with private health coverage alone (no public assistance) (b)

PctEmpPrivCoverage: Percent of county residents with employee-provided private health coverage (b)

PctPublicCoverage: Percent of county residents with government-provided health coverage (b)

PctPubliceCoverageAlone: Percent of county residents with government-provided health coverage alone (b)

PctWhite: Percent of county residents who identify as White (b)

PctBlack: Percent of county residents who identify as Black (b)

PctAsian: Percent of county residents who identify as Asian (b)

PctOtherRace: Percent of county residents who identify in a category which is not White, Black, or Asian (b)

PctMarriedHouseholds: Percent of married households (b)

BirthRate: Number of live births relative to number of women in county (b)

(a): years 2010-2016 (b): 2013 Census Estimates

Hyperlink to dataset: https://data.world/nrippner/ols-regression-challenge

Jupyter Notebooks
Inspect the Jupyter Notebooks in order:

In "2.1) Preprocessing_and_EDA_Part_1", we thoroughly examine and preprocess the dataset. Tasks include transforming categorical variables, addressing missing data, and handling outliers and high-leverage points. We also analyze variable distributions.

Moving to "2.2) Preprocessing_and_EDA_Part_2, we deepen our exploration. We use scatterplots, boxplots, and correlation matrices to visualize relationships and identify patterns. We apply dimensionality reduction and split the dataset for model evaluation.

Transitioning to "3.1) Linear_Regression_Models_Part1", we initially focus on dimensionality reduction techniques. We reduce dataset complexity while retaining essential information using Principal Components Regression (PCR) and explore a polynomial version.

In "3.2) Linear_Regression_Models_Part2", we delve into the variable selection methods Forward Selection, Backwards Elimination and Stepwise Selection.

In "3.3) Linear_Regression_Models_Part3", we implement variable selection via the regularization methods Ridge and Lasso Regression.

Moving on to "4) KNN-Decision Tree", we evaluate KNN and Decision Tree algorithms' performance.

In "5.1) Sklearn_Ensemble_Methods_Part1" and "5.2) Sklearn_Ensemble_Methods_Part2", we employ Scikit Learn's ensemble methods including Bagging, Random Forest, AdaBoost and Gradient Boosting Regression.

In "6.1) XGBoost", "6.2) CatBoost" and "6.3) LightGBM", we implement the optimized boosting algorithms XGBoost, CatBoost and LightGBM.

In "7) SVR", we conduct Support Vector Regression.

Lastly, in "8) Results_and_Conclusions", we compare model performance metrics and identify the most accurate prediction method.

Note 1: Scaling
Certain methods necessitated scaling of predictor variables, while others were indifferent to scaling. Nevertheless, we tested each model with and without scaling, and retained the version that yielded the best performance.

Note 2: Optimization of models
For every model optimized through the GridSearchCV method, we determined the values of hyperparameters to be examined by referring to literature, articles, and also sought assistance from ChatGPT.

Note 3: Updates
In the future, we may consider incorporating additional methods.
