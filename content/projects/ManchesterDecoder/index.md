---
title: 'Real-Time Manchester Decoder via Webcam'
date: '2024-10-15'
summary: 'A Python project that uses OpenCV to read a live webcam feed, detect a Manchester-encoded signal (e.g., a blinking LED), and decode it in real-time using a Finite State Machine (FSM).'
tags:
  - Python
  - Computer Vision
  - OpenCV
  - Real-Time
  - FSM
  - Data Communications
---

This project is a real-time signal processing application that uses a standard webcam to decode a visually transmitted, Manchester-encoded data stream.

Instead of a physical hardware decoder, this project implements the entire decoding logic in software using Python and OpenCV.

### Key Features

* **Real-Time Video Capture:** Utilizes OpenCV (`cv2`) to capture and process a live webcam feed to identify a visual signal (like an LED) in the frames.
* **Software FSM Decoder:** Implements a Python-based Finite State Machine (FSM) to handle the protocol's states (IDLE, DATA, STOP) and accurately sample the signal based on timing.
* **Bitstream Reconstruction:** Successfully decodes the visual signal back into a byte stream, bridging the gap between physical signaling and digital data.

This project demonstrates the ability to use high-level computer vision tools to implement low-level data communication protocols.

* **[View Code on GitHub](https://github.com/Aurivelle/ManchesterCamDecoder)**