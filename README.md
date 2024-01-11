# Emotion Detection using NLP

This project aims to build and evaluate models for emotion detection in text data. We explore different architectures, including Convolutional Neural Networks (CNN), Long Short-Term Memory Networks (LSTM), and pre-trained transformer models like RoBERTa and DistilBERT.

## Dataset

We used the "emotion_dataset.csv" for training and evaluation. The dataset contains text samples labeled with different emotions.

## Setup and Dependencies

Ensure you have the necessary dependencies installed. You can install them using the following commands:

```bash
!pip install textblob
!pip install neattext
!pip install contractions
!pip install transformers
```

## Exploratory Data Analysis

We conducted exploratory data analysis to understand the distribution of emotions in the dataset, text length distribution, and preprocessing steps.

## Text Processing

We performed various text processing steps, including lowercasing, handling HTML tags, removing special characters, handling contractions, removing punctuation, and stopwords. Tokenization and lemmatization were also applied to reduce the feature space.

## Model Architectures

### CNN Model

We implemented a Convolutional Neural Network (CNN) model with embedding, convolutional, and dense layers. The model was trained on the preprocessed text data.

### LSTM Model

We implemented a Long Short-Term Memory Network (LSTM) model with bidirectional layers for sequence processing. The model was trained on the preprocessed text data.

### RoBERTa Pretrained Model

We used the RoBERTa transformer model with a fine-tuned classification head for emotion detection. The model was trained and evaluated using the Hugging Face `transformers` library.

### DistilBERT Pretrained Model

Similar to RoBERTa, we used the DistilBERT transformer model for emotion detection. The model was trained and evaluated using the Hugging Face `transformers` library.

## Model Evaluation

We evaluated the models on a test set and visualized their performance using accuracy, confusion matrices, and other relevant metrics.

## Results

The trained models achieved competitive performance in emotion detection on the provided dataset.

## Usage

To use the pre-trained models for emotion detection, you can follow the examples provided in the respective model sections. Make sure to install the required dependencies and load the models accordingly.


Feel free to contribute, provide feedback, or use the models for your own applications.

