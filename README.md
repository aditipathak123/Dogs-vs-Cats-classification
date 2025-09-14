# Dogs vs Cats Classification

## Overview
This project uses **Convolutional Neural Networks (CNN)** with **Transfer Learning (MobileNetV2)** to classify images of dogs and cats.  
Achieved **96% accuracy** on the validation set.

## Dataset
- Kaggle: [Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats/data)
- Images resized to 160x160 pixels.
- Data augmentation applied to improve generalization.

## Model
- Base: **MobileNetV2** (pre-trained on ImageNet)
- Added custom layers: GlobalAveragePooling2D → Dense → Dropout → Dense (sigmoid)
- Binary classification: Dog vs Cat

## Results
- Validation Accuracy: **96%**
- Confusion Matrix:
[[469 31]
[ 11 489]]
## Usage
1. Open `dogs_vs_cats.ipynb` in Google Colab
2. Run all cells to train or evaluate the model
3. Example prediction on a single image:
 ```python
 predict_img("path_to_image.jpg", model)

-
