# YOLO Real-Time Object Detection

This project implements real-time object detection on **images**, **videos**, and **webcams** using the **YOLO (You Only Look Once)** algorithm. YOLO is a fast and accurate deep learning-based object detection method, capable of processing real-time streams with high performance.

The implementation is done in **Python** using **OpenCV** and pre-trained YOLOv3 weights. YOLOv3 was introduced in the research paper [YOLOv3: An Incremental Improvement](https://pjreddie.com/media/files/papers/YOLOv3.pdf) by Joseph Redmon and Ali Farhadi.

> 🔗 Project GitHub Repository: [YOLO Real-Time Object Detection](https://github.com/ShyamSanjeyS/YOLO-OBJECT-DETECTION/tree/main/YOLO-Real-Time-Object-Detection)

The model is trained on the **COCO dataset**, which includes 80 common object categories.

---

## Features

- Real-time object detection via **webcam**, **video files**, or **images**
- Uses **YOLOv3** and **YOLOv3-tiny**
- Built with **OpenCV DNN module** (no need for Darknet)
- Lightweight and easy to run locally

---

## Requirements

- Python 3.6+
- OpenCV 4.2+
- NumPy

Install dependencies:

```bash
pip install numpy opencv-python
```

---

## Setup

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/ShyamSanjeyS/YOLO-OBJECT-DETECTION.git
   cd YOLO-OBJECT-DETECTION/YOLO-Real-Time-Object-Detection
   ```

2. **Download YOLOv3 Weights and Configs**:

   - [Download yolov3.weights](https://pjreddie.com/media/files/yolov3.weights)
   - [Download yolov3-tiny.weights](https://pjreddie.com/media/files/yolov3-tiny.weights)
   - [Download yolov3.cfg](https://github.com/pjreddie/darknet/blob/master/cfg/yolov3.cfg)
   - [Download yolov3-tiny.cfg](https://github.com/pjreddie/darknet/blob/master/cfg/yolov3-tiny.cfg)

   Place the files in the appropriate folders:
   - `weights/` for weights files
   - `cfg/` for config files

---

## How to Use

Run the following commands based on your input type:

- **UK Real-Time Road Detection** (sample video):

  ```bash
  python real_time_yolo_detector1.py
  ```

- **USA Real-Time Road Detection** (sample video):

  ```bash
  python real_time_yolo_detector2.py
  ```

- **Webcam Detection**:

  ```bash
  python real_time_yolo_webcam.py
  ```

Ensure your weights, config, and class files are properly placed and the paths are correctly set in the scripts.

---

## Notes

- You can customize the scripts to use your own videos or images.
- This project runs well on CPU; GPU support can further speed up inference.
- You can switch between YOLOv3 and YOLOv3-tiny by updating the config and weights paths.

---

## License

This project is licensed under the MIT License.
