# Simple-CV-Calculator
 
## Description

Goal of this the project is making the simple and lightweight application for deploying on the edge devices. 
Main task is segmenting and recognizing handwritten digits and math. operator in the image.
And finally creating a pipeline for calculating the value of that expression. It includes only basic operations : Add: +, Subtract: - , Multiply: * and Divide: /.
Covolutional Neural Network model contains 160 000 trainable params, making it easy to deploy on less powerfull edge devices. 
The dataset can be taken from Kaggle.
Performance of the model uses this metrics:
-	Loss and Accuracy
(loss: 0.0941 - accuracy: 0.9837 - val_loss: 0.1219 - val_accuracy: 0.9829 –> where we can se that are great results even on the validation loss and accuracy)

-	Classification report (Precision , Recall, F1-Score)
(average metrics of precision, recall and F1- Score are great : 0.98)
-	Confusion Matrix
(In confusion matrix we can see that results are very satisfying)

Final pipeline includes reading the image, grayscale conversion, edge detection, segmenting the digits and operators, bounding boxes extraction and preprocessing, making predictions, and displaying the results on the original image.

Project can be increased further by including more mathematical operators and symbols and making it more intelligent.

## Problems: 
Because the data from MNIST dataset is quite different then data taken from pictures, model can be significantly increased with more real world pictures and techniques like: Transfer Learning, Data Augmentation (Mirroring, Random Cropping, Rotation, Color Shifting, etc.).

## Instruction for using the application:
-	Take the picture with your mathematical expression on the blank paper, written very, very pretty.
-	Put it in the folder /data.
-	Run the last cell in Jupyter Notebook where the application calculate expression from picture, and put the correct path with the correct name of the picture.
-	See the result.
