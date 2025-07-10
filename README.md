# Multiclass-Fish-Image-Classification
This project focuses on classifying fish images into multiple categories using deep learning models and deploying a Streamlit application to predict fish categories from user-uploaded images.

## Business Use Cases:
1.	Enhanced Accuracy: Determine the best model architecture for fish image classification.
2.	Deployment Ready: Create a user-friendly web application for real-time predictions.
3.	Model Comparison: Evaluate and compare metrics across models to select the most suitable approach for the task.

### Dataset
The dataset consists of images of fish, categorized into folders by 11 species. The dataset is loaded using TensorFlow's ImageDataGenerator for efficient processing.
- data
  - test
    - class 1
    - class 2
    - class ..
  - train
    - class 1
    - class 2
    - class ..
  - val
    - class 1
    - class 2
    - class ..
   
## Approach:
- Data Preprocessing and Augmentation
  - Rescale images to [0, 1] range.
  - Apply data augmentation techniques like rotation, zoom, and flipping to enhance model robustness.
- Model Training
  - Train a CNN model from scratch.
  - Experiment with five pre-trained models (e.g., VGG16, ResNet50, MobileNet, InceptionV3, EfficientNetB0).
  - Fine-tune the pre-trained models on the fish dataset.
  - Save the trained model (max accuracy model ) in .h5 or .pkl format for future use.
- Model Evaluation
  - Compare metrics such as accuracy, precision, recall, F1-score, and confusion matrix across all models.
  - Visualize training history (accuracy and loss) for each model.
- Deployment
  - Build a Streamlit application to:
    - Allow users to upload fish images.
    - Predict and display the fish category.
    - Provide model confidence scores.

## CNN Architecture:
![CNN](https://github.com/Priyadharshini8163/Multiclass-Fish-Image-Classification/blob/main/CNN%20Architecture.png)

