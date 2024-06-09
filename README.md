# Secured Encryption Mechanism On Vehicles’ Numberplates

A deep learning model that detects license plates/registration plate numbers in images, and then encrypts them for privacy purposes.

## Abstract

Information security has become crucial nowadays as it has ensured individual privacy and prevented unauthorized access. Securing data and information has the capability to establish a secure environment and has ensured trust by keeping them confidential and protected in diverse situations. The license plate or number plate information has been considered sensitive data as it contains unique identifiers for individuals' vehicles. Ensuring the security of this data is important to prevent unauthorized access, which could result in privacy violations and potential safety risks for vehicle owners. Our research has introduced an innovative security system for vehicle number plate privacy, featuring a powerful combination of a deep learning model and robust encryption. This system has ensured the secure transmission of information by adding an extra layer of protection to number plate data. Our proposed system has integrated the You Only Look Once version 8 (YOLOv8) for precise car number plate detection and utilized the robust security features of the Chaotic-based Logistic Map encryption process. This powerful combination has not only enhanced the accuracy of car number plate detection but also established a robust framework for efficiently safeguarding sensitive data through the use of chaotic encryption methods. It is an efficient approach where object detection has been combined with secure transmission technologies. It is suitable for real-time applications and traffic surveillance, resolving privacy concerns and emphasizing data security.

## Citation

Please add the following citation (BibTeX) to your research paper if you use our model/pipeline.

```
@inproceedings{khan2024vehicle,
  title={Vehicle Number Plate Detection and Encryption in Digital Images Using YOLOv8 and Chaotic-Based Encryption Scheme},
  author={Khan, Israt Jahan and Amin, Md Fahim Bin and Sabbir, Mahady Hasan and Nejhum, Durba Morshaline and Nanzil, Abu Hasib Muhammad and Rahman, Raiyan},
  booktitle={2024 6th International Conference on Electrical Engineering and Information \& Communication Technology (ICEEICT)},
  pages={717--722},
  year={2024},
  organization={IEEE}
}
```

## Conference Paper

You can access our research paper directly from [IEEE Xplore](https://ieeexplore.ieee.org/abstract/document/10534375/).

## Short Demonstration

Our research combines YOLOv8 for precise car number plate detection with a chaotic-based logistic map encryption method. YOLOv8 ensures accurate identification of number plates in real-time, while the chaotic encryption provides robust security. The integration of these technologies offers a streamlined and secure solution for handling car number plate data, applicable in diverse domains like transportation and surveillance.

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

## Configuration Of The Local Machine

|  **Component Category**  |          **Specific model**           |
| :----------------------: | :-----------------------------------: |
|           CPU            |    Ryzen 5 3500X 6 Core, 6 Threads    |
|           RAM            |          24GB DDR4 3200 BUS           |
|           GPU            |   Nvidia GeForce RTX 3050 8GB GDDR6   |
| Compute Capability (GPU) |                  8.6                  |
|        CUDA Cores        |                 2560                  |
|           SSD            | Samsung 980 1TB PCIe 3.0 M.2 NVMe SSD |

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
