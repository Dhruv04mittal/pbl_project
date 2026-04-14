# pbl_project
# Dhruv Mittal
# 23FE10CSE00708
# Title:- Sign Language Recognition Model
# Mentor:- Mr. Arvind Mehta


This project implements a real-time American Sign Language (ASL) hand gesture recognition system using Computer Vision and Deep Learning. The system captures hand gestures via webcam, processes them, and predicts the corresponding ASL alphabet.

Overview

The pipeline consists of:

Image data collection using OpenCV
Preprocessing (grayscale conversion, resizing to 48×48)
CNN-based model training using TensorFlow
Real-time prediction using webcam input

The model is designed to classify ASL alphabets with high accuracy under controlled lighting and background conditions.

Tech Stack
Python
TensorFlow / Keras
OpenCV
NumPy
Dataset

Custom dataset created using webcam input:

Hand gesture images captured in real-time
Grayscale images of size 48×48
Organized into labeled directories (A–Z)
Model Architecture
Convolutional Neural Network (CNN)
Multiple Conv + ReLU + MaxPooling layers
Fully connected dense layers
Softmax output layer for multi-class classification
Training Details
Loss Function: Categorical Crossentropy
Optimizer: Adam
Evaluation Metrics:
Accuracy
Precision
Recall

Model trained for 100 epochs with performance stabilizing in later stages.

Performance
Achieved strong classification accuracy on training and validation data
Performs well in real-time detection with minimal latency
Sensitive to lighting variations and background noise
Features
Real-time ASL gesture detection via webcam
Custom dataset generation pipeline
End-to-end ML workflow (data → training → prediction)
Lightweight model suitable for local execution
Limitations
Requires consistent lighting conditions
Background noise can reduce accuracy
Limited to static ASL alphabet gestures (no dynamic gestures)
Future Improvements
Add dynamic gesture recognition (e.g., words, sentences)
Improve robustness with data augmentation
Deploy as a web/mobile application
Integrate hand tracking (e.g., MediaPipe) for better segmentation
Conclusion

This project demonstrates a complete deep learning pipeline for sign language recognition, combining computer vision and CNN-based classification to enable real-time human-computer interaction.
