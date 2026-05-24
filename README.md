# Drowsy Driver Detection System

A real-time AI-powered driver drowsiness detection system developed using Computer Vision and Deep Learning techniques to reduce road accidents caused by driver fatigue.

## Overview

Driver drowsiness is one of the major causes of road accidents worldwide. This project detects driver fatigue by monitoring eye states in real time using a webcam and alerts the driver with an alarm when drowsiness is detected.

The system uses:
- Computer Vision for face and eye detection
- Convolutional Neural Networks (CNN) for eye state classification
- Transfer Learning with InceptionV3
- OpenCV for real-time video processing

## Features

- Real-time drowsiness detection
- Eye state classification (Open / Closed)
- Alarm alert when drowsiness is detected
- Works in low-light conditions
- Supports users wearing glasses
- Webcam-based implementation
- Deep learning based prediction model

## Technologies Used

- Python
- OpenCV
- TensorFlow
- Keras
- NumPy
- Flask
- HTML
- CSS
- JavaScript
- Jupyter Notebook

## Dataset

The project uses the MRL Eye Dataset containing:
- 84,000+ eye images
- Images of 37 individuals
- Open and closed eye samples
- Images with glasses
- Different lighting conditions

Dataset features include:
- Eye state
- Gender
- Glasses/no glasses
- Reflections
- Lighting conditions

## Project Workflow

### Training Phase
1. Data Collection
2. Data Preprocessing
3. Feature Extraction
4. Transfer Learning
5. CNN Model Training
6. Model Validation

### Testing Phase
1. Webcam captures real-time video
2. Face detection using Viola-Jones Algorithm
3. Eye region extraction using Haar Cascade
4. Eye classification using CNN
5. Drowsiness prediction
6. Alarm activation

## Algorithms Used

### Convolutional Neural Network (CNN)
Used for classifying eye states as:
- Open
- Closed

### Viola-Jones Algorithm
Used for:
- Real-time face detection
- Eye region localization

### Haar Cascade Features
Used for:
- Eye feature extraction
- Face region detection

### Transfer Learning
The project experimented with:
- VGG19
- ResNet50
- InceptionV3

InceptionV3 provided the best performance and was selected for final implementation.

## Model Performance

| Metric | Value |
|--------|--------|
| Training Accuracy | 94.7% |
| Validation Accuracy | 92.6% |
| Training Loss | 16.16% |
| Validation Loss | 13.98% |

## System Architecture

```text
Webcam Input
      ↓
Image Preprocessing
      ↓
Face Detection
      ↓
Eye Detection
      ↓
CNN Classification
      ↓
Drowsiness Detection
      ↓
Alarm Alert