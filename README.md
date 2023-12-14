# Deep Learning Model For Encrypting Images For Vehicles' Numberplates

A deep learning model that detects license plates/registration plate numbers in images, and then encrypts them for privacy purposes.

<!-- Use `jupyter lab --allow-root` in terminal. -->

## Short Demonstration

### Initial image:

<br>

![Initial image](./manually_test/fr61z22ysw5z.jpg)

### Final image:

<br>

![Final image](./encrypted.jpg)

### Image Bouding Box

<br>

![Image Bouding Box](./runs/detect/train22/fr61z22ysw5z.jpg)


## Complete Jupyter Notebook

### 🖱️ [Click Here](./Vehicle_Image_Encryption_Research.ipynb)


## Current Results

| Metric                       | Result |
| ---------------------------- | ------ |
| Number of correct detections | 896    |
| Precision                    | 0.98   |
| Recall                       | 0.99   |
| F1 Score                     | 0.99   |
| True Positives (TP)          | 896    |
| False Positives (FP)         | 15     |
| False Negatives (FN)         | 6      |
| Accuracy                     | 0.98   |

## Used Dataset

Source: [Roboflow](https://universe.roboflow.com/augmented-startups/vehicle-registration-plates-trudk/dataset/1?ref=roboflow2huggingface)

Categories: YOLOv8 <br>
Classes: 1 <br>
Class Names: 'License_Plate' <br>

## Dataset Split

- Train set: 80% (6176 images)
- Validation set: 20% (1765 images)
- Test set: 10% (882 images)

## Dataset Preprocessing

- Auto-Orient: Applied
- Resizing: Applied (460x460)
- Zooming
- Cropping

#### The dataset is also available in the `dataset` folder.
