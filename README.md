# Towards-an-Optimization-Driven-Deep-Learning-Framework-for-Multi-class-Brain-Tumor-Detection-in-MRI

# Advanced-Deep-Learning-Based-Automated-Weld-Quality-and-Defect-Detection-for-Industrial-Applications

### A Deep Learning Framework for Real-Time Visual Analysis

### Overview

This repository contains the implementation of a customized YOLOv12-based deep learning model for automated weld quality and defect detection. The system is designed to assist in industrial inspection by automatically detecting Good Welds, Bad Welds, and Defects from weld surface images in real time.

Manual weld inspection is time-consuming and subjective, often leading to inconsistencies in quality assessment.
This project introduces a advanced computer vision-based inspection framework that leverages YOLOv12, the latest model in the YOLO family(as of 2025), for multi-scale weld detection and classification. The model was trained on a curated weld dataset, consisting of 2,151 labeled images (5,937 total annotations).
It achieves strong detection accuracy and generalization across different weld textures, lighting conditions, and defect types.

### Model Architecture

The customized YOLOv12 model consists of three main components:
- Backbone – Modified CSPDarknet with Cross-Stage Partial (CSP) connections and dual attention (SAM + CAM) for enhanced weld feature extraction.
- Neck – Bidirectional Path Aggregation Network (Bi-PAN) for fusing multi-scale features to detect defects of various sizes.
- Head – Decoupled classification and regression branches for independent optimization of detection accuracy and localization.


<img width="747" height="332" alt="image" src="https://github.com/user-attachments/assets/82254e4b-dbdf-4a71-91c7-3cd02521d832" />

Figure: Customized YOLOv12 architecture for weld inspection.


### Results

<img width="569" height="460" alt="image" src="https://github.com/user-attachments/assets/fb5f85c5-c488-43b4-9b87-07c530deeb2c" />

Figure: Example predictions showing correct detection and classification of Good Weld, Bad Weld, and Defect regions.


### Tools & Technologies:
```
Python 3.12.12
PyTorch 2.8.0 + CUDA 12.6
Ultralytics YOLOv12 (customized architecture)
Torchvision
NumPy / Pandas
OpenCV
Matplotlib & Seaborn
```



#### Citations
If you use this work, please cite:

T. Kidu, Y. Abraha, Y. Berhane, H. Gebrekidan, and T. Tesfaye,
“Automated Weld Quality and Defect Detection for Industrial Applications: A Deep Learning Framework for Real-Time Visual Inspection,”
in IEEE Proc. ACAI 2025.


