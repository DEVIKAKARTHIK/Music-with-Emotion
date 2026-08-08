# 🎵 Facial Emotion-Based Music Recommendation System

## Overview

Facial Emotion-Based Music Recommendation System is a Deep Learning application that detects a person's emotion from a facial image and recommends music based on the detected emotion. The system uses Computer Vision techniques for image processing and a Convolutional Neural Network (CNN) trained with ArcFace Loss (ArcLoss) for emotion classification.

The application identifies six emotions and automatically recommends songs corresponding to the detected emotional state.

---

## Objectives

* Detect human emotions from facial images.
* Classify emotions using Deep Learning.
* Recommend suitable music based on the detected emotion.
* Provide a simple and interactive user interface using Gradio.

---

## Emotion Categories

The model classifies facial expressions into the following categories:

* Angry
* Ahegao
* Sad
* Happy
* Neutral
* Surprise

---

## Dataset

The dataset consists of facial images organized into separate folders for each emotion category.

```text
dataset/
│
├── Angry/
├── Ahegao/
├── Sad/
├── Happy/
├── Neutral/
└── Surprise/
```

Images were preprocessed and augmented before training to improve model performance and reduce overfitting.

---

## Data Augmentation

Albumentations library was used for image augmentation:

* Resize (256 × 256)
* Horizontal Flip
* Random Brightness Adjustment
* Random Contrast Adjustment

These techniques increase dataset diversity and improve model generalization.

---

## Technologies Used

### Programming Language

* Python

### Deep Learning

* TensorFlow
* Keras

### Computer Vision

* OpenCV

### Data Processing

* NumPy
* Pandas

### Data Augmentation

* Albumentations

### User Interface

* Gradio

### Visualization

* Matplotlib
* Seaborn

---

## Model Architecture

The emotion recognition model is built using a Convolutional Neural Network (CNN).

Key features:

* Multiple Convolution Layers
* Pooling Layers
* Dropout Regularization
* Dense Layers
* Softmax Output Layer
* ArcFace Loss (ArcLoss)

ArcLoss helps improve class separation and increases classification performance.

---

## System Workflow

1. Load facial image.
2. Preprocess image using OpenCV.
3. Resize image to the required input size.
4. Pass image to the trained CNN model.
5. Predict facial emotion.
6. Match emotion with corresponding music playlist.
7. Display detected emotion and play recommended song.

---

## Emotion-Based Music Recommendation

| Emotion  | Recommended Music |
| -------- | ----------------- |
| Angry    | Angry.mp3         |
| Ahegao   | Ahegao.mp3        |
| Sad      | Sad.mp3           |
| Happy    | Happy.mp3         |
| Neutral  | Neutral.mp3       |
| Surprise | Surprise.mp3      |

---

## Features

* Facial emotion recognition
* Deep Learning-based prediction
* Music recommendation system
* Image upload support
* Interactive Gradio interface
* Emotion visualization
* Automated song selection

---

## Project Structure

```text
emotion-music/
│
├── dataset/
│   ├── emotion/
│   └── songs/
│
├── xtrain.npy
├── xtest.npy
├── ytrain.npy
├── ytest.npy
│
├── best_model.h5
├── training_history.json
│
├── project.ipynb
│
└── README.md
```

---

## Results

The trained model successfully detects facial emotions and recommends music based on the predicted emotional state.

Performance was evaluated using:

* Accuracy
* Precision
* Recall
* Confusion Matrix

Training and validation metrics were visualized using Matplotlib.

---

## Future Enhancements

* Real-time webcam emotion detection
* Spotify API integration
* Personalized playlist recommendation
* Mobile application support
* Additional emotion categories
* Multilingual music recommendation

---


