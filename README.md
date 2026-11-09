# Handwritten Character Recognition Using CNN

## Project Overview
This project is a Handwritten Character Recognition system developed using a Convolutional Neural Network (CNN). It recognizes handwritten English alphabet characters (A–Z) from uploaded images.

The model is trained using the EMNIST Letters dataset and uses image preprocessing techniques to improve recognition accuracy.

## Objectives
- Recognize handwritten English alphabet characters from A to Z.
- Train a CNN model using an existing handwritten character dataset.
- Process uploaded handwritten images for prediction.
- Display the predicted character and its confidence score.

## Dataset
**EMNIST Letters Dataset**

Dataset: https://www.kaggle.com/datasets/crawford/emnist

The dataset contains:
- 88,800 training images.
- 14,800 testing images.
- 26 alphabet classes (A–Z).
- Each image has a resolution of 28 × 28 pixels.
- Uppercase and lowercase letters are combined into the same class.

Required files:
- `emnist-letters-train.csv`
- `emnist-letters-test.csv`

## Technologies Used
- Python
- TensorFlow / Keras
- Convolutional Neural Network (CNN)
- NumPy
- Pandas
- Matplotlib
- OpenCV
- Pillow
- Google Colab

## Model Architecture
The CNN model consists of:
1. Convolutional layers for feature extraction.
2. Batch Normalization for stable training.
3. Max Pooling layers for dimensionality reduction.
4. Flatten layer to convert feature maps into a vector.
5. Dense layers for classification.
6. Dropout to reduce overfitting.
7. Softmax output layer for 26 alphabet classes.

## Workflow
1. Upload the EMNIST training and testing datasets.
2. Load and preprocess the images.
3. Normalize pixel values and reshape images.
4. Build and compile the CNN model.
5. Train the model using the training dataset.
6. Evaluate the model using the testing dataset.
7. Upload a handwritten character image.
8. Preprocess the uploaded image.
9. Predict the character and display the confidence score.

## Output
The system displays:
- Predicted alphabet character.
- Prediction confidence percentage.
- Top three predicted characters.
- Training and validation accuracy graph.
- Test dataset accuracy.

## How to Run the Project

1. Open [Google Colab](https://colab.research.google.com/).
2. Create a new notebook.
3. Copy the project code into a code cell.
4. Run the code.
5. Upload the EMNIST training and testing CSV files when prompted.
6. Wait for the model to train.
7. Upload an image containing a single handwritten alphabet character.
8. View the prediction result.

## Project Structure

```text
Handwritten-Character-Recognition/
│
├── README.md
├── handwritten_character_model.keras
├── emnist-letters-train.csv
└── emnist-letters-test.csv
```

## Future Enhancements
- Improve recognition accuracy for different handwriting styles.
- Support recognition of handwritten words and sentences.
- Develop a web application for real-time character recognition.
- Support handwritten digit recognition.
- Improve image preprocessing for different lighting conditions.

## Conclusion
This project demonstrates the use of Convolutional Neural Networks for handwritten alphabet recognition. It trains on the EMNIST Letters dataset and predicts characters from user-uploaded handwritten images.