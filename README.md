🚦 A Data-Centric Approach to High-Accuracy Traffic Sign Detection Using Optimized YOLOv8

This repository contains the implementation and experimental results of my undergraduate research project focused on high-accuracy traffic sign detection using a data-centric optimization strategy with the YOLOv8-Large model.

Author: Piyash Basak
Institution: Daffodil International University
Degree: BSc in Software Engineering
Status: Final Year Research / Thesis

📌 Abstract

Traffic Sign Recognition (TSR) is a critical component of Autonomous Driving and Advanced Driver Assistance Systems (ADAS). Real-world performance is often degraded due to challenging conditions such as poor lighting, occlusion, blur, and small object sizes.

Instead of proposing a new architecture, this research adopts a data-centric approach to maximize the performance of an existing state-of-the-art detector, YOLOv8-Large, through optimized data preprocessing, augmentation, and training strategies.

The proposed framework achieves 94.18% mAP@0.5, demonstrating that high-quality data and training pipelines are as crucial as model design for reliable real-world deployment.

🎯 Objectives

Develop a robust training pipeline using YOLOv8-Large

Improve detection of small and distant traffic signs

Achieve state-of-the-art accuracy using data-centric optimization

Validate effectiveness through ablation studies

Ensure generalization under challenging real-world conditions

🧠 Methodology

Workflow Overview:

Dataset Preparation → Data Augmentation → YOLOv8 Training → Evaluation

Key Methodological Choices:

Model: YOLOv8-Large (≈55M parameters)

Approach: Data-centric optimization (not architecture redesign)

Evaluation: Quantitative metrics + ablation studies

📂 Dataset

Source: Roboflow – Traffic and Road Signs Dataset

Total Images: 10,000

Classes: 29 traffic sign categories

Split:

Training: 71% (7,092 images)

Validation: 19% (1,884 images)

Testing: 10% (1,024 images)

Input Size: 416 × 416

🔗 Dataset Link:
https://universe.roboflow.com/usmanchaudhry622-gmail-com/traffic-and-road-signs/dataset/1

🔧 Data Augmentation Strategy

A comprehensive augmentation pipeline was applied to improve robustness:

Random brightness & contrast

Blur and noise injection

Rotation and scaling

Horizontal flipping

Bounding box-aware transformations

📌 Impact:

Baseline (No Augmentation): 42.10% mAP

Proposed Method: 94.18% mAP

+52% absolute improvement

📊 Results
🔹 Final Test Performance
Metric	Value
mAP@0.5	94.18%
mAP@0.5:0.95	81.06%
Precision	97.70%
Recall	94.11%
🔹 Key Observations

Stable training with no overfitting

High accuracy across nearly all 29 classes

Strong performance under low-light, blur, and occlusion

Excellent localization for small objects

🔬 Ablation Study
Configuration	mAP@0.5
YOLOv8-L (No Augmentation)	42.10%
YOLOv8-L + Full Augmentation	94.18%

✔ Confirms the effectiveness of the data-centric approach

🏁 Conclusion

Successfully developed a high-accuracy traffic sign detection framework

Demonstrated that data quality and augmentation can outperform architectural tweaks

Validated YOLOv8-Large’s capacity for complex, real-world TSR tasks

Provides a reproducible and scalable solution for ADAS and autonomous driving systems

🚀 Future Work

Evaluate generalization on international datasets (e.g., GTSRB)

Integrate attention mechanisms for improved small-object detection

Optimize the model for edge and embedded deployment

Explore lightweight variants for real-time in-vehicle systems

📚 References

Flores-Calero et al., Mathematics, 2024

Mirzaei et al., Sensors, 2023

Huang et al., Journal of Computer and Communications, 2023

Han et al., Applied Sciences, 2023

Zhang et al., IEEE Access, 2024

Du et al., IET Image Processing, 2024

📄 Citation

If you use this work, please cite:

Piyash Basak,
"A Data-Centric Approach to High-Accuracy Traffic Sign Detection Using an Optimized YOLOv8 Model",
BSc Thesis, Daffodil International University, 2025.

🤝 Acknowledgements

Supervisor: Mr. Md. Rajib Mia
Lecturer (Senior Scale), Daffodil International University
