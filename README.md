# Face-Controlled-Game-Player
A gesture-recognition-based system where facial movements are translated into keyboard inputs to control gameplay. Utilized real-time face tracking to interact with games like Subway Surfers without using hands.
Face-Controlled Game Player 🎮🧠

A computer vision project that lets users control simple games like Subway Surfers using facial movements instead of traditional keyboard input. This project uses real-time face tracking via a webcam to detect nose position and convert it into directional keyboard commands.

👨‍💻 Features

- Hands-free game control using facial gestures
- Real-time nose tracking using MediaPipe Face Mesh
- Smooth movement with average tracking buffer
- Direction-based key press automation (Up, Down, Left, Right)
- Cooldown system to avoid unintended multiple presses

🛠 Tech Stack

- *Python*  
- *OpenCV* – For camera capture and image processing  
- *MediaPipe* – For facial landmark detection  
- *PyAutoGUI* – For simulating keyboard actions  
- *NumPy* – For smoothing movement data

📸 How It Works

1. Starts webcam and detects the user's face
2. Tracks nose position frame-by-frame
3. Averages recent nose positions to reduce jitter
4. Compares current position with the average to detect movement direction
5. Sends arrow key commands to the system based on facial movement

## 🎯 Game Compatibility

This system is ideal for games that use *arrow keys* to navigate, such as:
- Subway Surfers (via PC emulators)
- Temple Run
- Google Chrome Dino Game

## 🧪 Results & Limitations

- Works best in well-lit environments
- Camera resolution affects tracking accuracy
- Only supports nose-based gesture input
- Might lag slightly due to cooldown setup

## 🚀 Getting Started

### Requirements

- Python 3.x
- OpenCV
- MediaPipe
- PyAutoGUI
- NumPy

### Installation

```bash
pip install opencv-python mediapipe pyautogui numpy
