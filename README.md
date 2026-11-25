# YOLOv8 Object Detection

Real-time object detection using YOLOv8 deep learning models integrated with a Flask web application. Captures live webcam footage or uses static images to detect and label objects.

---

## Problem Statement

Real-time object detection requires an efficient, deployable system that can process webcam feeds and static images with minimal latency.

## Objectives

- Implement real-time object detection from webcam
- Support image-based detection
- Provide a Flask web interface for live feed
- Use pre-trained YOLOv8 models (nano, medium)

## Key Features

- **Real-Time Webcam Detection** — Flask MJPEG streaming with YOLOv8n
- **Image-Based Detection** — YOLOv8m for static image analysis
- **Flask Web Interface** — browser-based live feed viewer
- **Frame Rate Limiting** — ~16 FPS for smooth streaming
- **Confidence Thresholding** — 0.5 minimum confidence

## Technologies Used

| Component | Technology |
|-----------|-----------|
| Backend | Python (Flask) |
| Object Detection | Ultralytics (YOLOv8) |
| Computer Vision | OpenCV |
| Visualization | Matplotlib |

## Project Structure

```
yolov8-object-detection/
├── app.py              # Flask web app for live webcam detection
├── model.py            # Script for image-based object detection
├── templates/
│   └── index.html      # Web UI for live feed
├── static/             # Sample images
├── runs/               # Detection output
└── README.md
```

## Installation and Setup

### Prerequisites
- Python 3.8+
- pip
- Webcam (for live detection)

### Setup
```bash
pip install -r requirements.txt
python app.py
```

Application runs at `http://localhost:5000`.

### Image Detection
```bash
python model.py
```

## Limitations

- Requires webcam for live detection
- Model files (yolov8n.pt, yolov8m.pt) must be downloaded separately
- No error handling for missing camera or model files

## Author and Contact Information

**SAMALA RAKSHITH BABU**

- Email: samalarakshithbabu7@gmail.com
- LinkedIn: https://www.linkedin.com/in/samala-rakshith-babu-9374ab281/
- GitHub: https://github.com/samalarakshithbabu

## License

MIT License (badge-confirmed; file path not verified).