---
title: 'CAPTCHA Generator'
date: '2025-07-01' 
summary: 'A Machine Learning project utilizing a VGG-based Convolutional Neural Network (CNN) in PyTorch to solve distorted text-based CAPTCHAs.'
tags:
  - Deep Learning
  - PyTorch
  - CNN
  - Computer Vision
  - Python
---

This project is a Deep Learning model designed to solve common text-based CAPTCHAs, built as a final project for a Machine Learning course.

The core of the project is a VGG-based Convolutional Neural Network (CNN) implemented in PyTorch, which is trained to recognize individual characters from heavily distorted and perturbed CAPTCHA images.

### Key Features

* **Model Implementation:** Built and trained a VGG-based CNN model using PyTorch for character-level image recognition.
* **Data Pipeline:** Includes scripts for synthetic CAPTCHA data generation, image augmentation, and character-level perturbation (`perturber.py`) to create a robust training dataset.
* **Web Demo:** Features a simple web interface (`app.py`) to demonstrate the trained model's real-time solving capabilities.
* **Academic Analysis:** Supported by a full academic report and presentation slides detailing the methodology and evaluation metrics.

You can view the complete source code and academic papers from the links below:

* **[View Code on GitHub](https://github.com/Aurivelle/CAPTCHAPlatform)**
* **[Read the Full Report (PDF)](report.pdf)**
* **[View Presentation (PDF)](Slide.pdf)**