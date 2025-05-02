🚗 Accident Detection Using EfficientNet-B3
This project uses deep learning to detect traffic accidents in real-time from video feeds using EfficientNet-B3. The system is designed to work even in foggy or low-visibility conditions and helps in triggering alerts for quick response.

🔍 Project Overview
Real-time accident detection using CCTV or camera footage.

Built using EfficientNet-B3 pre-trained on ImageNet.

Trained on a dataset of accident/non-accident images with advanced augmentations like fog, brightness, and noise.

Capable of detecting accidents even in challenging weather conditions.

🧠 Model Architecture
Base Model: EfficientNet-B3 (pre-trained on ImageNet).

Custom head added:

Flatten Layer

Dense Layer with Sigmoid activation

Activation Functions:

ReLU for intermediate layers

Sigmoid for final classification

Loss Function: CrossEntropy with class weights to manage class imbalance.

Optimizer: Adam

Trained for 60 epochs, tracking accuracy, precision, recall, and F1-score.

🔄 System Workflow
Input: Real-time video stream or image frames.

Processing: Each frame is passed through the model.

Output: If an accident is detected, the system triggers an alert.

🧰 Technologies Used
Deep Learning Framework: PyTorch

Model: EfficientNet-B3

Computer Vision: OpenCV

Augmentations: Albumentations (fog, brightness, noise, etc.)

Data Tools: pandas, numpy

Language: Python

📁 Dataset Overview
Training Data: Accident/Non-Accident images from traffic datasets with foggy and weather-based augmentations.

Validation Data: Similar to training, used to avoid overfitting.

Testing Data: Real-world video frames to test performance.

📊 Performance
High Accuracy and F1 Score on both training and validation sets.

Confusion Matrix showed:

High True Positive Rate (accidents detected correctly).

High True Negative Rate (very few false alarms).
