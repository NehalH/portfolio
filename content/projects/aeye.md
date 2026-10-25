---
title: "A-EYE - SMART VISUAL ASSISTANCE SYSTEM"
description: "Real-time smart glasses system connected to a companion mobile application for assisting the visually impaired with currency classification and text recognition. | Tech Stack: Flutter, Embedded C, Python, TensorFlow, ESP32"
#dateString: 
draft: false
tags: ["Flutter", "Embedded C", "Python", "TensorFlow", "ESP32", "Computer Vision", "Machine Learning", "Mobile Application Development"]
showToc: false
weight: 90
--- 
### [Currency Classifier Model on GitHub](https://github.com/NehalH/RupeeClassifier_MobileNet)

## Overview

**A-EYE** is an assistive wearable technology system engineered to empower visually impaired individuals with greater environmental awareness and independence. The system connects custom-built **smart glasses** equipped with a camera to an intuitive **companion mobile application**, delivering real-time currency denomination identification, optical character recognition (OCR), and audio feedback.

## Key System Components

### Smart Glasses & Edge Hardware
- Built around the **ESP32** microcontroller and embedded camera module, programmed in **Embedded C**.
- Captures image frames upon user prompt and streams them efficiently over low-latency wireless communication to the companion smartphone.
- Designed with low power consumption and compact ergonomics for comfortable daily wear.

### Companion Mobile Application
- Developed with **Flutter** to deliver a responsive, accessible cross-platform mobile experience.
- Incorporates accessible voice controls, touch gestures, and instant text-to-speech audio narration to communicate findings back to the user seamlessly.
- Handles edge image preprocessing and runs offline machine learning inference.

### Deep Learning & Computer Vision
- **Currency Recognition**: Trained a lightweight **MobileNet** Convolutional Neural Network (CNN) specifically tailored to classify Indian rupee denominations across diverse lighting conditions, backgrounds, angles, and folding states.
- Quantized and converted the deep learning model to **TensorFlow Lite (TFLite)** to achieve sub-second, on-device inference without requiring active internet connectivity.
- **Text Recognition (OCR)**: Integrated text extraction and parsing pipelines to identify and read street signs, documents, and product packaging aloud.

## Tech Stack

- **Mobile Application**: Flutter, Dart
- **Hardware & Firmware**: ESP32, Embedded C
- **Machine Learning**: Python, TensorFlow, TensorFlow Lite, MobileNet CNN, OpenCV
