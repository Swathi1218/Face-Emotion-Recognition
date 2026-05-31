# Face-Emotion-Recognition
This project implements a Facial Emotion Recognition (FER) system using Transfer Learning with MobileNet and a Self-Attention mechanism.  The model is trained on the RAF-DB dataset and classifies facial expressions into seven emotions:  - Anger - Disgust - Fear - Happiness - Neutral - Sadness - Surprise

# Architecture

Input Image
      │
Data Augmentation
      │
MobileNet Backbone
      │
Custom Conv Feature Extractor
      │
Global Average Pooling
      │
Self Attention
      │
Dense Layer
      │
Softmax Classifier
      │
Emotion Prediction

# Dataset

Dataset: RAF-DB (Real-world Affective Faces Database)

Number of Classes: 7

The dataset is not included in this repository due to licensing restrictions.

# Installation

git clone https://github.com/yourusername/face-emotion-recognition.git

cd face-emotion-recognition

pip install -r requirements.txt

# Training

python src/train.py

# Evaluation

python src/evaluate.py
