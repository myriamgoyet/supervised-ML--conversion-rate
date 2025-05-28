Project completed as part of my Data Science training with Jedha Bootcamp (Paris)

# Challenge : predict conversions 🏆🏆
In this project, I participated to a machine learning competition like the ones that are organized by https://www.kaggle.com/. I worked with jupyter notebooks as usual, but in the end I have to submited my model's predictions to our teacher/TA, so its performances could be evaluated in an independent way. The scores achieved by the different teams were stored into a leaderboard 🏅🏅

## Company's Description 📇
www.datascienceweekly.org is a famous newsletter curated by independent data scientists. Anyone can register his/her e-mail address on this website to receive weekly news about data science and its applications !

## Project 🚧
The data scientists who created the newsletter would like to understand better the behaviour of the users visiting their website. They would like to know if it's possible to build a model that predicts if a given user will subscribe to the newsletter, by using just a few information about the user. They would like to analyze the parameters of the model to highlight features that are important to explain the behaviour of the users, and maybe discover a new lever for action to improve the newsletter's conversion rate.

They designed a competition aiming at building a model that allows to predict the *conversions* (i.e. when a user will subscribe to the newsletter). To do so, they open-sourced a dataset containing some data about the traffic on their website. To assess the rankings of the different competing teams, they decided to use the **f1-score**.

## Goals 🎯
The project has been cut into three steps :
- Part 1 : EDA in order how to get the keys insights of the data
- Part 2 : Models testing where I've been abble to test +30 different models, variying the estimators, the proprocessing, the hyperparameters...)
- Part 3 : Metrics analysis and definition of the best model depending on the business priorities + lever for action that would help to improve the newsletter's conversion rate

## Results 📬
🏆 Finally, the model that gives us the best F1 score on the test set remains the **Logistic Regression with an adjusted threshold**, achieving an F1 score of 0.764774.
- The Recall at 0.718954 indicates that the model captures the positive instances quite well, missing only 29% of the positives.
- While the Precision at 0.816832 demonstrates a high accuracy of the positive instances detected, being correct in 81% of the cases.

⚖️ Depening on business priorities:
- If we wish to maximize the accuracy of the positive predictions without missing too many of the positive cases (maximizing Precision), we could increase the threshold.
- If our priority is to capture the maximum number of positive instances (prioritizing Recall), we could decrease the threshold.

### Metrics for best models tested
| Model                                             | Set   | Accuracy | Precision | Recall | F1-score |
|---------------------------------------------------|-------|----------|-----------|--------|----------|
| Logistic Regression_optimal_threshold_0.42        | Train | 0.98599  | 0.81900   | 0.72622 | 0.76982  |
| Logistic Regression_optimal_threshold_0.42        | Test  | 0.98573  | 0.81683   | 0.71895 | 0.76477  |
| Logistic Regression_interaction_features_threshold: 0.4 | Train | 0.98585  | 0.80824   | 0.73614 | 0.77051  |
| Logistic Regression_interaction_features_threshold: 0.4 | Test  | 0.98538  | 0.79952   | 0.72985 | 0.76310  |
| Logistic Regression_optimal_threshold_0.47        | Train | 0.98623  | 0.84235   | 0.70491 | 0.76753  |
| Logistic Regression_optimal_threshold_0.47        | Test  | 0.98601  | 0.84211   | 0.69717 | 0.76281  |
| Logistic Regression_interaction_features_threshold: 0.38 | Train | 0.98557  | 0.79606   | 0.74316 | 0.76870  |
| Logistic Regression_interaction_features_threshold: 0.38 | Test  | 0.98517  | 0.78904   | 0.73747 | 0.76239  |
| Logistic Regression_interaction_features_threshold: 0.45 | Train | 0.98612  | 0.83134   | 0.71472 | 0.76863  |
| Logistic Regression_interaction_features_threshold: 0.45 | Test  | 0.98584  | 0.83140   | 0.70370 | 0.76224  |
| Logistic Regression_optimal_threshold_0.4         | Train | 0.98593  | 0.80938   | 0.73747 | 0.77175  |
| Logistic Regression_optimal_threshold_0.4         | Test  | 0.98531  | 0.79762   | 0.72985 | 0.76223  |
| Logistic Regression_interaction_features_threshold: 0.42 | Train | 0.98598  | 0.81728   | 0.72815 | 0.77015  |
| Logistic Regression_interaction_features_threshold: 0.42 | Test  | 0.98556  | 0.81335   | 0.71678 | 0.76202  |
| GradientBoostingClassifier optuna                  | Train | 0.98618  | 0.84507   | 0.69983 | 0.76563  |
| GradientBoostingClassifier optuna                  | Test  | 0.98601  | 0.84483   | 0.69390 | 0.76196  |
| Logistic Regression_optimal_threshold_0.45        | Train | 0.98623  | 0.83465   | 0.71484 | 0.77011  |
| Logistic Regression_optimal_threshold_0.45        | Test  | 0.98580  | 0.83119   | 0.70261 | 0.76151  |
| xgb.XGBClassifier optuna                          | Train | 0.98653  | 0.85217   | 0.70467 | 0.77143  |
| xgb.XGBClassifier optuna                          | Test  | 0.98598  | 0.84371   | 0.69390 | 0.76151  |




## Levers of action 🎯
![Description de l'image](https://github.com/myriamgoyet/supervised-ML--conversion-rate/blob/main/metrics/Coeff.png)


➡️ To increase the conversion rate, the newsletter company should focus on enhancing the attractiveness of the website pages to encourage readers to visit more pages and to attract new users to revisit the website.

➡️ German readers seem to be more passionate about the newsletter, even though they represent only a small percentage of the total readership. Communicating externally in Germany could help the newsletter attract new readers.



