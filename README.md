# HandCount - Hand Gesture Detection Project

## Overview
HandCount is a computer vision project that leverages **MediaPipe** and **OpenCV** to detect hand gestures in real-time and count the number of raised fingers. This project is designed for applications like gesture-based interfaces, interactive systems, or educational tools. It processes video input (e.g., from a webcam) to identify hand landmarks and determine the count of extended fingers with high accuracy.

## Features
- Real-time hand detection and tracking using MediaPipe's hand landmark model.
- Finger counting logic based on hand landmark coordinates.
- Lightweight and easy-to-use implementation with OpenCV for video processing.
- Customizable for different gesture recognition tasks.

## Technologies Used
- **Python**: Core programming language.
- **MediaPipe**: For hand detection and landmark extraction.
- **OpenCV**: For video capture, processing, and visualization.

## Installation
Clone the repository:
   ```bash
   git clone https://github.com/Sripadh-Sujith/Realtime_handcount.git
   cd HandCount
```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure you have a working webcam or video input source.

## Usage
1. Run the main script:
   ```bash
   python handcount.py
   ```
2. Point your webcam at your hand, and the program will display the number of raised fingers in real-time.
3. Press `q` to exit the application.

## How It Works
- **Hand Detection**: MediaPipe's pre-trained model detects hand landmarks (e.g., fingertips, joints) from the video feed.
- **Finger Counting**: Custom logic analyzes the y-coordinates of fingertips relative to other landmarks to determine which fingers are raised.
- **Visualization**: OpenCV overlays the finger count and hand landmarks on the video feed.

## Requirements
- Python 3.7-3.10
- Libraries: `mediapipe`, `opencv-python` (listed in `requirements.txt`)

## Future Improvements
- Add support for multiple hands.
- Implement additional gesture recognition (e.g., thumbs up, peace sign).
- Optimize for lower-end devices.

## Contributing
Feel free to fork this repository, submit issues, or create pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

##THANK YOU! ❤



