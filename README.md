# Nutrigo(Building a Recommender System)
The goal of this project is to develop a recommender system that provides product recommendations.
# Tasks/Activities List:

	Data Collection
	Data Preprocessing
	Feature Engineering
	Recommender System
	Evaluation
	Integration
	User Interface/API
	Testing and Validation
	Model Refinement
	Documentation
	Deployment Plan

# Data :
We construct a dataset via collecting data from Allrecipes.com. The website is chosen since it is one of the largest food-oriented social networks with 1.5 billion visits per year. In particular, we crawl 52,821 recipes from 27 categories posted between 2000 and 2018. For each recipe, we crawl its ingredients, image and the corresponding ratings from users. To ensure the quality of the data, we filter recipes that do not have images and that contain repeated ingredients and zero reviews. Then we obtain raw_data, including 1,160,267 users, 49,698 recipes with 38,131 ingredients and 3,794,003 interactions , which contains files as following:

•	recipe_file:
each recipe information is presented in one line, which consists of recipe id, name, average ratings of reviewers, image url, review nums, ingredients, cooking directions, nutritions, and reviews.

•	interaction_file:
each interaction is presented in one line, which consists of user id, recipe id, rating, and dateLastModified.

•	images:
49,698 images, named with recipe_id.jpg.

Besides, in order to evaluate recommendation models’ performance, we holdout the latest 30% of interaction history to construct the test set, and split the remaining data into training (60%) and validation (10%) sets. Then we retain users which occur in both training and test sets, and obtain 68,768 users, 45,630 recipes with 33,147 ingredients and 1,093,845 interactions. We call this dataset as core_data, the dataset consists of files as following:

•	recipe_file: each recipe information is presented in one line, which consists of recipe id, name, image url, ingredients, cooking directions, nutritions.

•	interaction_file(train.rating/valid.rating/test.rating): each interaction is presented in one line, which consists of user id, recipe id, rating, and dateLastModified.

•	images: 45,630 images, named with recipe_id.jpg.

 | S.NO.| TOPIC | LINK |
|-|-|-|
|01| Problem Statement |(https://kh3-ls-storage.s3.us-east-1.amazonaws.com/Updated%20Project%20guide%20data%20set/Guide%20-%20Data%20Science%202.0%20Capstone%20Project.docx)
|02| Data Sources |(https://kh3-ls-storage.s3.us-east-1.amazonaws.com/Updated Project guide data set/NutriGro.zip)
|03| Model Traning & Preprocessing |(http://localhost:8888/notebooks/Nutrigo.ipynb#)
|04| Evaluation |(http://localhost:8888/notebooks/Nutrigo.ipynb#)
|05|Integretion |(http://localhost:8888/notebooks/Nutrigo.ipynb#)
|06| Model Refinement |(http://localhost:8888/notebooks/moodformusic.ipynb)



