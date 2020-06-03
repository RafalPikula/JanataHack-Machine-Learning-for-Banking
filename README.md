# JanataHack-Machine-Learning-for-Banking

We present a summary of the outcome of taking part in a hackathon organized by Analytics Vidhya (under the name JanataHack: Machine Learning for Banking) in which the participants, given loan applicants data, were to determine the loan rate category (out of 3 different categories). On the officially binding private leaderboard our best model secured the position in the top **4.7%** of the participants.

Here is the link to the competition website: https://datahack.analyticsvidhya.com/contest/janatahack-machine-learning-for-banking/#ProblemStatement

## Approach Summary

We split our work into two Jupyter notebooks. The first notebook is devoted to the exploratory data analysis of both original and engineered features. The second one contains the actual data preparation and model training. 

In the first notebook we look at the data and note that we are given 14 columns and 164309 observations to work with. We determine the columns with missing data, compute simple statistics of both categorical and numeric variables, and visualize the distribution of our variables (as well as certain conditional distributions). We also spend some time deriving new features (by both analyzing the available data and, whenever applicable, utilizing a semi-automated feature engineering procedure) and visualizing them.

In the second notebook we first prepare our data and apply feature engineering to enlarge the pool of available features and then we construct a preprocessing pipeline (mainly to impute missing data) together with a modeling pipeline and apply the procedure of 5-fold cross-validation for hyperparameter tuning, model training and selection. During the model training phase we tried several sets of features, as well as various machine learning algorithms, including Random Forest, Forest of Randomized Trees, CatBoost and LightGBM. The best performing model turned out to be the LigthGBM classifier. Moreover, predominantly thanks to the features added during the feature engineering phase, this model placed highly among its competitors.



