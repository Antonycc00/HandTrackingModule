

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

2. Run the main script:
   ```bash
python hand_control.py
Gestures:

Bring your Thumb and Index finger together to decrease volume.

Move them apart to increase volume.

License
MIT License

