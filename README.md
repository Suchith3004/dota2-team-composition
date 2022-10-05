
# Dota2 Team Composition Generation w/ ML

CS5644 - Machine Learning with Big Data (Fall 2021)

Through a comparative analysis of 4 different ML models (Decision Trees, Random Forest, Naive Bayes and Logistic Regression) and an ANN on two different datasets, we attempt to create an effective model to predict Dota2 match outcomes based on the teams’ selection heroes, team and match characteristics. Specifically, given two sets of five heroes, team statistics, and the characteristics of the match, each model is trained to predict which team is more likely to win against the other team. 

In order to accomplish our goal of predicting which team variations (team players and their chosen heroes) have the best probability of winning a match, we model it as a supervised ML problem. 5 different classification models on two datasets were built to accomplish this task. For training, we will have the models classify a match between two teams as a winner or loser. For each model, 5-fold cross validation with shuffling of the folds was used to train, test, and score each model, to guarantee randomness and generalization. Within each fold, all the features were normalized using the standard scaler to ensure that the logistic regression model converged. Lastly, each model was scored with precision, recall, and f1 to evaluate and compare the effectiveness of the models on the classification task at hand. 

## Tech Stack

This project was primarily implmented in the Jupyter Lab enviornment. 

Python Libraries: Scikit-Learn, SciPy, Keras, TensorFlow

## Run Locally

Clone the project

```bash
  git clone https://github.com/Suchith3004/dota2-team-composition.git
```

Go to the project directory

```bash
  cd dota2-team-composition
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Extract Data

```bash
  tar -xzvf data.tar.gz
```
## Dataset

Both datasets were aggregated utilizing the [OpenDota API](https://docs.opendota.com/#). Further specifications about the dataset are included in "Dota2_Final_Project_Report.docx".
## Authors

- Suchith Suddala - [@suchith3004](https://www.github.com/suchith3004)
- Muhammad Ali Qadri - [@muhammadaliq](https://git.cs.vt.edu/muhammadaliq)
- Xiaolu Dedman - [@xiaolu92](https://git.cs.vt.edu/xiaolu92)
