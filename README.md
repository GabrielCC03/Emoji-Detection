# Emoji-Detection
Emoji Detection with traditional machine learning algorithms

# Emoji Classification with SVM

This repository contains my computer vision project for COMP4423 (Semester 2, 2023/24) that tackles the challenge of classifying emojis using traditional machine learning techniques.

## Project Overview

Emojis, though simple in appearance, are notoriously difficult to classify due to their high visual similarity. This project covers:
- **Data Collection & Preprocessing:** An extended, manually labeled dataset with 24 classes.
- **Feature Extraction:** Application of Sobel, Laplacian, Circular LBP, and HOG filters to extract meaningful features.
- **Image Stacking:** Combining filtered outputs to simulate a CNN-like flattening process.
- **Model Training:** Using a Support Vector Classifier (SVC) optimized with grid search and cross-validation.
- **Testing:** Achieved 60.42% accuracy on emojis, highlighting challenges when applied to human facial expressions.

## Dataset
Link: https://emojikitchen.dev
- **Composition:** 149 training images and 48 testing images across 24 classes.
- **Challenges:** Overlapping features between classes and limited data per class, resulting in a low baseline chance of random correct classification.

![TSNE](https://github.com/user-attachments/assets/8dd34cdb-a75a-4222-9835-c641d72b8bca)


## Methods

- **Preprocessing:** Converting Unicode emojis to grayscale images.
- **Feature Extraction Techniques:**
  - *Sobel Filter:* For edge detection.
  
![Sobel](https://github.com/user-attachments/assets/c85d986d-f17d-4f53-86d8-a7359383acc8)

  - *Laplacian Filter:* To highlight sharp features.
    
![Laplacian](https://github.com/user-attachments/assets/aee91ee9-89ae-43ec-aaa8-b5359d42627a)

  - *Circular LBP:* For capturing local texture details.
    
![CircleLBP](https://github.com/user-attachments/assets/a4b0612a-82ab-4ede-a2c3-6eeca71a2263)

  - *HOG:* For local shape patterns.
  
![Hog](https://github.com/user-attachments/assets/69eb6e89-bd33-4b5b-8d95-1aab3a822483)

- **Model:** A Support Vector Classifier was chosen due to its strength in handling high-dimensional, non-linear data.
- **Training & Optimization:** Employed grid search with cross-validation to fine-tune hyperparameters.

## Results & Discussion
- **Emoji Classification:** Achieved an accuracy of 60.42%.
- **Future Work:** Expand the dataset with colored images and refining feature extraction techniques to reduce class overlap.
