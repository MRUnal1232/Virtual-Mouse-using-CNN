# Virtual Mouse Control Using Hand Gestures

A computer vision-based project that allows you to control your computer's mouse using hand gestures captured through your webcam. This project utilizes MediaPipe for hand tracking and implements various gesture controls for mouse operations.

## Features

- **Mouse Movement**: Control cursor movement using your index finger
- **Click Operations**:
  - Left Click: Perform by specific hand gesture
  - Right Click: Dedicated gesture for right-click operation
  - Double Click: Special gesture for double-clicking
- **Scrolling**:
  - Scroll Up: Gesture control for scrolling up
  - Scroll Down: Gesture control for scrolling down
- **Screenshot**: Take screenshots with a specific hand gesture
- **Real-time Hand Tracking**: Visual feedback with hand landmark detection

## Requirements

- Python 3.x
- OpenCV (cv2)
- MediaPipe
- PyAutoGUI
- Pynput

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd virtual_mouse
```

2. Install the required packages:
```bash
pip install opencv-python mediapipe pyautogui pynput
```

## Usage

1. Run the main script:
```bash
python main.py
```

2. Position your hand in front of the webcam

3. Use the following gestures:
   - Move cursor: Point with your index finger
   - Left click: Make a specific gesture with index finger while maintaining distance from thumb
   - Right click: Similar gesture with middle finger
   - Double click: Specific gesture with both index and middle fingers
   - Scroll up/down: Use ring and pinky finger gestures
   - Screenshot: Special gesture with minimal thumb-index distance

4. Press 'q' to quit the application

## How It Works

The application uses MediaPipe's hand tracking to detect hand landmarks in real-time through your webcam. These landmarks are then used to:
- Track the position of your index finger for mouse movement
- Calculate angles between fingers for gesture recognition
- Determine distances between specific landmarks for different mouse operations

## Project Structure

- `main.py`: Contains the core functionality and gesture detection logic
- `util.py`: Utility functions for angle and distance calculations

## Notes

- Ensure good lighting conditions for optimal hand detection
- Keep your hand within the camera's field of view
- Screenshots are saved in the project directory with random numbers as filenames

## Contributing

Feel free to fork the project and submit pull requests for any improvements.

## License

This project is open source and available under the MIT License.