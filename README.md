### Machine Learning Competition: Movie Rating Prediction

Welcome to my Machine Learning Competition Code! In this competition, our task was to predict movie ratings using a given set of training samples and outcomes, alongside a test set of samples without ground truth outcomes. You can locate these datasets in the data tab above.

#### Data Overview

The training samples consist of distinct films, each accompanied by metadata encompassing language, title, description, and more. The corresponding outcomes represent the average voter ratings, ranging from 0 to 10.

#### The Challenge

Our primary objective in this competition was to generate a test-outcomes CSV file that predicts the outcomes for each sample within the test set. 

#### Achievements

I'm delighted to share that my efforts bore fruit, earning me the esteemed first prize in this competition, prevailing over a competitive field of 60 applicants. This accolade was granted in recognition of achieving the highest R-squared score. My model successfully predicted average voter ratings for movies without the luxury of ground truth outcomes.




#### Approach:
Took the dataset and cleaned it making sure that there weren't any undefined values in the rows, and sorted the numerical and categorical columns. Then I did a column transformer depending on the type of column value it was. For numerical columns, I did a standard scalar. For categorical columns, I did a one-hote encoder. For the title, tagline, and overview I did a TFIDF Vectorizer. I created a pipeline with all these transformations with a random forest regressor. I created a test and train split to fine-tune my parameters and test accuracy. 


Let's journey through this codebase to delve into the intricacies of the competition and the strategies employed to conquer the challenge. Feel free to explore the data, dive into the code, and gain insights into how cutting-edge machine-learning techniques contributed to securing the top spot. Your exploration might offer inspiration and valuable insights for your own data science endeavors. Happy exploring!
