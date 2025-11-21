Project Objective:
Classify chest X-ray images into three categories: COVID-19, Pneumonia, and Normal using deep learning.

Dataset Preparation:
Used publicly available COVID-19 radiography datasets.
Applied image preprocessing and real-time data augmentation to improve model robustness.

Model Architecture:
Employed transfer learning with DenseNet121 pretrained on ImageNet.
Added custom classification layers for three output classes.

Model Training:
Trained using TensorFlow and Keras frameworks.
Used sparse categorical cross-entropy loss and Adam optimizer.
Validated model performance using separate validation data

Model Saving and Loading:
Saved the trained model as covid_xray_model.h5.
Loaded the saved model for making predictions on new images.

 Prediction Workflow:
Preprocessed input X-ray images to match model input size (224x224).
Ran the model to predict the class index, then mapped it to readable labels (COVID-19, Pneumonia, Normal).
