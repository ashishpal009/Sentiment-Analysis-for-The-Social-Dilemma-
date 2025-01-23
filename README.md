# Twitter Sentiment Analysis for "The Social Dilemma"

## Project Overview
"The Social Dilemma" is a documentary-drama hybrid that explores the impact of social networking on society. Following its release on September 9th, 2020, the hashtag **#TheSocialDilemma** trended on Twitter, reflecting user sentiments about the documentary. This project aims to analyze and classify these tweets into three sentiment categories: **Positive**, **Neutral**, and **Negative**.

---

## Goal
The goal is to build a Recurrent Neural Network (RNN)-based deep learning model to:
- Categorize tweets into three sentiment categories.
- Achieve the best possible accuracy using only RNN (without LSTMs or traditional ML models).

---

## Data Description
The dataset contains nearly 20,000 tweets extracted using the Twitter API. Key attributes include:

### Attributes:
1. **user_name**: The Twitter handle of the user.
2. **user_location**: The location specified by the user.
3. **user_description**: A short bio written by the user.
4. **user_created**: The account creation date and time.
5. **user_followers**: Number of followers.
6. **user_friends**: Number of accounts the user is following.
7. **user_favourites**: Total number of tweets favorited by the user.
8. **user_verified**: Whether the account is verified.
9. **date**: Date and time when the tweet was posted.
10. **hashtags**: Other hashtags included in the tweet along with #TheSocialDilemma.
11. **source**: The platform or app used to post the tweet (e.g., web).
12. **is_retweet**: Indicates if the tweet is a retweet.
13. **clean_text**: The preprocessed text of the tweet.
14. **Sentiment (target)**: The sentiment of the tweet, categorized as Positive, Neutral, or Negative.

### Data Files
1. **Train_data**: Used to train the model.
2. **Test_data**: Used to generate predictions after training.

---

## Steps Performed

### 1. Data Cleaning and Preprocessing
- Removed special characters, numbers, and unnecessary symbols from the text.
- Converted all text to lowercase for uniformity.
- Removed stopwords to focus on meaningful words in the tweets.

### 2. Building the RNN Model
- Developed a Recurrent Neural Network (RNN) architecture.
- Used embedding layers for word representations.
- Trained the model on the cleaned text data.

### 3. Model Evaluation
- Evaluated the model on the test data using accuracy as the primary metric.
- Generated predictions for sentiment categories: Positive, Neutral, and Negative.

---

## Requirements
### Libraries
Install the following libraries to run the project:
```bash
pip install tensorflow numpy pandas matplotlib nltk

## Steps to Run the Project

3. **Train the Model:**
   - Run the training script:
     ```bash
     python train_rnn.py
     ```

4. **Test the Model:**
   - Run the testing script to generate predictions:
     ```bash
     python test_rnn.py
     ```

5. **View Results:**
   - Predictions and accuracy scores will be displayed in the console and saved in a `results.csv` file.


## License
This project is open-source and available for educational and research purposes.
