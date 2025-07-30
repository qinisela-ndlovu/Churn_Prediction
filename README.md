# Data-Science-Challenge - Churn Prediction

This project is a fun data science challenge from Coursera, I was predicting which subscribers are likely to cancel their subscription to online video streaming company.
This challenge is testing your data science skills.

# 📌 Problem statement
Coursera: In this challenge, you'll get the opportunity to tackle one of the most industry-relevant maching learning problems with a unique dataset that will put your modeling skills to the test. Subscription services are leveraged by companies across many industries, from fitness to video streaming to retail. One of the primary objectives of companies with subscription services is to decrease churn and ensure that users are retained as subscribers. In order to do this efficiently and systematically, many companies employ machine learning to predict which users are at the highest risk of churn, so that proper interventions can be effectively deployed to the right audience.

# 📊 Dataset
Coursera provided all data needed to complete the challenge, everything was done on browser.

# source: Coursera
Features(before drop): AccountAge,MonthlyCharges,TotalCharges,SubscriptionType,PaymentMethod,PaperlessBilling,ContentType,MultiDeviceAccess,DeviceRegistered,ViewingHoursPerWeek,AverageViewingDuration,ContentDownloadsPerMonth,GenrePreference,UserRating,SupportTicketsPerMonth,Gender,WatchlistSize,ParentalControl,SubtitlesEnabled,CustomerID.
Target: Churn 

#  🧪 Approach:
1. EDA - I started with exploartion to understand the data, I wanted to see if there are missing values? how many rows and columns are there, and also their data types.
   then I visualised using matplot and seaborn to understand the relationship between columns, distribution(target) and also to see the collinearity in the features
2. The data had no missing values. but it contained numeric and categorical values, I preprocessed that using the pipeline for a cleaner code and dropped CustomerId column that I did not neeed for model training.
3. with the model selection - I selected XGBoost (Extreme Gradient Boosting) for this project because of its strong performance in structured/tabular data tasks and its ability to handle common data science challenges effectively. Specifically: (a) High predictive perfomance (b) Robustness to Missing Values and Outliers (c) Flexibility and Interpretability  (d)  Built-in Regularization
4. Evaluation - after submission, The system evaluates your predictions using the AUC metric on a hidden test set.
5. then you get your results ... which was 74% for me in this challenge
6. to pass you need at leat 50%


# 🧠 Key Learnings:
For now I used just one algorithm, XGBoost and I got the passing mark. but I will improve my score.
The first learning: I did not use the pipeline, the preprocessing process was done seperately which made my work big and the results were low.
After building a pipeline, the model took many minutes to train(approx 12 mins) then I tuned the parameters to make it fast yet efficient and alos the feature transforming was handled easily.
Pipelines with hyperparameter tuning are easy to reuse, modify, and deploy.
You can swap models or preprocessing steps without rewriting large parts of code.

# 📈 Results
Best model : for now XGBoost, 
AUC = 74% on test set

# Tools used:
Python

pandas, numpy

scikit-learn

matplotlib, seaborn

Jupyter Notebook

The prediction results.png shows the results after submission

   



