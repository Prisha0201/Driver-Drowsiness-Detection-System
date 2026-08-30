# Driver Drowsiness Detection System

A real-time computer vision system that detects driver drowsiness using a webcam and facial landmarks. It analyzes the driver's eyes and classifies their state as **Active, Drowsy, or Sleeping**.

## Features

- Real-time webcam monitoring
- Face detection using **dlib**
- 68-point facial landmark detection
- Eye Aspect Ratio (EAR)-based eye-state detection
- Detects **Active, Drowsy, and Sleeping** states
- Displays facial landmarks and status on the video feed

## Technologies

- **Python**
- **OpenCV**
- **dlib**
- **NumPy**
- **imutils**

## How It Works

```text
Webcam → Face Detection → Facial Landmarks
       → Eye Landmark Extraction
       → Eye Ratio Calculation
       → Active / Drowsy / Sleeping
```

The system uses the 68-point facial landmark model to track both eyes and calculates an eye ratio to determine whether the eyes are open, partially closed, or closed.

## Installation

```bash
pip install opencv-python numpy dlib imutils
```

Download and place:

```text
shape_predictor_68_face_landmarks.dat
```

in the project directory.

## Run

```bash
python drowniness.py
```

Press **ESC** to exit.

## Project Structure

```text
Driver-Drowsiness-Detection/
├── drowniness.py
├── shape_predictor_68_face_landmarks.dat
└── README.md
```
