# 🚗 License Plate Detection System

A computer vision-based License Plate Detection system that detects vehicles, localizes license plates, and extracts license numbers from video streams in real time.

This project leverages YOLOv8 object detection, multi-object tracking, and OCR to accurately identify and track vehicles while reading license plate information, enabling applications in smart parking, traffic monitoring, and security systems.

## 🚀 Features

### Vehicle Detection & Tracking
- Detects vehicles in video streams using YOLOv8.
- Tracks multiple vehicles across frames using the SORT tracking algorithm.
- Assigns unique IDs to detected vehicles.

### License Plate Detection
- Identifies and localizes license plates using a custom-trained YOLOv8 model.
- Associates detected license plates with tracked vehicles.

### OCR-Based Plate Recognition
- Extracts license plate text using EasyOCR.
- Applies character correction and formatting rules to improve accuracy.
- Filters and validates license plate formats.

### Video Annotation & Visualization
- Draws bounding boxes around vehicles and license plates.
- Displays recognized license numbers directly on video frames.
- Generates annotated output videos with tracking information.

### Data Logging
- Stores detection and recognition results in CSV format.
- Records vehicle IDs, bounding boxes, confidence scores, and license plate numbers.

## 🛠️ Tech Stack

- Python 3.11+
- YOLOv8 (Ultralytics)
- OpenCV
- EasyOCR
- NumPy
- Pandas
- SORT Tracking Algorithm
- Computer Vision & Deep Learning

## 📂 Dataset and Pre-trained Models

A custom dataset was used to train the license plate detection model using YOLOv8. The project utilizes:

- YOLOv8 Nano for vehicle detection (COCO dataset)
- Custom-trained YOLOv8 model for license plate localization
- EasyOCR for license plate text extraction

The trained weights and dataset can be included separately for inference and retraining purposes.

After downloading the required model weights, place them in the project directory before running the application.
