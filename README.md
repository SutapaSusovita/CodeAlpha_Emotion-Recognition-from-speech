# CodeAlpha_Emotion-Recognition-from-speech
# 🎤 Speech Emotion Recognition (SER) Using CNN and Audio Features

This project focuses on detecting emotions from human speech using machine learning and deep learning techniques, primarily leveraging CNNs and audio signal processing.

---

## 📚 Datasets Used

This project combines multiple emotional speech datasets:

- [RAVDESS](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio)
- [TESS](https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess)
- [CREMA-D](https://www.kaggle.com/datasets/ejlok1/cremad)
- [SAVEE](https://www.kaggle.com/datasets/ejlok1/surrey-audiovisual-expressed-emotion-savee)
- [Speech Signal Features (MFCC, Chroma, etc.)](https://www.kaggle.com/datasets/mostafaabdlhamed/speech-signal-features)

---

## ⚙️ Features Extracted

The model is trained on audio features extracted from each sample:

- MFCC (Mel-Frequency Cepstral Coefficients)
- Chroma
- Spectral Contrast
- Tonnetz

Audio augmentation techniques used:
- Noise injection
- Time shifting
- Pitch scaling

---

## 🧠 Model Architecture

The core model is a **Convolutional Neural Network (CNN)** trained on extracted features.

- Input: reshaped 2D features (e.g., MFCCs)
- 2–3 convolution layers
- Batch Normalization & Dropout
- Dense + Softmax output for emotion classification

Other classifiers tried:
- Random Forest
- SVM
- Decision Tree (for baseline)

---

## 🏷️ Target Emotions

Classes typically include:
- Happy
- Sad
- Angry
- Fearful
- Disgust
- Calm
- Surprise
- Neutral
