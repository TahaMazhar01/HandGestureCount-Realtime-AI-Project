HandCount - Hand Gesture Detection Project
Python
OpenCV
MediaPipe
Overview
HandCount is an open-source computer vision project built with MediaPipe and OpenCV for real-time hand gesture detection and finger counting. It processes video input (e.g., from a webcam) to identify hand landmarks and accurately count raised fingers, making it ideal for gesture-based interfaces, interactive applications, educational demos, or accessibility tools.
Features

Real-Time Detection: Tracks hands and landmarks using MediaPipe's efficient hand model.
Finger Counting: Analyzes fingertip positions relative to joints to count extended fingers.
Video Processing: Handles webcam or file-based input with seamless OpenCV integration.
Customizable: Easily extend for multi-hand support or additional gestures (e.g., thumbs up, victory sign).

Tech Stack

Python (3.7+): Primary language for scripting and logic.
MediaPipe: Hand landmark detection and pose estimation.
OpenCV: Video capture, image processing, and real-time visualization.

Quick Start
Prerequisites

Python 3.7–3.10
A webcam or compatible video source

Installation

Clone the repository:bashgit clone https://github.com/TahaMazhar01/HandCount.git
cd HandCount
Install dependencies:bashpip install -r requirements.txt

Usage

Launch the application:bashpython handcount.py
Position your hand in front of the camera—the finger count will overlay on the video feed in real-time.
Exit with Esc or close the window.

For custom video input, modify handcount.py to load a file via cv2.VideoCapture('path/to/video.mp4').
How It Works

Detection: MediaPipe processes each frame to extract 21 hand landmarks (e.g., fingertips, PIP joints).
Analysis: Custom heuristics compare y-coordinates of fingertips to base joints—fingers above the base are counted as "raised."
Rendering: OpenCV draws landmarks, connections, and the count on the frame for intuitive feedback.

Example output: A bounding box around the hand with numbered fingertips and a large overlay showing "Fingers: 3".
Requirements
See requirements.txt for full list:
textmediapipe>=0.10.0
opencv-python>=4.5.0
numpy>=1.21.0
Roadmap

Support for multiple simultaneous hands.
Expanded gestures (e.g., rock-paper-scissors, sign language basics).
Performance tweaks for mobile/edge devices.
Integration with webcams via browser (using WebRTC).

Contributions to these features are encouraged!
Contributing
Contributions are welcome! To get started:

Fork the repo and create a feature branch (git checkout -b feature/amazing-feature).
Commit your changes (git commit -m 'Add amazing feature').
Push to the branch (git push origin feature/amazing-feature).
Open a Pull Request.

Please adhere to PEP 8 for code style and include tests where possible. Report issues via the Issues tab.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Contact

Author: Taha Mazhar
GitHub: TahaMazhar01
Email: tahamazhar01@gmail.com

Feel free to reach out for questions, collaborations, or feedback. Let's build something awesome together!
