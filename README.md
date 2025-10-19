# 🧠 Celebrity Face Detection using YOLOv8

This project focuses on detecting **celebrity faces** using **YOLOv8 (You Only Look Once, version 8)** — a state-of-the-art object detection model.  
It covers both **model training** and **testing** on single and collage images, with optional face recognition using **DeepFace**.

---

## 🚀 Project Overview

The project is divided into two main notebooks:

### 🧩 1. `main_code.ipynb`
This notebook handles **training, testing, validating and demo** the YOLOv8 model.

#### 🛠️ Steps Performed
- Installed required dependencies and mounted Google Drive.
- Loaded and prepared the **celebrity face dataset**.
- Configured YOLOv8 model parameters using a custom YAML file.
- Trained the YOLOv8 model for **face detection**.
- Evaluated performance on validation/test data.
- Visualized predictions on sample images.
- Saved trained model weights for future use.
- Detected and recognized faces in:
  - Individual test images.
  - **collage images** (to test detection on multiple faces).
- Integrated **DeepFace** for celebrity recognition.
- Applied image enhancements (brightness, rotation, contrast) for improved results.
- Displayed detection outputs with bounding boxes and labels.
- Implemented a **Gradio interface** for easy testing.

✅ **Outcome:** A trained YOLOv8 model capable of detecting celebrity faces with high accuracy.

---

## ⚙️ YOLOv8 Architecture — How It Works

**YOLO (You Only Look Once)** is a real-time object detection algorithm that views detection as a single regression problem — directly predicting bounding boxes and class probabilities from an image in one pass.

### 🧩 Architecture Components
1. **Input Layer:** Resizes and normalizes images.  
2. **Backbone (CSPDarknet):** Extracts deep image features.  
3. **Neck (PANet):** Merges multi-scale feature maps for better context.  
4. **Head:** Predicts bounding boxes, objectness scores, and class probabilities.  
5. **Output:** Detects faces with bounding boxes and confidence levels.

### 🚀 What Makes YOLOv8 Better
- **Anchor-free detection** for faster training and inference.  
- **Improved backbone** and **dynamic shape input support**.  
- Handles **detection, segmentation, classification, and pose estimation**.  
- Optimized for **real-time applications**.

---

## 🧰 Libraries & Tools Used

| Library | Purpose |
|----------|----------|
| `ultralytics` | YOLOv8 model training and inference |
| `DeepFace` | Celebrity recognition and face verification |
| `MTCNN` | Face landmark detection |
| `OpenCV`, `PIL` | Image preprocessing and augmentation |
| `Gradio` | Interactive web app for model testing |
| `scikit-learn`, `pandas`, `numpy` | Data processing and evaluation |
| `Google Colab`, `Drive` | Model training and storage |

---

## 📊 Results

- Trained YOLOv8 model accurately detects celebrity faces.  
- Integration with DeepFace improves recognition precision.  
- Works effectively on both **single** and **multi-face (collage)** images.  
- Can be extended for **real-time face detection** in videos or webcams.

---


