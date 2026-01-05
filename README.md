# YOLOv11 Multi-Image Detection (Google Colab)

This repository provides a simple and reliable script for running **YOLOv11 object detection on multiple unlabeled images** using Google Colab.

The script allows uploading **up to 5 images at once**, performs inference using a trained YOLOv11 model, and displays all detection outputs together.

---

## 📌 Features
- Manual image upload (up to 5 images)
- Supports **unlabeled data**
- YOLOv11 inference using Ultralytics
- Automatic saving of detection outputs
- Grid-based visualization
- Safe handling of "no detection" cases

---

## 📂 File Structure
.
├── multi_image_detection_colab.py
└── README.md

yaml
Copy code

---

## 🚀 How to Use (Google Colab)

1. Upload the script to Google Colab
2. Ensure your YOLOv11 weights are available  
   (e.g. `/content/yolo11n.pt` or `best.pt`)
3. Run the script
4. Upload up to **5 images** when prompted
5. View detection results directly in the notebook

Detection outputs are saved automatically to:
/content/runs/detect/manual_predict_multi/

yaml
Copy code

---

## 📊 Notes for Research & Demos
- This script is intended for **qualitative evaluation**
- Suitable for:
  - Conference demos
  - Failure case visualization
  - Generalization testing on unseen images
- No ground-truth labels are required

---

## ⚠️ Important
- If no detections appear, it indicates model confidence is below the threshold
- This behavior is expected and demonstrates conservative prediction

---

## 📜 License
MIT License