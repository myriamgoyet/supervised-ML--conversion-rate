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



➡️ To increase the conversion rate, the newsletter company should focus on enhancing the attractiveness of the website pages to encourage readers to visit more pages and to attract new users to revisit the website.

➡️ German readers seem to be more passionate about the newsletter, even though they represent only a small percentage of the total readership. Communicating externally in Germany could help the newsletter attract new readers.



