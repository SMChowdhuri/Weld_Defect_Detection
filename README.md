# Weld Defect Detection | Deep Learning

## Overview

This project focuses on detecting weld defects using deep learning techniques. By fine-tuning a pre-trained ResNet50 and refining YOLOv5, the system achieves real-time defect detection with high accuracy. It also incorporates Class Activation Mappings (CAM) and segmentation techniques to improve model interpretability.

## Features

✅ Fine-tuned ResNet50 for defect classification with over 85% accuracy\
✅ Integrated GradCAM for visualizing key regions in classification\
✅ Applied SAM model for segmentation, Gaussian blur, and edge detection\
✅ Refined YOLOv5 model for real-time weld defect detection\
✅ Achieved a **MAP score of 0.82** for defect localization

## Technologies Used

- **PyTorch** – Model training and fine-tuning
- **ResNet50** – Pre-trained model for classification
- **GradCAM** – Class Activation Mapping for interpretability
- **SAM (Segment Anything Model)** – Image segmentation
- **YOLOv5** – Object detection for real-time analysis
- **OpenCV** – Image preprocessing (Gaussian blur, edge detection)

## Installation

### Prerequisites

Ensure you have Python installed (Python 3.8+ recommended). Install dependencies using:

```bash
pip install -r requirements.txt
```

### Clone the Repository

```bash
git clone https://github.com/SMChowdhuri/Weld_Defect_Detection.git
cd weld-defect-detection
```

## Usage

### Running the Classification Model

```bash
python classify.py --model resnet50 --image input.jpg
```

### Running the Object Detection Model (YOLOv5)

```bash
python detect.py --source video.mp4 --weights yolov5_best.pt
```

### Running Live Detection

```bash
python live_detection.py
```

## Dataset

- Custom dataset created for weld defect classification and detection.
- Preprocessed using image segmentation techniques for better bounding box identification.

## Results

- **Classification Accuracy**: 85%+ using ResNet50
- **MAP Score**: 0.82 with YOLOv5
- **Real-time Processing**: Optimized for live video streams

## Contributing

Feel free to fork this repository, create a branch, and submit a pull request for improvements.


## Contact

For any queries, feel free to reach out at [sumat4421@gmail.com].

