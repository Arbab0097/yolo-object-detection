# yolo-object-detection
Custom YOLO model trained on my own dataset for object detection practice
# YOLOv11 — Detection & Segmentation

This repository contains my assignment: training and inference for object detection/segmentation using Ultralytics YOLO (custom dataset).

## Files included
- `notebooks/YOLO_Detection_and_Segmentation.ipynb` — main Colab notebook (how I trained / ran inference).
- `models/best.pt` — trained model checkpoint (best).
- `data/data.yaml` — dataset config (train/val/test paths and class names).
- `dataset/Task11.v1i.yolov11.zip` — Roboflow dataset export (optional).
- `videos/input_video.mp4` — sample input video.
- `videos/segmented_output_video1.mp4` — sample output from inference.
- `results/results.png` — training loss/metrics plot.

## How to run (quick)
1. Open the notebook in Colab:  
   `https://colab.research.google.com/github/<YOUR_USERNAME>/<REPO>/blob/main/notebooks/YOLO_Detection_and_Segmentation.ipynb`  
2. Install requirements: `pip install -r requirements.txt` (or run the notebook cells that install dependencies).  
3. Load the model: `from ultralytics import YOLO; model = YOLO('models/best.pt')`  
4. Run inference on a video: call the notebook cell that runs `infer_video('videos/input_video.mp4','videos/segmented_output_video1.mp4')`.

## Requirements
- ultralytics
- opencv-python
- torch
- torchvision
- numpy

(See `requirements.txt` for exact versions.)

## Notes
- I have included a small dataset export (Roboflow) and a sample video. If any file is missing, please contact me.
