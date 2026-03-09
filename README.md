# strikezone

# AI Strike Zone Detection (YOLOv7)

This project explores automatic baseball strike zone detection using **computer vision and deep learning**. The system uses **YOLOv7** to detect the baseball in images and video frames and evaluates whether a pitch falls inside or outside the strike zone.

The goal of this project is to demonstrate how modern object detection models can assist with automated decision making in sports analytics.

---

## Project Overview

Baseball strike calls are traditionally determined by human umpires, which can introduce inconsistencies and bias. This project investigates how **deep learning models** can be used to detect the baseball and estimate pitch location from broadcast footage.

The model is trained using a **custom dataset exported from Roboflow** and trained with the **YOLOv7 architecture using PyTorch**.

Key steps in the pipeline:

1. Clone the YOLOv7 repository
2. Install dependencies
3. Download the custom dataset from Roboflow
4. Train the YOLOv7 model on baseball images
5. Run inference on test images to detect the baseball

---

## Technologies Used

* Python
* PyTorch
* YOLOv7
* OpenCV
* Roboflow
* Google Colab
* Jupyter Notebook

---

## Model Training

The model is trained on a custom baseball dataset using YOLOv7.

Training configuration:

* Model: YOLOv7
* Epochs: 100
* Batch size: 16
* Dataset format: YOLOv7 (Roboflow export)
* Framework: PyTorch

Training is performed in **Google Colab with GPU acceleration**.

---

## Running the Project

The easiest way to run this project is through Google Colab.

1. Open the notebook:

```
strikezone_yolov7_training.ipynb
```

2. Enable GPU in Colab:

```
Runtime → Change Runtime Type → GPU
```

3. Run all cells.

The notebook will:

* Install YOLOv7 dependencies
* Download the dataset
* Train the model
* Run detection on test images

---

## Example Output

The trained model detects the baseball in frames and produces bounding boxes around detected objects.

Example outputs include:

* Baseball detection bounding boxes
* Confidence scores for predictions
* Visualized detection results

(Example result images can be added in a `results/` folder.)

---

## Future Improvements

Possible extensions of this project include:

* Integrating **OpenPose** to detect batter posture
* Dynamically estimating the strike zone based on batter height
* Running inference on full game video
* Deploying the model as a **real-time strike detection system**


