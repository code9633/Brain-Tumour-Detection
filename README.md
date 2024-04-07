# Brain Tumor Detection

This repository contains code for a brain tumor detection system using deep learning techniques. The system uses a convolutional neural network (CNN) to classify magnetic resonance images (MRI) of the brain as either containing a tumor or being healthy.

## Dataset

The [brain tumor dataset](https://www.dropbox.com/s/jztol5j7hvm2w96/brain_tumor%20data%20set.zip) used in this project is downloaded and preprocessed. It consists of MRI images categorized into two classes: brain tumors and healthy brains.

## Model Architecture

The CNN model architecture consists of multiple convolutional layers, followed by max pooling, dropout, and dense layers. The final layer uses a sigmoid activation function to output a probability indicating the presence of a tumor.

## Data Preparation

The dataset is split into three sets: training, validation, and testing, with proportions of 70%, 15%, and 15% respectively. Data augmentation techniques such as zooming, shearing, and horizontal flipping are applied to the training set to improve model generalization.

## Model Training

The model is trained using the training set and evaluated on the validation set. Early stopping and model checkpointing are implemented to prevent overfitting and save the best model based on validation accuracy.

## Model Evaluation

The trained model is evaluated on the testing set to measure its performance. The accuracy of the model is calculated and reported.

## Prediction

A sample image from the validation set is selected, and the trained model is used to predict whether it contains a brain tumor or not. The image is displayed with a highlighted region indicating the predicted class.

Please refer to the Jupyter Notebook file [Brain_Tumor_Detection.ipynb](https://colab.research.google.com/drive/1uXj2QMmNOCJVEAAXgIA7l4_Dk5CjpXbx) for the complete code and detailed implementation.

## Results

The model achieves an accuracy of [insert accuracy value]% on the testing set. The training and validation accuracy and loss curves are shown in the accompanying plots.

![Accuracy Curve](github/acc.PNG!)[Loss Curve](github/loss.PNG)

## Example Prediction

![Example Image]g(ithub/output.PNG)

The above image is predicted to have a brain tumor with a probability of [insert probability value]. The predicted class label is "Brain Tumor".

## Conclusion

This project demonstrates the application of deep learning techniques for brain tumor detection using MRI images. The trained model shows promising results in accurately identifying the presence of brain tumors.