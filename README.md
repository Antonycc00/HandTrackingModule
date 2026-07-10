
<img width="642" height="512" alt="handtracking" src="https://github.com/user-attachments/assets/11b7708a-0016-41a0-8cb8-571374674e96" />

Hand Tracking & Gesture Control
A Python-based computer vision project that detects hand landmarks in real-time and uses gestures to interact with the system (e.g., controlling system volume).

Features
Real-time Hand Detection: Accurate tracking of 21 hand landmarks using MediaPipe.

Gesture Logic: Calculation of distances between fingertips (e.g., thumb and index) to trigger actions.

System Integration: Dynamic control of system volume using the ctypes library to interface with Windows audio endpoints.

Prerequisites
Before running the script, ensure you have the following installed:

Bash
pip install opencv-python mediapipe
How It Works
OpenCV (cv2): Captures video frames from your webcam.

MediaPipe (mp): Processes frames to identify hand structures and finger positions.

Math: Calculates the Euclidean distance between specific landmarks to determine gesture intensity.

Ctypes: Maps the calculated distance to the master volume levels of your operating system.

python hand_control.py
Gestures:

Bring your Thumb and Index finger together to decrease volume.

Move them apart to increase volume.

License
MIT License

