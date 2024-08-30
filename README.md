
# HopeBot - A mental health chatbot 

## Overview

This project implements a chatbot designed to handle various user inputs, including detecting potential suicide risks, providing stress management suggestions, recommending websites, and engaging users in games. The chatbot uses machine learning models to process and respond to user queries effectively.

## Features

- **Suicide Risk Detection**: Identifies if the user is expressing potential suicidal thoughts and provides appropriate responses.
- **Keyword Matching**: Responds based on specific keywords found in user input.
- **Intent Matching**: Uses predefined intents and patterns to generate responses.
- **Stress Management**: Offers suggestions for managing stress.
- **Game Interaction**: Allows users to play various text-based games, such as trivia quizzes and puzzles.
- **Website Recommendations**: Provides links and resources based on user requests.

## Prerequisites

To run this project, you need to have the following Python libraries installed:

- `joblib`
- `numpy`
- `scikit-learn`
- `pandas`
- `nltk` (for some NLP functionalities, if needed)
- `re` (part of Python standard library)

You can install the required libraries using pip:

```bash
pip install joblib numpy scikit-learn pandas nltk
```

## Files

- **`intents.json`**: Contains predefined intents and patterns for matching user queries.
- **`keywords.csv`**: A CSV file with keywords and corresponding responses for keyword matching.
- **`vectorizer.pkl`**: A pickled TF-IDF vectorizer used for transforming user input.
- **`model1.pkl`**: A pickled Logistic Regression model for detecting potential suicide posts.

## How to Use

1. **Load Models and Data**:
   Ensure that the `vectorizer.pkl` and `model1.pkl` files, as well as `intents.json` and `keywords.csv`, are in the correct paths specified in the script.

2. **Run the Script**:
   Execute the script to interact with the chatbot. The `get_response` function processes user input and generates appropriate responses based on the implemented features.

3. **Testing**:
   The script includes a set of test inputs to validate the chatbot's responses. You can modify or add new test cases as needed.

## Functions

- **`preprocess_input(user_input)`**: Preprocesses user input by converting to lowercase and removing special characters.
- **`detect_suicide(user_input)`**: Checks if the user input indicates a potential suicide risk.
- **`match_intent(user_input, intents)`**: Matches user input against predefined intents and returns a response.
- **`match_keyword(user_input, keywords)`**: Matches user input against keywords and returns a response.
- **`get_response(user_input)`**: Processes user input and generates a response based on various criteria.

## Example Usage

```python
test_inputs = [
    "I am sad",
    "I want to die",
    "Hello there",
    "angry"
]

for test_input in test_inputs:
    print(f"User Input: {test_input}")
    print(f"Response: {get_response(test_input)}\n")
```


## Contact

For any questions or issues, please contact. Details in are in my github profile.

## Project is made By Tannu Rawat, Jaina Pal , Tanushi Vermma


