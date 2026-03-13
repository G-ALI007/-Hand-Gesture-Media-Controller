# Hand Gesture Media Controller (Thumbs + Lock Edition) 🖐️📺

A real-time computer vision application that allows you to control your media player (Spotify, YouTube, VLC, etc.) using hand gestures through your webcam. This tool uses **MediaPipe** for hand tracking and **PyAutoGUI** to simulate media key presses.

## ✨ Features
- **Smart Locking System:** Toggle the controller ON/OFF with a "Victory" sign to prevent accidental commands.
- **Continuous Volume Control:** Adjust volume smoothly by holding a Thumb UP or DOWN.
- **Visual Feedback:** High-quality HUD (Heads-Up Display) with a cooldown bar, gesture labels, and a visual skeleton.
- **No Training Required:** Uses a robust rule-based classification logic (no heavy ML models needed for inference).

## 🖐️ Gesture Map
| Gesture | Action |
| :--- | :--- |
| **Victory (2 Fingers)** | 🔓 Toggle Lock ON/OFF |
| **Thumb UP** | 🔊 Volume Up (+1 every second) |
| **Thumb DOWN** | 🔉 Volume Down (-1 every second) |
| **Thumb RIGHT** | ⏭️ Next Track |
| **Thumb LEFT** | ⏮️ Previous Track |
| **Open Palm** | ⏯️ Play / Pause |
| **Fist** | ⏹️ Stop |

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed on your system. You will also need a working webcam.

### Installation
1. Clone this repository or download the source code.
2. Install the required dependencies:
   ```bash
   pip install opencv-python mediapipe pyautogui numpy
Running the Controller
Run the script using the following command:

Bash
python hand_controller.py
⚙️ Configuration
You can tweak the performance in the hand_controller.py file:

COOLDOWN_SECONDS: Adjust the delay between track changes (Default: 1.5s).

VOLUME_INTERVAL: Speed of volume adjustment (Default: 1.0s).

CAMERA_INDEX: Change this if you have multiple webcams (0, 1, etc.).

🛠️ Built With
MediaPipe - For hand landmark detection.

OpenCV - For image processing and UI rendering.

PyAutoGUI - For controlling media keys.

Created with ❤️ for a better media experience.
