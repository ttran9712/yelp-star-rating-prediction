# yelp-star-rating-prediction
Goal: Accurately classify Yelp Reviews into 1 star or 5 star categories based off the text content in the reviews

Data: Yelp Review Data Set from Kaggle (yelp.csv).

Each observation in this dataset is a review of a particular business by a particular user.

The "stars" column is the number of stars (1 through 5) assigned by the reviewer to the business. (Higher stars is better.) In other words, it is the rating of the business by the person who wrote the review.

The "cool" column is the number of "cool" votes this review received from other Yelp users.

All reviews start with 0 "cool" votes, and there is no limit to how many "cool" votes a review can receive. In other words, it is a rating of the review itself, not a rating of the business.

The "useful" and "funny" columns are similar to the "cool" column.

# Data
![ttran9712/yelp-star-rating-prediction/main/blob](images/data.png)

Get descriptive statistics for data

![ttran9712/yelp-star-rating-prediction/main/blob](images/descriptive_stats.png)

# Exploratory Data Analysis
Histogram: Text length based on star review

![ttran9712/yelp-star-rating-prediction/main/blob](images/EDA_01.png)

Boxplot: Text length based on star review

![ttran9712/yelp-star-rating-prediction/main/blob](images/EDA_02.png)

Number of occurrences for each type of star rating

![ttran9712/yelp-star-rating-prediction/main/blob](images/EDA_03.png)

Mean values grouped by star rating

![ttran9712/yelp-star-rating-prediction/main/blob](images/EDA_04.png)

![ttran9712/yelp-star-rating-prediction/main/blob](images/heatmap.png)

# Model evaluation
Confusion matrix and classification report

![ttran9712/yelp-star-rating-prediction/main/blob](images/model1_eval.png)

Model performed well. Will including TF-IDF (statistical measure that evaluates how relevant a word is to a document in a collection of documents) in this process using SciKit Learn's pipeline improve the model?

# Text Processing: using Term Frequency-Inverse Document Frequency (TF-IDF)
Confusion matrix and classification report after using SciKit Learn's pipeline

![ttran9712/yelp-star-rating-prediction/main/blob](images/model2_eval.png)

Tf-Idf worsened model based on evaluation metrics.
