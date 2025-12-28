# CS Final Project: Vehicle Detection with YOLOv8

This project demonstrates vehicle detection using the YOLOv8 framework.  
We trained a custom dataset of vehicles and tested the model on video footage to evaluate detection accuracy.

---

## Project Contents
- `best.pt & last.pt` — trained YOLOv8 weights
- `data.yaml` — dataset configuration file
- `report.pdf` — final written report
- `presentation.pdf` — slides for final presentation
- `results` — training logs and prediction results
- `video.mp4` — sample input video used for testing

---

## How to Run
You can reproduce predictions directly from the command line without writing Python scripts:

```bash
1. yolo predict model="best.pt & last.pt" source="video.mp4" show=True save=True
model="best.pt & last.pt" → trained weights
source="video.mp4" → input video file
show=True → display detections live
save=True → save results to runs/detect/

2. Training Summary
Framework: YOLOv8 (Ultralytics)
Model: YOLOv8s
Epochs: 100
Dataset: Custom labeled vehicle dataset
Performance:
Precision: 0.81
Recall: 0.77
mAP@50 (Car class): 0.849

3. Results
The trained model successfully detects cars and other vehicles.
Example detections include 15–27 cars per frame, plus motorcycles, buses, pickups, and trucks.

4. Author: Group 1
Group members: Faizan, Pasha, Eric, Frank.

