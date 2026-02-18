TACO Trash Instance Segmentation 🛰️🗑️

🚀 Project Overview
This project focuses on the automated detection and segmentation of environmental litter. Using the TACO (Trash Annotations in Context) dataset, we built a Deep Learning model capable of identifying individual pieces of waste in diverse real-world settings.

Our goal is to support smart-city initiatives like automated cleaning robots and intelligent waste-sorting bins.

🛠️ Tech Stack
Framework: PyTorch

Architecture: Mask R-CNN with ResNet-50-FPN backbone

Dataset: TACO (COCO-style annotations)

Libraries: torchvision, pycocotools, opencv, albumentations

📊 Methodology
We implemented an Instance Segmentation approach, which provides pixel-level masks rather than just bounding boxes.

Key Features:
Transfer Learning: Leveraged pre-trained weights from the COCO dataset to improve learning speed and accuracy.

Data Augmentation: Applied random flips, brightness adjustments, and blurring to handle varied lighting and "waste in the wild."

Class Mapping: Consolidated 60 original TACO categories into 4 manageable super-categories: Plastic, Glass, Metal, and Other.

📈 Evaluation Metrics
The model is evaluated using the standard COCO metrics:

mAP (Mean Average Precision) for masks.

Per-class AP to identify strengths and weaknesses in material detection.
