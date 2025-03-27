# Hand Sign Recognition Web App

## Overview
This web application uses MediaPipe Hands and JavaScript to perform real-time hand gesture recognition through your computer's webcam. The app can detect four distinct hand gestures: Peace, Thumbs Up, Fist, and Open Palm. Try it here: 

## Features
- Real-time hand gesture detection
- Webcam-based interaction
- Simple, user-friendly interface
- Visual hand landmark tracking
- Four distinct gesture recognitions

## How to Use It
1. Click "Start Camera"
2. Allow webcam access
3. Make hand gestures in front of the camera
4. See real-time gesture detection
5. Press 'Q' or click "Quit" to stop the camera

## Use Cases
- Prototype interfaces for smart home devices
- Augmented reality navigation
- Robotics control systems
- Human-computer interaction research
- Touchless presentation controls

## Libraries and Technologies

### MediaPipe Libraries
- `@mediapipe/camera_utils`: Provides camera utility functions for accessing and managing webcam input
- `@mediapipe/control_utils`: Offers control utilities for MediaPipe applications
- `@mediapipe/drawing_utils`: Helps in drawing hand landmarks and connections on the canvas
- `@mediapipe/hands`: Core library for hand tracking and landmark detection

## How It Works

### Gesture Detection Algorithm
The app uses a sophisticated landmark-based approach to recognize gestures:

1. **Hand Tracking**: MediaPipe detects hand landmarks (21 key points on the hand)
2. **Landmark Analysis**: Compares the positions of fingertips, pip (proximal interphalangeal) joints, and base points
3. **Gesture Conditions**: Checks specific extended/non-extended finger configurations

### Recognized Gestures
- **Peace Sign**: Index and middle fingers extended, others closed
- **Thumbs Up**: Thumb extended, all other fingers closed
- **Fist**: All fingers closed
- **Open Palm**: All fingers fully extended

## Limitations
- Works best with single-hand gestures
- Requires good lighting and clear hand visibility
- Accuracy depends on camera quality and hand positioning

## Future Improvements
- Add more gesture recognitions
- Implement gesture-triggered actions
- Improve detection accuracy
- Add calibration and training features
