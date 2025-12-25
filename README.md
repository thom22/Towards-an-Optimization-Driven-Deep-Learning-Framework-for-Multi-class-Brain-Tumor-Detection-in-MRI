# Towards-an-Optimization-Driven-Deep-Learning-Framework-for-Multi-class-Brain-Tumor-Detection-in-MRI

### Project Overview
This project presents an advanced deep learning based object detection pipeline for multi class brain tumor detection and localization from MRI scans. Instead of only predicting a scan level label, the model detects tumor regions using bounding boxes and assigns one of four classes: Glioma, Meningioma, Pituitary Tumor, or No Tumor. The framework is designed to handle common MRI challenges such as low contrast tumor boundaries, high variation in tumor size and morphology, and appearance differences caused by acquisition settings. The final model was trained with controlled medical imaging augmentations and an optimized training configuration to improve stability and generalization.

---

### Model Description
We build an object detection framework based on the latest YOLOv12n (You Only Look Once)** architecture for an efficient balance between computational cost and detection accuracy. The pipeline takes resized MRI inputs (640 × 640) and applies preprocessing and controlled augmentations, followed by a backbone that performs **multi scale feature extraction**. A **PANet neck** fuses features across resolutions using upsampling and concatenation to strengthen small and large tumor detection. Finally, multi scale detection heads output **bounding boxes, confidence scores, and class labels** for the four categories.  

<img width="1117" height="481" alt="image" src="https://github.com/user-attachments/assets/9f5b9821-b58e-4879-97fc-59e7b146f8fb" />

---

### Results
The trained detector achieves strong performance for multi class tumor detection on the test set and produces tight bounding box localizations across different MRI orientations and tumor sizes. Qualitative examples show correct detections across all four classes with confidence scores typically ranging from **~0.68 to ~0.87**, demonstrating practical detection behavior in diverse MRI scenarios.  

<img width="622" height="304" alt="image" src="https://github.com/user-attachments/assets/a1959636-d7e9-4006-8b73-19110167e7e3" />


### Tools & Technologies:
```
Python 3.12.12
PyTorch 2.8.0 + CUDA 12.6
Ultralytics YOLOv12 (customized architecture)
Torchvision
NumPy / Pandas (data handling)
OpenCV / Pillow** (image preprocessing utilities)
Matplotlib & Seaborn (training curves and evaluation visualizations)
```



### Citation
If you use this work, please cite:

T. Kidu, Y. Abraha, Y. Berhane, H. Gebrekidan, A. Ramakrishnan and T. Tesfaye,  
“Towards an Optimization Driven Deep Learning Framework for Multi Class Brain Tumor Detection in MRI Imaging,”  
in *IEEE Proc. 2025 6th International Conference on Computers and Artificial Intelligence Technology (CAIT) 2025*.

---

