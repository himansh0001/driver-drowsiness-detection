# Driver Drowsiness Detection System

This project implements a **Driver Drowsiness Detection System** using **OpenCV**, **Dlib**, and **NumPy**. It monitors a driver's eye blinks and detects drowsiness or sleepiness in real-time by analyzing facial landmarks.

---

## Features

- **Real-Time Eye Blink Detection**: Monitors both eyes using facial landmarks.
- **Drowsiness Detection**: Detects three states - **Active**, **Drowsy**, and **Sleeping**.
- **Visual Indicators**: Displays a bounding box around the face and eye landmarks, and shows the current status (Active, Drowsy, or Sleeping) on the frame.

---

## Prerequisites

Ensure the following are installed:

1. **Python**: Version 3.8 or higher.
2. **Dependencies**:
   - OpenCV
   - NumPy
   - Dlib
   - imutils

3. **Dlib Pre-Trained Model**: Download the `shape_predictor_68_face_landmarks.dat` file from [Dlib's official website](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) and place it in the project directory.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/himansh0001/driver-drowsiness-detection.git
   cd driver-drowsiness-detection
2. Install dependencies:

bash
Copy code
pip install opencv-python numpy dlib imutils

3. Place the shape_predictor_68_face_landmarks.dat file in the project directory.

#Usage
Run the script:

bash
Copy code
python drowsiness_detection.py
The system will start accessing your webcam and detecting facial landmarks. It will classify the driver's state as:

Active :)
Drowsy !
SLEEPING !!!
Press Esc to exit the program.

## Code Overview
# Core Functions
1. compute(ptA, ptB): Calculates Euclidean distance between two points.
2. blinked(a, b, c, d, e, f): Determines if the eye is open, partially closed, or fully closed based on the Eye Aspect Ratio (EAR).
# Main Workflow
1. Capture Frames: Uses OpenCV to capture frames from the webcam.
2. Face Detection: Detects faces using Dlib's frontal face detector.
3. Facial Landmark Detection: Identifies 68 facial landmarks, focusing on eye landmarks.
4. Eye Blink Analysis: Computes the EAR to classify blink states.
5. Status Monitoring: Updates the driver's status (Active, Drowsy, or Sleeping) based on the blink analysis.
## Screenshots
Real-Time Detection
Coming soon.

## Acknowledgments
1. Dlib for providing the pre-trained facial landmark model.
2. OpenCV for real-time image processing.
3. NumPy for efficient numerical calculations.


# Author
Himansh
https://github.com/himansh0001

