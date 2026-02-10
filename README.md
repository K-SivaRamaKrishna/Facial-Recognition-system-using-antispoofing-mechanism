
## Face Anti-Spoofing using MobileNetV3 & Vision Transformer

This project focuses on building a **real-time Face Anti-Spoofing system** to detect whether a face is **Live or Spoof (photo/video attack)**. The pipeline uses **MTCNN for face detection**, and compares **MobileNetV3-Small and Vision Transformer (ViT)** models for classification and generalization.

### Key Features

* Face detection and preprocessing using **MTCNN**
* Lightweight CNN model: **MobileNetV3-Small**
* Transformer model: **Vision Transformer (ViT)**
* Evaluation using **Accuracy, AUC, ROC Curve & Confusion Matrix**
* Tested on **original and new unseen dataset**
* Model converted to **TensorFlow Lite (TFLite)** for edge/mobile deployment

### Results Summary

* MobileNetV3 achieved **AUC ≈ 0.91** on the original dataset
* ViT achieved **AUC ≈ 0.84** on the original dataset
* Performance dropped on new dataset → highlights **generalization challenge**
* Training curves show **zig-zag patterns**, indicating need for further tuning and more data.

### Tech Stack

Python • TensorFlow/Keras • OpenCV • MTCNN • MobileNetV3 • Vision Transformer • TFLite

### Future Improvements

* Collect larger real-world dataset
* Improve generalization using augmentation
* Build ensemble model (MobileNet + ViT)
* Deploy real-time mobile application

---
