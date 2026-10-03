# Facial Emotion Detection Using YOLO11

## Project Overview

This project focuses on detecting and classifying human facial expressions using a fine-tuned YOLO11 model.

The model is trained to identify nine facial expression categories from images using object detection techniques.

The project was developed in Google Colab using a pretrained YOLO11 model and GPU acceleration.
## Emotion Classes

The model detects the following nine facial expressions:

1. Angry
2. Contempt
3. Disgust
4. Fear
5. Happy
6. Natural
7. Sad
8. Sleepy
9. Surprised
## Dataset

The model was trained using the **8-Facial-Expressions-for-YOLO** dataset from Kaggle.

The dataset contains annotated facial images prepared in YOLO format for object detection.

### Dataset Split

| Split      |    Images |
| ---------- | --------: |
| Training   |     7,000 |
| Validation |     1,000 |
| Testing    |     1,000 |
| **Total**  | **9,000** |
## Model

This project uses **YOLO11n**, a pretrained YOLO11 model that was fine-tuned for facial emotion detection.

### Training Configuration

* **Model:** YOLO11n
* **Task:** Object Detection
* **Training Epochs:** 10
* **Image Size:** 416 × 416
* **Batch Size:** 16
* **Workers:** 2
* **Environment:** Google Colab
* **GPU:** NVIDIA Tesla T4
## Model Performance

The trained model was evaluated using standard object detection metrics.

| Metric    | Result |
| --------- | -----: |
| Precision |  53.1% |
| Recall    |  55.0% |
| F1-Score  | ~54.0% |
| mAP@50    |  58.7% |
| mAP@50–95 |  43.1% |

These results represent the performance of the trained model on the evaluation data used in the project.
## Technologies Used

* Python
* YOLO11
* Ultralytics
* Google Colab
* PyTorch
* OpenCV
* NumPy
* Matplotlib
* Kaggle Dataset
## Project Workflow

1. Obtain and prepare the facial expression dataset.
2. Use the YOLO-format annotations provided with the dataset.
3. Load the pretrained YOLO11n model.
4. Fine-tune the model on the facial expression dataset.
5. Evaluate the trained model using precision, recall, F1-score, and mAP.
6. Use the trained model to detect facial expressions in new images.
## Usage

The complete implementation is provided in the Google Colab notebook included in this repository.

Open the `.ipynb` file in Google Colab and run the cells sequentially to:

* Prepare the dataset
* Train the YOLO11n model
* Evaluate the model
* Perform facial emotion detection on images

The notebook also contains the code used for inference on custom images.
## Limitations

The current model provides a baseline for facial emotion detection, but its performance can be improved further. The reported results indicate that the model may have difficulty detecting some facial expressions consistently.

## Future Improvements

* Train for more epochs.
* Perform hyperparameter tuning.
* Investigate class imbalance.
* Improve data quality and augmentation.
* Analyze per-class performance using a confusion matrix and class-wise metrics.
* Test the model on more diverse real-world facial images.
* Explore deployment as a future application.
## Project Status

**Completed — Experimental / Learning Project**

The current version demonstrates the complete workflow of training and evaluating a YOLO11-based facial emotion detection model. Further improvements can be made through additional training, tuning, and experimentation.
