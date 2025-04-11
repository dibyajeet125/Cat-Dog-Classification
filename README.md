# Cat-Dog-Classification
Developed a Cat Dog Classification model using CNNs, achieving up to 76.62% training accuracy and 60.20% validation accuracy on a dataset of 551 training images. Utilized VGG16 for feature extraction, further enhancing validation accuracy to 88.00%.


This project involves developing and training a Convolutional Neural Network (CNN) to classify images of cats and dogs. The dataset consists of 551 training images (249 cats, 302 dogs) and 500 validation images (250 cats, 250 dogs).

Methodology

Initial Model:

Architecture: The initial CNN model includes three convolutional layers (Conv2D) followed by max pooling layers, a flatten layer, and two dense layers.

Training: The model was trained for 10 epochs with a batch size of 20 using the RMSprop optimizer with a learning rate of 1e-4.

Metrics: Binary cross-entropy loss and accuracy were used as evaluation metrics.

Data Augmentation:

Techniques: To enhance model robustness, data augmentation techniques such as rotation, width/height shift, shear, zoom, and horizontal flip were applied.

Training: The augmented model was trained for 5 epochs with a batch size of 32.

Feature Extraction with VGG16:

Model: A pre-trained VGG16 model (without top layers) was used for feature extraction.

Classifier: Two dense layers were added on top of the extracted features.

Training: The classifier was trained for 10 epochs with a batch size of 20 using the RMSprop optimizer with a learning rate of 1e-5.

Performance Metrics

Initial Model:

Training Accuracy: Up to 76.62%

Validation Accuracy: Up to 60.20%

Augmented Model:

Training Accuracy: Up to 56.92%

Validation Accuracy: Up to 50.60%

VGG16 Feature Extraction Model:

Training Accuracy: Up to 99.95%

Validation Accuracy: Up to 88.00%

Key Findings

Data Augmentation: While it improved model robustness, careful tuning was necessary to avoid overfitting.

Pre-trained Models: Using VGG16 significantly enhanced performance, demonstrating the effectiveness of transfer learning.


Code Structure

The repository includes:

Model Definitions: Code for defining and training the CNN models.

Data Augmentation: Implementation of data augmentation techniques.

VGG16 Feature Extraction: Code for using VGG16 for feature extraction and adding a custom classifier.

Training Scripts: Scripts for training the models with specified hyperparameters.

Evaluation Metrics: Plots and metrics for evaluating model performance.

DATASET LINK: https://zenodo.org/records/5226945
