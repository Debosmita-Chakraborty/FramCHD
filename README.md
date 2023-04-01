# FramCHD
Predicting the 10 year risk of CHD (coronary heart disease) using a random forest classifier on the Framingham Heart Study dataset.

## Context
This was my very first personal project! It was a thrilling ride, from applying what I've learnt to getting stuck in roadblocks and figuring my way out, and best of all, learning new things along the way!

Now, about the project. I chose it mainly to highlight (and develop) my exploratory data analysis skills: to examine the relationships between different risk factors, which ones affected the target variable and how/to what extent, visualising those relationships, and drawing conclusions and insights from the data. After cleaning the data, I also tried my hand at building a machine learning model to try and predict the outcome based on the risk factors. The result? A 90% accurate random forest classifier for predicting CHD!

## Skills
Skills shown:
* Exploratory data analysis
* Data visualisation
* Data cleaning
* Implementing ML model (Random Forest)

New Skills Learnt:
* Oversampling and undersampling

## Process
* I first examined the structure of the dataset to learn about the features and then started examining their relationships with each other via boxplots, countplots, barplots, etc. Some factors (like smoking) had greater effects on the target variable than others (like cholesterol).
* Next I started to clean the data and handle the missing values. Most of them were a small part of the dataset whose removal did not affect its structure, so they were deleted, while the remaining were imputed.
* The target variable (10 year risk of CHD) could have only two outcomes, 0 (no CHD) and 1 (CHD). Therefore to predict this outcome was a classification problem of supervised learning. For my model I went with a random forest.
* A problem that I faced was that my data was imbalanced, with the majority of people having TenYearCHD=0. I knew that this was making my model biased, but did not know how to handle it as I had learnt ML on cleaner datasets.
* I discovered the technique of oversampling and undersampling using the imblearn library, tried it out and found that the two combined gave me the best results.

Check out my notebook for the final result!
