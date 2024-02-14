# Image Classification with Transfer Learning

## Overview
This project aims to predict image categories and landmark names using transfer learning with the EfficientNetB0 pre-trained model. By leveraging transfer learning, we can utilize pre-trained neural network weights, allowing for training with fewer data points and computational resources. The project employs data augmentation techniques like rotation, translation, flipping, and contrast adjustment to enhance model performance.

## Team Members
- Lian Lian
- Aining Ding
- Weixin Sheng
- Yuqi Zhang

## Dataset
The dataset comprises images of five famous landmarks, categorized into six groups: Gothic, Modern, Mughal, Neoclassical, Pagodas, and Pyramids. Given the small size of the dataset, transfer learning and data augmentation are crucial to improving model accuracy.

## Methods
1. **Data Loading**: Images are loaded from Google Drive, sorted by landmark within each architectural category.
2. **Data Augmentation**: Includes RandomRotation, RandomTranslation, RandomFlip, and RandomContrast to generate additional training data.
3. **Model Selection**: EfficientNetB0 was chosen for its efficiency. The model's lower layers are frozen to prevent overfitting, with fine-tuning applied to the upper layers.
4. **Training**: The dataset is split into 80% training and 20% validation, targeting both category and landmark predictions.

## Results
The model achieved ~96% accuracy in category classification and ~91.6% in landmark classification, highlighting the effectiveness of transfer learning and data augmentation in this context.

## Conclusions
This project validates the application of transfer learning and data augmentation in image classification tasks, especially with limited datasets. Future efforts will focus on model fine-tuning and exploring more advanced regularization techniques.

## Bibliography
- [Keras Documentation](https://keras.io)
- [TensorFlow Documentation](https://www.tensorflow.org)
- [Scikit-learn Documentation](https://scikit-learn.org)

