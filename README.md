# 🍎 Fruits Detection using YOLOv8 - Computer Vision Project

This project focuses on detecting different types of fruits using the powerful YOLOv8 (You Only Look Once) object detection model. The notebook uses **Ultralytics YOLOv8**, one of the fastest and most accurate object detection architectures available, to build an end-to-end fruit detector.

## 📌 Project Highlights

- ✅ Real-time fruit detection with YOLOv8
- 🖼️ Bounding boxes on apples, bananas, oranges, and more
- 📦 Trained on a custom labeled dataset of fruits
- 🧠 Fine-tuned YOLOv8 with transfer learning
- 📊 Evaluation metrics like mAP (mean Average Precision), Precision, Recall

---

## 📂 Dataset

We used a publicly available dataset containing various images of fruits such as apples, bananas, oranges, etc. The dataset is labeled in **YOLO format** with annotations for object location and class.


---

## ⚙️ Installation & Setup


> Make sure you have Python 3.8+ and PyTorch installed.

### 1. Install YOLOv8 (Ultralytics)

```bash
pip install ultralytics
```

---

## 🚀 How to Run

### Train the YOLOv8 model

```bash
yolo task=detect mode=train model=yolov8n.pt data=fruits.yaml epochs=50 imgsz=640
```

### Evaluate the model

```bash
yolo task=detect mode=val model=runs/detect/train/weights/best.pt data=fruits.yaml
```

### Inference on new images

```bash
yolo task=detect mode=predict model=best.pt source='path_to_image_or_video'
```

---

## 📈 Results

- 🔎 **Precision:** 0.92
- 🔄 **Recall:** 0.89
- 📉 **mAP50:** 0.94
- 📉 **mAP50-95:** 0.86


---

## 📓 Project Notebook

The full code, training pipeline, visualizations, and explanations are available in the Jupyter Notebook:

📘 [`Fruits_Detection_Using_YOLOv8_Computer_Vision_DL.ipynb`](./Fruits_Detection_Using_YOLOv8_Computer_Vision_DL.ipynb)

---

## 📌 Use Cases

- Smart agriculture: Detecting fruit ripeness or type
- Retail inventory and fruit counting
- Quality assurance in packing and distribution

---

## 🙌 Acknowledgements

- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)

---

## 📬 Contact

Created by [Sameh Raouf](https://github.com/Sameh20200218AI)  
If you found this project helpful, feel free to give it a ⭐ and share your feedback!
