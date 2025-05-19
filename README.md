# 🔥 Fire and Smoke Detection using OpenCV

This project demonstrates a basic **real-time fire and smoke detection system** using color segmentation in HSV color space with Python and OpenCV.

---

## 📌 Overview

The system analyzes video frames from a webcam (or video file) to detect:
- **Fire** based on orange-yellow color range.
- **Smoke** based on light gray color range.

Alerts are displayed on the screen when fire or smoke is detected.

---

## 🧠 How It Works

1. **Convert Frame to HSV**: HSV color space is more effective for color detection.
2. **Define Color Ranges**:
   - Fire: Orange-yellow hues.
   - Smoke: Light gray tones.
3. **Create Binary Masks**: Use `cv2.inRange()` to segment pixels in defined color ranges.
4. **Bitwise AND**: Extract potential fire/smoke regions.
5. **Pixel Count Threshold**: Detect presence if a minimum number of pixels match.
6. **Display Alerts**: Overlay alert text on video frame if detection occurs.

---

## 🛠️ Requirements

Install required packages:

```bash
pip install opencv-python numpy
