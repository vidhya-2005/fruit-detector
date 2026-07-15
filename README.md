# Fruit Object Detection Dataset (YOLO Format)

## 📌 Project Objective
This repository contains a high-quality, structurally verified image dataset built for object detection models. The dataset features manually labeled bounding boxes surrounding five fruit categories: Apples, Bananas, Oranges, Mangoes, and Grapes. 

## 🛠️ Tools & Technologies
* **Data Retrieval:** `kagglehub` API via Python
* **Dataset Source:** Kaggle Fruits Dataset (`moltean/fruits`)
* **Annotation Suite:** Label Studio
* **Validation & Metrics:** Python 3.12 & Google Colab

---

## 🗂️ Dataset Architecture
The dataset consists of a clean sample of 150 images. Images were downsampled to exactly 30 pictures per class to maintain balance, then processed into standard YOLO format (`.txt` files containing normalized coordinates: `[class_id x_center y_center width height]`).

```text
├── dataset/
│   ├── images/   # Contains 150 raw fruit photographs (.jpg)
│   └── labels/   # Contains 150 YOLO bounding box annotation files (.txt)
├── notebooks/
│   └── fruit_dataset_project.ipynb  # The data pipeline & validation script
└── README.md
