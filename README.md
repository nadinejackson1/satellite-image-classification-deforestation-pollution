### 100 Days of Machine Learning: Day 23

# Satellite Image Classifier for Deforestation and Pollution

This repository contains a satellite image classifier that identifies signs of deforestation and pollution using transfer learning with a pre-trained ResNet50 Convolutional Neural Network (CNN) model. The model is fine-tuned for binary classification tasks to detect 'habitation' as a proxy for deforestation and 'slash_burn' as an indicator of pollution in Amazon rainforest satellite images.

### Dataset

The dataset used for this project is sourced from the [Planet: Understanding the Amazon from Space Kaggle competition](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space/data). The dataset contains multi-label satellite images taken from the Amazon rainforest, with each image associated with one or more tags.

### Requirements

    Python 3.7+
    TensorFlow 2.0+
    pandas
    scikit-learn
    Keras
    Matplotlib

### Usage

1. Download the dataset from the [Planet: Understanding the Amazon from Space Kaggle](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space/data) competition and extract the contents to a directory named data.

2. Run the **satellite_image_classifier.py** script to train the model:

         python satellite_image_classifier.py

3. After training, the model will be saved as **'model.h5'**. You can use the **predict_deforestation_pollution()** function in the **satellite_image_classifier.py** script to make predictions on new images.

### License

This project is licensed under the **MIT License**. See the **LICENSE** file for details.
