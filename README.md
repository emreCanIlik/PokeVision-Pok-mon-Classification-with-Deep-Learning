# **1000 Pokémon Dataset**


Pokémon dataset includes approximately 40 images for each of the 1,000 Pokémon species, organized into subdirectories by class. Each image is in PNG format and resized to 128x128 pixels. Initially created for a Pokédex project in Flutter, it is recommended to apply data augmentation when using this dataset for model training.

![image](https://github.com/user-attachments/assets/1f0ec613-bde8-480e-bcb5-0b8d6227db6d)

Dataset Overview

    Total images: 26,539
    Total classes: 1,000
    Size: ~407MB

Suggested Use Cases

    Image classification tasks
    Fine-tuning Vision Transformers or Convolutional Neural Networks
    Benchmarking datasets for computer vision projects


# Pokémon Image Classification with Deep Learning

This project focuses on classifying images of Pokémon species using deep learning techniques, leveraging the **EfficientNetV2B0** architecture for transfer learning. The dataset consists of 1,000 Pokémon species, with approximately 40 images per species, resized to 128x128 pixels and stored as PNG files.

## Key Steps:

1. **Dataset Preparation:**
   - Organized dataset into training, validation, and test sets.
   - Used TensorFlow’s `image_dataset_from_directory` for efficient data loading.

2. **Data Augmentation:**
   - Applied various augmentation techniques to enhance dataset variability and improve model generalization.

3. **Model Architecture:**
   - **EfficientNetV2B0** pre-trained model used for feature extraction.
   - Frozen base model initially for transfer learning, followed by fine-tuning.
   - **Global Average Pooling** layer used to reduce overfitting.

4. **Model Training:**
   - Compiled with **categorical cross-entropy** loss and the **Adam optimizer**.
   - Achieved solid classification performance for multi-class image classification tasks.

## Technologies Used:
- **TensorFlow** for model training and evaluation.
- **Keras** for model building and fine-tuning.
- **Python** for data preprocessing and analysis.

This repository serves as a great example of applying deep learning techniques to a large-scale image classification problem using transfer learning. It can be used for benchmarking, further fine-tuning, or as a foundation for similar image classification tasks.
