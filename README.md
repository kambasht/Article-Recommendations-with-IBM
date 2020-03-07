# Article-Recommendations-with-IBM
Recommendation system for users on the IBM Watson Studio Platform for articles based on top n ranking, collaborative filtering and latent features

# Table of Contents
1. Project Motivation
2. Project Tasks
3. File Descriptions
4. Running the code
5. Results
6. Licensing, Authors, and Acknowledgements

## Project Motivation

Recommendation systems have gained immense popularity in recent times primarily due to the advent of Big Data and user-specific data available on proprietary platforms. Platforms like Netflix, Spotify, YouTube and Amazon are the most common examples of how effective recommendation systems can be for user engagement ultimately leading to a increase in customer satisfaction and revenue growth.

For my project here, I am using data provided by IBM to analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles they will like

## Project Tasks

I. Exploratory Data Analysis

Exploring the data to find patterns and dive into the details of the provided dataset

II. Rank Based Recommendations

We look at the most popular articles simply based on the most interactions. We assume that the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

III. User-User Based Collaborative Filtering

we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users.

IV. Matrix Factorization

An attempt to complete a machine learning approach to building recommendations. Using the user-item interactions, we will build out a matrix decomposition. Using our decomposition, we will get an idea of how well we can predict new articles an individual might interact with.

V. Conclusion

## File Descriptions

articles_community.csv - file that contains the details for each article. the columns are the article-id , its status on the platform, the article body, description and full name

user-item-interactions.csv - file that contains the raw data for every user interaction with an article per row. The three columns are article-id , the title of the article and the email of the user who interacted with the article.

## Running the code

Installations required before running the code:
- no external libraries are required for installation

Folder structure:
- Place all the test files, data files and the jupyter notebook from the repo into a single folder and then run the notebook

## Results
Rank based recommendations are fairly straight forward for recommending it to both existing as well as new users.

User based collaborative filtering makes it easier for us to find users based on similar interests and provide them related recommendation.

A challenge that we face is in the form of a 'cold start problem' where we need to improve on providing recommendations to new users on the platform where we dont have enough information to start with. A relatively simple form of recommendation in this case is either rank based or knowledge based filtering i.e. initial "interests" gathered from a series of questions to the user to start off with.


## Licensing, Authors, Acknowledgements
Credits to [IBM](https://www.ibm.com/us-en/?ar=1) for the dataset and [Udacity](https://www.udacity.com/) for the skeleton structure for the code.
