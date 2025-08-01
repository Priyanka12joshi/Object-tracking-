# 🎯 Object Tracking in Computer Vision

A comparative project demonstrating the core differences between **Object Detection** and **Object Tracking** using real-time video inputs and deep learning models such as YOLOv8 and DeepSORT. This repo is ideal for learning, benchmarking, and visualizing both techniques side-by-side.

---

## 📑 Table of Contents

* [Overview](#-overview)
* [Key Concepts](#-key-concepts)
* [Demo Video](#-demo-video)
* [Tech Stack](#-tech-stack)
* [Setup & Installation](#-setup--installation)
* [How to Use](#-how-to-use)
* [Examples](#-examples)
* [Results](#-results)
* [License](#-license)
* [Author](#-author)

---

## 📌 Overview

This repository compares two fundamental computer vision tasks:

* **Object Detection** – Identifying and locating objects (e.g., YOLOv8)
* **Object Tracking** – Assigning IDs and tracking object movements over time (e.g., DeepSORT)

> This project visualizes both methods using video input and provides scripts and examples to learn the differences clearly.

---

## 📘 Key Concepts

| Feature    | Object Detection               | Object Tracking                 |
| ---------- | ------------------------------ | ------------------------------- |
| Purpose    | Find and classify objects      | Maintain identity across frames |
| Output     | Boxes + labels                 | Boxes + labels + unique ID      |
| Tools Used | YOLOv8                         | DeepSORT, ByteTrack             |
| Use Cases  | Image classification, counting | Surveillance, motion analysis   |

---

## 🎥 Demo Video

[https://user-images.githubusercontent.com/demo-path/preview.gif](https://user-images.githubusercontent.com/demo-path/preview.gif)

---

## 🛠️ Tech Stack

* 🧠 YOLOv8 (via [Ultralytics](https://github.com/ultralytics/ultralytics))
* 🚀 DeepSORT for tracking
* 🐍 Python 3.9+
* 📷 OpenCV for video frame handling
* 🖥️ Streamlit (optional live demo)
* 📁 Pre-recorded or webcam input

---

## 🔧 Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/object-detection-vs-tracking.git
cd object-detection-vs-tracking
```

### 2. Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

> Requirements include `ultralytics`, `deep_sort_realtime`, `opencv-python`, `streamlit`, etc.

---

## 🚀 How to Use

### ▶️ Run Object Detection (YOLOv8)

```bash
python detect_yolo.py --source video.mp4  # or 0 for webcam
```

### 🎯 Run Object Tracking (YOLO + DeepSORT)

```bash
python track_objects.py --source video.mp4
```

### 📡 Run Streamlit Dashboard (Optional)

```bash
streamlit run app.py
```

---

## 🖼️ Examples

* `output/detection_output.mp4` – Video with detected objects
* `output/tracking_output.mp4` – Same video with tracking enabled

---

## 📊 Results

| Model           | FPS | Accuracy | Note                       |
| --------------- | --- | -------- | -------------------------- |
| YOLOv8          | 30+ | High     | Real-time detection only   |
| YOLO + DeepSORT | 20+ | High     | Real-time with ID tracking |

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Author

* **Priyanka Joshi**
  📧 [priyanka@example.com](mailto:priyankajoshi2300@gmail.com)
  🔗 [LinkedIn]linkedin.com/in/priyanka-joshi450643247/)

---

## 🌟 Star the Repo

If you found this helpful, give it a ⭐ and consider contributing or raising an issue!


