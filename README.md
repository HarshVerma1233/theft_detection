
# Theft Detection Project

This project aims to develop a machine learning model capable of detecting shoplifting incidents from video footage. The model is designed to analyze video frames and classify them as either "shoplifting" or "normal" behavior.
Dataset
The project utilizes the DCSASS dataset, which contains videos labeled as "shoplifting" and "normal." The dataset is preprocessed to filter out irrelevant videos, and the remaining videos are converted into a suitable format for model training.
Model Architecture
The ResNet50 model, a deep convolutional neural network, is employed for this task. ResNet50 is known for its ability to learn complex patterns and features from images effectively, making it suitable for detecting subtle indicators of shoplifting behavior.

# Video Preprocessing: 
Videos are converted to a suitable format (224x224 resolution) and normalized to ensure consistent input data for the model.
Frame Extraction: A fixed number of frames (10) are extracted from each video to capture relevant visual information while avoiding overfitting.
Model Training: The ResNet50 model is trained on the preprocessed video frames, utilizing techniques such as global average pooling and a dense layer with a sigmoid activation function for binary classification.

# Evaluation
The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. The confusion matrix provides insights into the model's ability to correctly identify shoplifting and normal behavior instances.

# Potential Improvements

Data Augmentation: Implementing data augmentation techniques to enhance the model's generalization capabilities.
Model Complexity Adjustment: Exploring simpler model architectures or reducing the number of layers in ResNet50 to mitigate potential overfitting issues.
Better Dataset: Utilizing a more balanced dataset with a larger number of shoplifting instances and higher-quality video frames for improved model performance.
