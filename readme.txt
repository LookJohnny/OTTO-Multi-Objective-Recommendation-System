1 Download the data to the input folder
https://www.kaggle.com/datasets/columbia2131/otto-chunk-data-inparquet-format
https://www.kaggle.com/datasets/cdeotte/otto-validation
https://www.kaggle.com/competitions/otto-recommender-system/data
https://www.kaggle.com/datasets/radek1/otto-full-optimized-memory-footprint

2 Run the word2vec training model word2vec-train.ipynb; recommended to use kaggle's GPU training

3 Run the model validation code in turn
Run the recall program code/recall_valid.ipynb; it is recommended to use kaggle's GPU training
Run the feature program code/feature_prepare_valid.ipynb
Run the ranking model code/rank_model_valid.ipynb
There are three types of code to run, and the parameter t=clicks/carts/orders can be modified
The number of recalls can be modified, the default is 50, and it can be modified to 250. The more recalls, the better the score

4 Run the model prediction code in turn
Run the recall program code/recall_test.ipynb; it is recommended to use GPU training from kaggle
Run the feature program code/feature_prepare_test.ipynb
Run the ranking model code/rank_model_test.ipynb, and get the submission file submission.csv


Key code packages
pandas
numpy
lightgbm
cudf
gensim

Recommended memory 128G, the code needs to run for 48 hours




