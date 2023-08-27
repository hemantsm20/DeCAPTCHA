# DeCAPTCHA(HexaCAPTCHA)

## Problem Description

In the world of online security, CAPTCHAs (Completely Automated Public Turing test to tell Computers and Humans Apart) are commonly used to distinguish between humans and bots. Traditional CAPTCHAs present an image containing characters that need to be identified in a specific order. This assignment focuses on "HexaCAPTCHAs" where the challenge is to recognize a 4-digit hexadecimal number displayed in an image.

Each HexaCAPTCHA image is 500 × 100 pixels in size and contains a 4-digit hexadecimal code. The characters A-F are in upper case, and each character can be rotated (in degrees of 0, ±10, ±20, ±30) and displayed in a different color. The background color can also vary, but it's always a light shade. The images also have random stray lines in the background for added complexity.

## Problem Statement

Your task is to predict whether the 4-digit hexadecimal number in an image is odd or even. Given a HexaCAPTCHA image, your output should be the string "EVEN" if the number is even and "ODD" if the number is odd.

For example, the hexadecimal number 10 is even because it corresponds to the decimal number 16, which is even. On the other hand, the hexadecimal number DECAF is odd because it corresponds to the decimal number 912559, which is odd.

## Dataset

You are provided with a training dataset containing 2000 HexaCAPTCHA images and their corresponding labels (odd/even) in the file `training_labels.txt`.

## Task

Your task is to build a predictive model that can accurately classify HexaCAPTCHA images as "ODD" or "EVEN" based on the hexadecimal number they contain.

## Approach

1. **Image Preprocessing**: Load and preprocess the HexaCAPTCHA images, including rotation, color adjustment, and removing background noise.
   
2. **Feature Extraction**: Extract relevant features from the preprocessed images that will help the model learn to classify them.
   
3. **Model Selection and Training**: Choose an appropriate machine learning algorithm (e.g., Support Vector Machine) and train it using the extracted features and their corresponding labels.
   
4. **Model Evaluation**: Evaluate the trained model's performance using appropriate metrics and techniques.
   
5. **Deployment**: Deploy the trained model to predict whether new HexaCAPTCHA images are odd or even.

## Getting Started

1. Clone this repository to your local machine.
   
2. Ensure you have the required libraries installed (e.g., OpenCV, numpy, scikit-learn).
   
3. Preprocess the images and extract features.
   
4. Train and evaluate your predictive model.
   
5. Deploy the model to make predictions on new HexaCAPTCHA images.

## Disclaimer

This project is intended for educational purposes and aims to solve the HexaCAPTCHA problem. The provided reference images can be used to enhance the model's performance, and creative approaches are encouraged. Remember that real-world CAPTCHAs may involve more complex challenges.
