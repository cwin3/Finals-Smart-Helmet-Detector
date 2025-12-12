
# Smart Helmet Detector
Real-time computer vision system that detects whether construction workers are wearing safety helmets.

## Team Members
- Erwin Cheng
- Koffi Viglo

## Project Tier
**Tier 2 – Object Detection (YOLOv8)**

## Problem & Solution
Construction sites are dangerous environments where missing safety gear can lead to serious injuries.
This project uses computer vision to automatically detect whether a worker is wearing a helmet,
helping supervisors quickly identify safety risks.

## Technical Overview
- Task: Object Detection
- Model: YOLOv8
- Framework: PyTorch (Ultralytics)
- Input: Images / Video
- Output: Bounding boxes labeled helmet / no-helmet

Pipeline:
Input → Preprocessing → YOLOv8 Inference → Post-processing → Visualization

## Dataset
- Source: https://roboflow.com/
- Classes: helmet, no-helmet
- Split: Train / Validation / Test
- Augmentation: resizing, flipping, normalization

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/04_demo.ipynb
```

## Results
Metrics will be reported after evaluation:
- Precision:
- Recall:
- mAP@0.5:

## Demo
(Add video or screenshots)

## AI Usage
See docs/AI_usage_log.md

## References
- https://docs.ultralytics.com
