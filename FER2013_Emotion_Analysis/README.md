# FER2013 Emotion Analysis

This project focuses on emotion recognition using the **FER2013 dataset**. The main objective is to achieve the highest accuracy by experimenting with both well-known models and a custom-designed neural network.

## Models Used

The following models were utilized in this project:

1. **FER2013_with_MobileNetV2**
2. **FER2013_with_NewModel** (Custom neural network)
3. **FER2013_with_ResNet50**
4. **FER2013_with_VGG16**

All models were implemented using TensorFlow's Keras module.

## Dataset

The dataset used in this project is the **FER2013 dataset**, which can be downloaded from Kaggle:

[Download FER2013 Dataset](https://www.kaggle.com/datasets/msambare/fer2013/code)

## Project Goal

The primary goal of this project was to analyze the performance of various models on the FER2013 dataset and determine the most effective architecture for emotion recognition. A custom model, located in the `FER2013_with_NewModel` file, was also developed and evaluated alongside popular architectures.

## Key Observations and Results

1. **Custom Model (NewModel):**
   - Achieved the highest accuracy among all tested models.
   - Demonstrated better performance due to its simplicity and compatibility with the FER2013 dataset.

2. **MobileNetV2:**
   - Accuracy continued to improve during training, but the validation accuracy started to decrease, indicating overfitting.

3. **ResNet50:**
   - Training took a significant amount of time.
   - Accuracy did not improve for 6 epochs, so training was halted early.

4. **VGG16:**
   - Did not achieve the desired accuracy.
   - Performance was significantly lower than expected.

## Additional Features

- **Training and Validation Accuracy Visualization:**
  - Plots were created to show the training and validation accuracy values across epochs for each model.
  
- **Prediction Demo:**
  - Each model was tested with a randomly selected image from the test set to demonstrate its prediction capabilities.

## Conclusion

The results suggest that the FER2013 dataset, with its limited image quality and size, is better suited for less complex models. While well-known architectures like MobileNetV2, ResNet50, and VGG16 are powerful, they appear overly complex for this dataset. The custom-designed model, with fewer layers and parameters, was more effective in understanding the dataset and achieving higher accuracy.

## How to Run

Ensure tensorflow is installed.

    pip install tensorflow


Clone the repository.
   ```bash
   git clone https://github.com/ecekizilkaya/Deep-Learning/FER2013_Emotion_Analysis.git