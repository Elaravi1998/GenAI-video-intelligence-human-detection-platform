# 🎥 Video Intelligence & Human Detection Platform

A privacy-conscious computer-vision project for detecting people in video, assigning temporary anonymous tracking IDs, analyzing crowd occupancy, and identifying simple video events using YOLO and OpenCV.

## 🚀 Features

- Human detection using pretrained YOLO
- Video processing with OpenCV
- Anonymous object tracking using IoU
- Real-time-style people counting on sampled frames
- Crowd threshold event detection
- Region of Interest (ROI) entry detection
- Video annotation with bounding boxes
- Occupancy timeline visualization
- CSV and JSON report generation

## 🛠️ Tech Stack

- Python
- YOLO (Ultralytics)
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## 📁 Project Structure

```text
video-intelligence-human-detection-platform/
│
├── video_intelligence_human_detection_platform.ipynb
├── README.md
├── requirements.txt
│
└── outputs/
    ├── annotated_sampled_video.mp4
    ├── detections.csv
    ├── events.csv
    ├── occupancy_timeline.csv
    └── summary.json
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/video-intelligence-human-detection-platform.git

cd video-intelligence-human-detection-platform
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

Windows:

```bash
.venv\Scripts\activate
```

Linux / macOS:

```bash
source .venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

`video_intelligence_human_detection_platform.ipynb`

## 🎬 Input Video Configuration

Place your authorized video file in the project directory and configure:

```python
VIDEO_PATH = "sample_video.mp4"
```

The notebook uses the lightweight YOLO model:

```python
MODEL_NAME = "yolov8n.pt"
```

The model weights are downloaded on first use, unless you configure a local weights file.

## 📊 Detection Configuration

| Parameter | Description |
|---|---|
| VIDEO_PATH | Input video location |
| MODEL_NAME | YOLO model weights |
| CONFIDENCE_THRESHOLD | Detection confidence |
| FRAME_SAMPLE_EVERY | Frame sampling interval |
| MAX_FRAMES | Optional processing limit |
| CROWD_THRESHOLD | Crowd alert threshold |
| ROI | Optional region of interest |

## 🧠 System Workflow

```text
Input Video
     |
     v
OpenCV Video Processing
     |
     v
Frame Sampling
     |
     v
YOLO Human Detection
     |
     v
Anonymous Object Tracking
     |
     v
People Counting
     |
     v
Crowd & ROI Event Detection
     |
     v
Analytics and Visualization
     |
     v
CSV / JSON / Annotated Video
```

## 📈 Output Reports

The notebook generates:

- Annotated video with human detection boxes
- People detection records
- Crowd threshold events
- Region entry events
- Occupancy timeline
- Video analysis summary

## 🔮 Future Enhancements

- ByteTrack and BoT-SORT tracking
- Live webcam human detection
- Real-time crowd monitoring dashboard
- Line-crossing detection
- Dwell-time analytics
- Streamlit web application
- Multiple video processing
- GPU acceleration
- Model performance evaluation
- Secure user authentication and audit logs

## 🔐 Privacy and Responsible Use

This project performs person detection and temporary anonymous tracking only. It does not perform face recognition, identify individuals, or infer sensitive attributes.

Only process footage you are authorized to use. Follow applicable privacy and surveillance requirements, minimize video retention, and restrict access to footage and reports. Alerts are review cues, not definitive safety conclusions.

## 📌 Project Purpose

This project demonstrates practical applications of:

- Computer Vision
- Deep Learning
- YOLO Object Detection
- Video Analytics
- Object Tracking
- AI-Based Event Detection
- Data Visualization

**Note:** This is an educational portfolio prototype, not a production surveillance or emergency-response system.

## 📄 License

Choose and add an appropriate open-source license before publishing.
