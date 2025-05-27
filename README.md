# 🧠 Sign Language Detection using Deep Learning

This project uses a Convolutional Neural Network (CNN) model to detect American Sign Language (ASL) hand signs from images. It includes a web app built using Gradio to interact with the model using webcam or image upload.

## 📁 Dataset

Dataset used: [ASL Alphabet Dataset](https://www.kaggle.com/datasets/debashishsau/aslamerican-sign-language-aplhabet-dataset)

Downloaded using `kagglehub` in Colab.

## 🏗️ Model Architecture

- 3 Convolutional layers
- MaxPooling after each conv layer
- Flatten + Dense + Softmax for classification
- 29 output classes (A–Z + special characters)

## 📊 Accuracy

- accuracy: 0.9955 - loss: 0.0176 - val_accuracy: 0.8018 - val_loss: 3.7273
- Training samples: 178,472
- Validation samples: 44,602
- 29 classes detected

## 🎮 Gradio Web App

You can run the Gradio interface in Colab or locally to interact with the model:

```python
import gradio as gr
# (see Sign_language_detection.ipynb for full code)
