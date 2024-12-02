# FakeNewsDetection1
Model Building
The model used in this project is based on an LSTM (Long Short-Term Memory) neural network, which is well-suited for handling sequential data like text. The steps involved in building the model include:

Text Preprocessing:

Tokenization of text data to convert words into sequences of numbers.
Padding sequences to ensure uniform input shape for the model.
Splitting the dataset into training and testing subsets.
LSTM Model Architecture:

An Embedding Layer to convert word indices into dense vectors.
Multiple LSTM Layers to capture dependencies in text sequences.
Dropout Layers to prevent overfitting.
Fully connected Dense Layers with a sigmoid activation function for binary classification.
Hyperparameter Tuning:

RandomizedSearchCV was used for hyperparameter optimization.
Parameters such as embedding dimension, number of LSTM units, dropout rate, batch size, and number of epochs were tuned to achieve optimal performance.
Model Evaluation:

The model was evaluated on the test dataset using metrics like accuracy and validation loss.
Deployment
The model is deployed using Streamlit, a Python framework for building interactive web applications. The app allows users to input a news headline or body text and returns a prediction indicating whether the news is "Real" or "Fake."

Features of the App:
Interactive Input: Users can type or paste a news headline or body text into the app.
Prediction: The app predicts if the news is fake or real with a probability score.
User-Friendly Interface: Streamlit provides an intuitive UI, making it accessible to non-technical users.
