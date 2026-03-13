# SportBot-AI

SportBot-AI is a Natural Language Processing (NLP) based chatbot designed to answer sports-related questions. The system uses machine learning techniques such as TF-IDF Vectorization, Logistic Regression, and Cosine Similarity to understand user queries and provide the most relevant response from a dataset.

This project demonstrates how basic NLP and machine learning models can be used to build a simple question-answering chatbot.

## Features

* Sports question answering chatbot
* Intent classification using Logistic Regression
* Text vectorization using TF-IDF
* Response retrieval using Cosine Similarity
* Interactive terminal-based chatbot

## Technologies Used

* Python
* Pandas
* Scikit-learn
* NumPy
* Natural Language Processing (NLP)

## Project Structure

```
sportbot-ai
│
├── sports_chatbot.ipynb
├── README.md
└── requirements.txt
```

## Dataset

The dataset used in this project is stored externally due to file size limitations. It can be accessed using the Google Drive link below.

Dataset Link:
(https://drive.google.com/file/d/1V1B2MODxHNGebbBJwyfvMJ9TZWsJsg78/view?usp=drive_link)

The dataset contains the following columns:

| Column   | Description                       |
| -------- | --------------------------------- |
| question | Sports related questions          |
| intent   | Category of the question          |
| response | Chatbot response for the question |

## How the Chatbot Works

1. The dataset containing sports questions and responses is loaded.
2. Questions are converted into numerical vectors using TF-IDF Vectorizer.
3. A Logistic Regression model is trained to classify the intent of user queries.
4. When a user asks a question:

   * The input is converted into a TF-IDF vector.
   * The trained model predicts the intent.
   * Questions with the same intent are filtered from the dataset.
   * Cosine Similarity is used to find the most similar question.
5. The chatbot returns the corresponding response.

## Installation

Clone the repository:

```
git clone https://github.com/shahlaparakkottil/SPORTBOT-AI.git
```

Navigate to the project directory:

```
cd SPORTBOT-AI
```

Install required libraries:

```
pip install pandas scikit-learn numpy
```

## Running the Chatbot

Run the notebook or Python script and start interacting with the chatbot through the terminal.

Example:

```
Sports Chatbot Ready! Type 'exit' to stop.

You: Who won the FIFA World Cup 2018?
Bot: France won the FIFA World Cup 2018.

You: exit
Bot: Goodbye
```

## Machine Learning Methods Used

* TF-IDF Vectorization
* Logistic Regression
* Cosine Similarity

## Future Improvements

* Expand the dataset with more sports topics
* Add a web interface using Streamlit
* Improve intent detection using advanced NLP models
* Add voice interaction support

## Author

Developed as part of a machine learning and NLP learning project.
