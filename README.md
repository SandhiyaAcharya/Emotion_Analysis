# Emotion Recognition with Deep Learning

## Introduction
This GitHub repository contains code for a deep learning-based emotion recognition model. The model is built using Convolutional Neural Network (CNN), Long Short-Term Memory (LSTM), and DistilBERT pre-trained models. The dataset used for training and evaluation includes text data labeled with different emotions.

## Code Overview

### Libraries
- **neattext**: For text preprocessing, including tasks such as removing HTML tags, URLs, emojis, and more.
- **textblob**: For sentiment analysis.
- **transformers**: For working with pre-trained DistilBERT models.
- **contractions**: For expanding contractions in text.

### Data Loading
- The dataset is loaded from a CSV file (`emotion_dataset.csv`) using the Pandas library.

### Data Preprocessing
- Various text preprocessing steps are performed, including lowercasing, handling HTML tags, removing special characters and numbers, expanding contractions, removing punctuation, and removing stopwords.

### Data Splitting
- The dataset is split into training, validation, and testing sets.

### Model Building
#### CNN Model
- A Convolutional Neural Network (CNN) is built using TensorFlow and Keras.
- The model includes an embedding layer, convolutional layers, dense layers, and an output layer.
- The model is compiled using stochastic gradient descent (SGD) as the optimizer and sparse categorical crossentropy as the loss function.

#### LSTM Model
- A Long Short-Term Memory (LSTM) model is built using TensorFlow and Keras.
- The model includes an embedding layer, batch normalization, dropout, LSTM layers, and a dense output layer.
- The model is compiled using the Nadam optimizer and sparse categorical crossentropy as the loss function.

#### DistilBERT Model
- A pre-trained DistilBERT model for sequence classification is loaded using the Hugging Face `transformers` library.
- The model is fine-tuned on the emotion dataset using TensorFlow.

### Model Training
- The CNN and LSTM models are trained on the preprocessed text data.
- Training progress is monitored, and early stopping is applied to prevent overfitting.

### Model Evaluation
- The trained models are evaluated on the testing set.
- Evaluation metrics, such as accuracy, are displayed, and confusion matrices are generated.

### DistilBERT Fine-Tuning
- The pre-trained DistilBERT model is fine-tuned on the emotion dataset.
- Training progress and evaluation metrics are displayed.

### Model Saving
- The trained DistilBERT model is saved to a specified directory for later use.

Feel free to explore and modify the code to suit your needs! If you have any questions or suggestions, please open an issue or contribute to the repository.
