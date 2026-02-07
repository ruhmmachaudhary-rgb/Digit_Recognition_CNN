# Digit_Recognition_CNN
# Digit Recognition using CNN

## Project Overview
This project predicts handwritten digits (0–9) from images using a Convolutional Neural Network (CNN).  
An interactive **Gradio interface** allows users to pick a random test sample and see the predicted digit along with prediction probabilities.

## Dataset
- **train.csv**: Contains labeled digit images (28x28 pixels).  
- **test.csv**: Contains unlabeled digit images for prediction.  

## Libraries Used
- Python, NumPy, Pandas  
- TensorFlow / Keras (CNN model)  
- scikit-learn (StandardScaler, train-test split)  
- Matplotlib (visualization of images and training curves)  
- Gradio (interactive demo for testing predictions)  

## Key Steps
1. Load and explore train and test datasets  
2. Visualize some sample images  
3. Preprocess data:  
   - Separate features and labels  
   - Standardize pixel values  
   - One-hot encode labels  
   - Reshape images to `(28, 28, 1)`  
4. Build CNN model:  
   - 2 convolutional + pooling layers  
   - Flatten layer → Dense layer → Dropout  
   - Output layer with softmax activation for 10 classes  
5. Train model with validation split  
6. Evaluate model:  
   - Training vs validation accuracy/loss plots  
   - Classification report on test set  
7. Interactive Gradio demo:  
   - Pick random sample from `test.csv`  
   - Predict digit and display prediction probabilities  

## How to Run
1. Clone the repository:
```bash
git clone <your-repo-link>
