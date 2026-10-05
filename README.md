DeepFashion Classification using VAE + ResNet50

Overview

This project focuses on fashion image classification using the DeepFashion dataset. It combines ResNet50 for feature extraction, a Variational Autoencoder (VAE) for learning compact latent features, and a Dense Neural Network for clothing category classification.

Architecture

Input Image
    ↓
Preprocessing & Augmentation
    ↓
ResNet50
    ↓
VAE
    ↓
Latent Features
    ↓
Dense Classifier
    ↓
Fashion Category

Dataset

The project uses the DeepFashion dataset, which contains clothing images across multiple fashion categories with variations in pose, background, and appearance.

Dataset: https://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html

Technologies

* Python
* TensorFlow / Keras
* ResNet50
* Variational Autoencoder (VAE)
* NumPy
* Matplotlib / Seaborn
* Scikit-learn

Model

ResNet50: A pretrained ResNet50 model is used to extract visual features from fashion images.

VAE: The extracted features are passed through a Variational Autoencoder to learn a compact latent representation.

Classifier: The latent features are passed to a Dense Neural Network with a Softmax output layer for final category prediction.

Training

Parameter	Value
Image Size	224 × 224
Batch Size	16
Optimizer	Adam
Loss	Categorical Crossentropy
Validation Split	30%

Evaluation

The model is evaluated using:

* Accuracy
* Precision, Recall and F1-score
* Confusion Matrix
* ROC Curve
* Training and Validation Loss

Run

Install the dependencies:

pip install tensorflow keras numpy matplotlib seaborn scikit-learn jupyter

Start Jupyter Notebook:

jupyter notebook

Open DeepFashion.ipynb and run the cells in order.

Conclusion

This project demonstrates an end-to-end fashion classification pipeline combining transfer learning, latent representation learning, and deep neural network classification.