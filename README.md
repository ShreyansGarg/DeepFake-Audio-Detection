# DeepFake-Audio-Detection

Link: https://deepfake-audio-detection.streamlit.app/

# Introduction

With the rise of sophisticated AI technologies, deepfake audio has become a significant concern. These fabricated audio clips can be used for malicious purposes, such as spreading misinformation, committing fraud, or damaging reputations. Therefore, developing robust tools to detect deepfake audio is essential for maintaining the integrity of information and protecting individuals from potential harm.

# Project Overview

This project aims to detect deepfake audio clips by leveraging Convolutional Neural Networks (CNNs). By converting 2-second audio clips into spectrograms, we can utilize the power of CNNs to classify these images and determine the authenticity of the audio.

# Data Preprocessing

Audio Clips: The audio data is divided into 2-second clips to ensure uniformity and manageability.
Spectrogram Conversion: Each audio clip is converted into a spectrogram, which visually represents the frequency spectrum of the audio signal over time. This conversion transforms the problem into an image classification task suitable for CNNs.

# Model Architecture

A Convolutional Neural Network (CNN) is designed to classify the spectrograms. The general architecture of a CNN includes:

Convolutional Layers: These layers apply convolutional filters to the input images (spectrograms) to extract features such as edges, textures, and patterns.
Activation Functions: Typically, ReLU (Rectified Linear Unit) is used to introduce non-linearity.
Pooling Layers: These layers downsample the feature maps, reducing the spatial dimensions and retaining the most important information.
Fully Connected Layers: These layers act as classifiers on the extracted features.
Output Layer: The final layer uses a softmax activation function to provide probability scores for classification.

# Training and Evaluation

The model is trained using a labeled dataset of real and deepfake audio clips. The training process involves:

Loss Function: Cross-entropy loss is used to measure the difference between the predicted and actual labels.
Optimizer: Adam optimizer is used to adjust the weights of the network based on the loss function.

# Results

The model achieved an accuracy of 84% on the test dataset, demonstrating its effectiveness in detecting deepfake audio. Detailed performance metrics such as precision, recall, and F1-score are also evaluated to ensure the robustness of the model.

# Contributors
