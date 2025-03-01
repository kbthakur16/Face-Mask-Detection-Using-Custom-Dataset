# Face Mask Detection using YOLOv8

## Project Overview
This project aims to develop a Face Mask Detection model using YOLOv8. The model distinguishes between individuals wearing masks and those without masks in images and videos. The workflow consists of dataset preparation, model training, evaluation, and testing on video data.

## Project Structure
```
├── dataset_preparation.ipynb   # Data filtering and preparation
├── train_model.ipynb           # Model training script
├── test_model.ipynb            # Model evaluation and testing
├── Documentation.pdf           # Detailed project documentation
```

## Steps Involved

### 1. Data Preparation
- Filtered the dataset to retain only two labels: `Mask` and `No Mask`.
- Corrected bounding box coordinate inconsistencies.
- Converted bounding box annotations to YOLO format.

### 2. Model Training
- Used YOLOv8n.yaml for efficient training.
- Achieved **81.5% accuracy** after training for 7 epochs.

### 3. Model Evaluation
- Utilized a **confusion matrix** for performance analysis.
- Conducted batch evaluations to identify misclassifications and improve accuracy.

### 4. Video Testing
- Implemented **real-time inference** using OpenCV.
- Processed video frames to detect and classify masked/unmasked faces.
- Saved the processed video with bounding boxes and class labels.

## How to Run
1. **Prepare Dataset**: Run `dataset_preparation.ipynb` to process images and annotations.
2. **Train Model**: Execute `train_model.ipynb` to train YOLOv8 on the dataset.
3. **Evaluate Model**: Use `test_model.ipynb` to analyze performance metrics.
4. **Test on Video**: Modify and run the testing script to perform inference on video files.

## Dataset
The dataset used for training can be downloaded from the following link:
[Face Mask Detection Dataset](https://drive.google.com/file/d/1-VjzHSY_Y0kjT1fUMWHDqEMENTFk1NYr/view?usp=sharing)

## Requirements
Ensure the following dependencies are installed:
```bash
pip install ultralytics opencv-python numpy torch torchvision

## References
For a detailed explanation of each step, refer to `Documentation.pdf`.

---
