# 👁️ Real-Time Eye Tracking with Gaze Detection

This project is a simple real-time eye-tracking system built using Python, OpenCV, and Mediapipe. It detects the user's gaze direction (left, center, or right) by analyzing both iris positions and displays visual feedback.

---

## 🚀 Features

- Real-time webcam-based eye tracking
- Tracks both eyes using Mediapipe Face Mesh
- Detects if the user is looking left, right, or center
- Visual debug overlay: iris and eye corner markers
- Potential use case: attention tracking, HCI, screen monitoring

---


## 🛠️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/eye-tracking-prototype.git
cd eye-tracking-prototype
```

### 2. Install Required Packages
Make sure you have Python 3.7 or later installed.
#### Option A: if you have requirements.txt
```bash
pip install -r requirements.txt
```
#### Option B: Install manually
```bash
pip install opencv-python mediapipe numpy
```

---

## ▶️ How to Run
Run the main script with:
```bash
python main.py
```
press Q to quit the application window

---

## 📁 Project Structure
```perl
eye-tracking-prototype/
├── main.py             # Main script for gaze detection
├── requirements.txt    # Dependency file
├── .gitignore          # Files/folders to be excluded from Git tracking
└── README.md           # This file
```

---

## Gaze Logic
This script calculates the relative position of the iris between the two eye corners to determine gaze direction. It averages results from both eyes for smoother classification.
| Gaze Ratio | Interpretation |
| ---------- | -------------- |
| < 0.35     | Looking LEFT   |
| 0.35–0.65  | Looking CENTER |
| > 0.65     | Looking RIGHT  |

---

## 🙋‍♂️ Author
### Sharavanan Mathivanan
#### GitHub: https://github.com/DiamondDolby
#### LinkedIn: https://www.linkedin.com/in/sharavanan-mathivanan/
