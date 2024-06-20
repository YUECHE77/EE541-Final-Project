# Sentence Bert movie recommendation system
#
# *I rewrite this project, please refer to my new repository: https://github.com/YUECHE77/Movie-Recommendation-System-with-Bert*
#
### Required libraries:
#### pandas, numpy, matplotlib, seaborn, json, random, logging, sklearn, torch, sentence_transformers, transformers

### FinalProcessing.ipynb 
#### is used for preprocessing the data. Before running, place the dataset in a folder named "dataset". "dataset" folder is in the same directory as the code. When run, the code automatically creates four new datasets and stores them in the "dataset" folder. These new datasets will be used in the FinalRecommender.ipynb run.

### FinalRecommender.ipynb 
#### is used for model traing and test the functionality. Running FinalRecommender.ipynb requires a new dataset created by FinalProcessing.ipynb. Running the model.fit() function, the results of the training are saved in the "model/training_nli_distilbert-model" path. So first you need to create a folder named "model", and then create a folder named "training_nli_distilbert-model" under it. If you want to use a model, then just use "model = SentenceTransformer(output_path)". (output_path: for example -> "model/training_nli_distilbert-model")

### resultAnalysis.ipynb 
#### is used to visualize the performance evaluation results during model training. The path where the model is saved during training, e.g. "model/training_nli_distilbert-model", there will be a folder "eval" underneath, where the csv file in the "eval" is the result of the evaluation. Change the path if you want to run the code.

## A portion of the timeline:

## Still in progress - 04/29/2024
#### The dataset: Kaggle - The Movies Dataset: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset - to download it.
#### Recommend the movies using user's watching history, inputs (movies' titles), or the movies' indices.

## Update - 05/02/2024
#### User can even input the movies' titles that are not in the dataset, the system will still gives recommendations.
#### Recommend_with_history now will consider the timestamps and the ratings. The system will recommend the movies that the users have recently watched and liked the most.
#### Finished "From genres to movies": input a LIST of genres, return a LIST of movies titles.
#### Several edge cases were dealt with. The code should be more robust now.

## Finished - 05/04/2024
