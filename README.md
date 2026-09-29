# Rep AI

Rep AI is a mobile computer-vision fitness coach that uses a phone camera to analyze exercise movements and track repetitions.

The project explores how pose estimation and movement analysis can be used to provide real-time, exercise-specific feedback.

## Project Overview

Rep AI analyzes human body movement through a phone camera and converts pose information into structured exercise data.

Core pipeline:

**Camera → Pose Estimation → Joint Angles → Movement Smoothing → Rep Detection → Form Analysis**

## Current Implementation

The current system includes:

* Real-time pose estimation using MediaPipe Pose
* Joint-angle extraction from body landmarks
* Temporal smoothing for movement signals
* Exercise-specific repetition detection
* Correct / incorrect form annotation
* Structured workout session capture
* Dataset collection and export

### Supported Exercises

* Squats
* Bicep curls
* Shoulder presses

## Dataset

The project includes a structured exercise dataset collected through the mobile data-collection pipeline.

| Metric | Value |
| --- | --- |
| Files | 79 |
| Sessions | 68 |
| Repetitions | 544 |
| Frames | 27,490 |

The dataset is intended to support future exercise-form classification and real-time coaching research.

## Technology

* **Language:** Kotlin
* **Platform:** Android
* **Camera:** CameraX
* **Computer Vision:** MediaPipe Tasks Vision
* **Pose Analysis:** MediaPipe Pose
* **Model:** Bundled pose model
* **Data:** Structured session and movement data

## System Architecture

```text
Phone Camera
     ↓
CameraX
     ↓
Pose Estimation
     ↓
Body Landmarks
     ↓
Joint-Angle Extraction
     ↓
Temporal Smoothing
     ↓
Exercise-Specific Rep Detection
     ↓
Form Data
     ↓
Future: Real-Time Coaching

```

## Research Direction

The broader objective of Rep AI is to develop a mobile AI fitness coach capable of:

* Detecting exercise-specific form errors
* Providing immediate corrective feedback
* Tracking exercise performance over time
* Supporting voice-based coaching
* Adapting feedback to individual users

These capabilities represent the ongoing research and development direction of the project.

## Demo

[Watch the Rep AI Demo](https://youtu.be/G3zaa_z5-Yo)

**REP-AI Demo — AI Fitness Coach Using Phone Camera**

## Project

Rep AI is developed as a Final Year Project at FAST-NUCES.

**Developer:** Abdul Wahab  
**Degree:** B.S. Cyber Security, FAST-NUCES
