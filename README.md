# Sentiment Analysis on Yelp Reviews

This project aims to apply Machine Learning techniques to perform Sentiment Analysis on Yelp reviews. The goal is to determine the sentiment expressed in the reviews by rating it with 1 to 5 stars and create a appropriate answer for the review.

## About the Project

This project was created by [Dino Pelesevic](https://github.com/peledin) as part of the 'Machine Learning II (2023-FS) module' at [ZHAW](https://www.zhaw.ch/en/university/).

## Motivation

At one point in my professional career, I was responsible for replying to comments on our Google Business account. Based on the experiences I had there, I came up with this project idea.

The increasing number of reviews on platforms like Yelp has made it difficult to manually keep track and make sense of the sentiments expressed by customers. This project aims to address this challenge by building a model that can automatically classify the sentiment expressed in a review, aiding in better understanding customer satisfaction and improving services.

The ultimate goal is to predict the sentiment of the review, and then use another model to write an appropriate response to the review. In this project, this approach was tried with a Flan-T5 model.

The solution is intended to help business owners (or younger-me) handle the large volume of reviews and generate appropriate responses.

# Repository Structure

Here's a list of main files in the repository:

- 1 - DatasetExploration.ipynb: This notebook contains initial exploration of the dataset.
- 2.1 - ModelTraining.ipynb: This notebook includes the main setup for training the model.
- 2.2 - ModelComparison.ipynb: This notebook contains the setup for comparing different models.
- 3 - ReviewResponder.ipynb: This notebook generates answers to the reviews based on their sentiment with the Flan-T5 model.
- DatasetCutter.ipynb: This notebook is used for cutting the dataset into manageable size.

The repository also includes the following directories:

- data: Contains the some of the datasets used for the project. The larger ones can be downloaded on [Kaggle](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset?select=yelp_academic_dataset_review.json) or [Google Drive](https://drive.google.com/drive/folders/1D2e3uQXDbrhEiTnAlGF62cqIUYZh-gc-?usp=share_link)

- models: Contains the some of the trained models. The larger ones can be downloaded on [Google Drive](https://drive.google.com/drive/folders/1ZUQQVPfTmqWb4lilc-oHfScGVQdK2TgD?usp=share_link)
- src: Contains the source code for the project.
- images: Contains the images for the project.
- preprocessing: Contains the preprocessed data in chunks (for lower ram usage) and as a whole json-file. The whole preprocessed dataset (divided in 50'000 rows per chunk) can be downloaded on [Google Drive](https://drive.google.com/drive/folders/1qj9h7urE_vs-uaF6Ar_546yCYkDI6_4A?usp=share_link)

## Installation

To clone and run this project locally, follow the steps below:

- Clone the repository to your local machine

```bash
git clone https://github.com/peledin/ML2-Project.git
```

- Install the required Python packages using the following command

```bash
pip install -r requirements.txt.
```
