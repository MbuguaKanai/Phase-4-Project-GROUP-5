## RECOMMENDATION SYSTEMS

### PROJECT PHASE 4
![image](https://github.com/MbuguaKanai/Phase-4-Project-GROUP-5/assets/128227310/bf38a9e6-f776-4e44-8a8b-61461e1c6db2)

1. **Student name**: GROUP 5
2. **Student pace**: Part Time
3. **Scheduled project review date/time**: 27th August 2023
4. **Instructor name**: William Okomba & Noah Kandie

## Executive Summary

In a rapidly evolving digital landscape, customer expectations for personalized interactions have surged.In response to the challenge of assisting our customers in efficiently navigating our diverse product catalog, we are embarking on a transformative journey to implement a state-of-the-art recommendation system. 

This visionary initiative aims to provide tailored product suggestions that resonate with individual preferences and interests. The projects entails; **Data Analysis -Explorative Data Analysis (EDA)**: Our journey commences with Exploratory Data Analysis (EDA), a crucial step in deciphering user behaviors. 

Through Univariate EDA, we meticulously dissect data, uncovering hidden patterns and trends that will underpin our personalized recommendation engine. **Algorithm Development** Our team of skilled data scientists crafts advanced algorithms, including collaborative filtering and matrix factorization, to generate accurate and relevant suggestions.

**Modelling** - We deploy a combination of models to ensure the highest quality of personalized suggestions for users. Here's an overview of the models utilized.

1. **Baseline Model**: K-Nearest Neighbors (KNN) Our modeling journey starts with a strong foundation—the K-Nearest Neighbors (KNN) baseline model. This model forms the bedrock of our recommendations by identifying similarities between users or items.

2. **KNNWithMeans** Building on the KNN baseline, we introduce KNNWithMeans, a variant that factors in user and item means. This approach compensates for potential rating biases, ensuring more balanced recommendations.

3. **KNNBasic** KNNBasic is a simplified yet effective version of the KNN algorithm. It prioritizes simplicity and computational efficiency, making it an optimal choice for scenarios where rapid recommendations are essential.

4. **Singular Value Decomposition (SVD)** One of the pillars of our modeling arsenal is Singular Value Decomposition (SVD). This powerful technique decomposes the user-item interaction matrix into latent factors.

Model Training Rigorous training and fine-tuning ensure that our Recommender System evolves, adapting to changing user behaviors and preferences. Performance Evaluation: Through thorough testing and validation, we ensure that our system consistently delivers high-quality recommendations.

**Hybrid Approach** We synergize multiple recommendation strategies, combining content-based and collaborative filtering methods to provide comprehensive suggestions.

We deployed the model using the validation dataset and obtained an RMSE of 1.16.

## Business Understanding

Our customers often face difficulty in navigating our extensive product catalog to find items that match their preferences. To overcome this challenge, we aim to implement a recommendation system that provides tailored product suggestions that align with individual preferences and interests. The goal is to increase user engagement, improve conversion rates, boost customer satisfaction and drive revenue growth and bolster our market position.

## Project Objectives
* To increase Engagement - by suggesting products that resonate with customers' past behaviors, such as browsing history, purchases, and interactions.

* To Enhance Conversion Rates - by delivering recommendations that are more likely to lead to purchases, thereby driving revenue growth.

* To enhance Customer Satisfaction - by reducing the time and effort required for customers to find products of interest.

* To differentiate our platform by providing an innovative and user-centric feature.
   
## Data Understanding

Group 5 team used the “MovieLens” database, developed by the GroupLens research lab at the University of Minnesota.

Exploring the data to get a glimpse of:

* Shape of the data
* The column names
* The data types
* Statistical summary of the data
* Missing values
* The duplicates

## Data Description Report

After merging the 4 datasets, the data had 285,672 rows and 11 columns.The rows reduced to 233,213 after dropping rows that contaiend null values. The dataset consists of three main data types; float, integer, and object. The datatypses are well suited for the data they represent.

There are no duplicated rows in this dataset.

We did a ststistical summary on ratings as it is the only feature that would give meanigful insights. These are our conclusin based on the statistical summary... That the mean rating for the movies is 3.97

* The spread around the mean rating for the movies is 0.96.
* The least rating that a movie was given by a user is 0.5
* The highest rating given for moview was 5.
* 25% of the ratings were below 3.5
* Half of the ratings were below 4.

Summary of Features in the Dataset

* UserIdrater: Represents the user ID of the rater.

* MovieId: Represents the ID of the movie being rated.

* Rating: Represents the rating given by the user to the movie.

* Timestamprater: Represents the timestamp of when the rating was given.

* Title: Represents the title of the movie.

* Genres: Represents the genres associated with the movie.

* UserIdtag: Represents the user ID of the tagger.

* Tag: Represents the tag associated with the movie.

* Timestamptag: Represents the timestamp of when the tag was assigned

![image](https://github.com/MbuguaKanai/Phase-4-Project-GROUP-5/assets/128227310/4fd444e7-51b2-4784-8b8f-f45a3bf471b0)

## Conclusions

Our quest to build an optimal recommendation model started with the Vanilla KNNBaseline baseline, yielding an initial RMSE of 0.88 Over five iterations, we explored KNNBasic, KNNWithMeans, and SVD models, fine-tuning each through grid search for better performance.

An innovative hybrid model combining content-based cosine similarity and collaborative SVD emerged as a highlight. The truncated SVD model stood out, achieving an impressive RMSE of 0.29, showcasing its potential.

When applied to unseen data, our model achieved a reasonable RMSE of 1.16, with opportunities for further enhancement.

In summary, our iterative journey provided insights into recommendation systems, emphasizing the efficacy of hybrid SVD techniques for improved predictive accuracy across various datasets.

## Recommendations

1. Consider expanding hyperparameter search using RandomizedSearchCV followed by fine-tuning with GridSearchCV for improved model performance.
2. Evaluate the model using a variety of metrics like precision, recall, MAP, and NCGD on a separate validation set to avoid overfitting.
3. Experiment with different weight combinations for content-based and collaborative predictions in the hybrid model to optimize recommendation accuracy.
4. Continuously monitor and retrain the deployed model with new data to ensure consistent predictive quality in real-world scenarios.
5. Enhance scalability by implementing distributed computing frameworks like Spark to handle large datasets more efficiently.
6. Create more comprehensive user and item profiles by incorporating features such as descriptions, demographics, and historical behavior.
7. Solve the cold start problem by employing strategies like content-based recommendations for new users or items.
8. Improve user trust and engagement by implementing mechanisms to provide explanations for the recommended items.

## Way Forward

* Enhance the recommendation system by implementing comprehensive model selection.
* Optimize the Hybrid model.
* Continuous monitoring and training of the model

