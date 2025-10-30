# Smart-Digit-Recognition
A Machine Learning model that recognizes handwritten digits using a neural network.



📋 Overview

This project focuses on building a machine learning model capable of recognizing handwritten digits (0–9). The model uses traditional ML techniques with HOG (Histogram of Oriented Gradients) for feature extraction and a Support Vector Machine (SVM) classifier for prediction.

⚙️ Tools & Technologies

Language: Python

Platform: Google Colab

Libraries: OpenCV, NumPy, Pandas, scikit-learn, scikit-image, Matplotlib

Model: Support Vector Machine (SVM) with RBF Kernel

Feature Extraction: HOG (Histogram of Oriented Gradients)



📊 Dataset

Total Images: ~1000 (10 digits × ~100 images each)

Train-Test Split: 70% training, 30% testing

Image Preprocessing:

Converted to grayscale

Resized to 28×28 pixels

Normalized pixel values (0–1 scale)

🔍 Methodology

Dataset Access: Mounted Google Drive in Colab.

Preprocessing: Standardized and normalized input images.

Feature Extraction: Applied HOG to capture edge and shape features.

Model Training:

Used SVM with RBF kernel.

Tuned hyperparameters using GridSearchCV.

Best parameters: C=10, gamma=0.1, kernel='rbf'.

Model Saving: Stored trained model with joblib for reuse.

🧩 Results

Accuracy: ~62% on test data

Evaluation Metrics: Confusion matrix, precision, recall, and F1-score

Observations:

High precision for digits 0, 1, 2, 7, and 9

Misclassifications common among similar digits (e.g., 3↔8, 4↔9, 5↔6)

Augmentation didn’t improve accuracy significantly

🧪 Testing

Single Image Prediction: Upload an image and get digit prediction.

Batch Prediction: Process multiple images from a folder.


🏁 Conclusion

This project demonstrates a complete handwritten digit recognition pipeline using traditional machine learning. The HOG + SVM approach achieved ~62% accuracy and proved effective for small datasets. It establishes a foundation for further improvement using deep learning techniques.
