# Finals-Smart-Helmet-Detector
# Smart Helmet Detector
*Real-time computer vision system that detects whether construction workers are wearing safety helmets.*

## Team Members
- Erwin Cheng —
-  Koffi Viglo —
-  
## Project Tier
**Tier 2** — Uses object detection (helmet vs no-helmet) and supports a live/demo workflow with evaluation.

---

## 🎯 Problem & Solution
### The Problem
On job sites, missing a helmet can quickly turn into serious injury. Supervisors can’t watch every worker at all times, especially across large areas.

### Our Solution
We built a computer vision detection pipeline that identifies people and classifies whether a helmet is present. When a “no-helmet” case is detected, the system can flag it visually (and can be extended to alerts/logging).

### Impact
Helps safety teams spot issues faster, improves compliance, and reduces reliance on constant manual monitoring.

---

## 🔧 Technical Details
### Approach
- **Task**: Object Detection
- **Model**: YOLOv8 (Ultralytics)
- **Framework**: PyTorch (via Ultralytics)
- **Key Libraries**: ultralytics, opencv-python

### System Architecture
**Input (image/video)** → **Preprocessing** → **YOLOv8 inference** → **Post-processing (confidence/NMS)** → **Bounding boxes + labels + counts**

---

## 📊 Dataset
Source: https://roboflow.com/  
Size: [# images]  
Classes: `helmet`, `no_helmet` (or whatever your dataset uses)  
Split: Train: X / Val: Y / Test: Z  
Preprocessing: [resizing, augmentation, normalization]

---

## 🚀 How to Run
### Install
```bash
pip install -r requirements.txt
