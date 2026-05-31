# Face-Emotion-Recognition
This project implements a Facial Emotion Recognition (FER) system using Transfer Learning with MobileNet and a Self-Attention mechanism.  The model is trained on the RAF-DB dataset and classifies facial expressions into seven emotions:  - Anger - Disgust - Fear - Happiness - Neutral - Sadness - Surprise

# Architecture
```
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
```
# Dataset

Dataset: RAF-DB (Real-world Affective Faces Database)

Number of Classes: 7

The dataset is not included in this repository due to licensing restrictions.

# How to Run

## On Google Colab (Recommended)

1. Upload `FACE_EMOTION.ipynb` to Google Colab
2. Mount your Google Drive:
```python
   from google.colab import drive
   drive.mount('/content/drive')
```
3. Place the RAF-DB dataset in your Drive at:
```
   MyDrive/RAFDB_DATASET/
```
4. Run all cells top to bottom: **Runtime → Run All**

## Locally

1. Clone the repository:
```bash
   git clone https://github.com/your-username/face-emotion-detection.git
   cd face-emotion-detection
```
2. Install dependencies:
```bash
   pip install -r requirements.txt
```
3. Update the dataset path in Cell 1 of the notebook to your local path:
```python
   PATH_PREFIX = '/your/local/path/to'  # change this
```
4. Launch Jupyter and run the notebook:
```bash
   jupyter notebook FACE_EMOTION.ipynb
```
