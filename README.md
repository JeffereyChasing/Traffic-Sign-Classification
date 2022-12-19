# Traffic-Sign-Classification

## Description of Project

1. Goal:
The objective of this project is to test and compare different CNN model architectures’ robustness in identifying different types of Graffitied traffic signs.

2. Motivation:
Within the skyrocketing industry of self-driving smart car, safety has always been an essential concern that all car manufacturer and innovator need to address while updating vehicle’s other attributes such as speed and energy consumption.  In this topic, abiding to the traffic signs is a significant component. However, in real life, some of the traffic signs are often damaged or doodled; therefore, it’s vital for all self-driving vehicles to be able to identify traffic signs robustly and consistently.

3. Benefit:
This project would not find out the most efficient models in classifying traffic signs but also indicates the most robust model against the unrelated feature information

## Description of Repository

1. Dataset Link: https://drive.google.com/file/d/1ZAjCtX0_zZ-qmmMSxxeCfIvp8IXD5ibd/view?usp=sharing
2. Modified Dataset Link: https://drive.google.com/file/d/19tspbi0lvCZHIUcfXe6hC_giNp10wHjJ/view?usp=sharing
3. image_change.ipynb: The code to modify the dataset
4. labels.csv: label classes
5. 

## Code Structure

## Example Commands of Code Execution

## Results


## Observations

1.  Accuracy:
* Compare LeNet-5, ResNet-50, VGG-16, and InceptionV3’s model accuracy in classifying various traffic signs on the traffic Sign Dataset to select the best model.
* InceptionV3 > VGG16 > LeNet5 > ResNet50


2. Robustness Against Graffitied Traffic Signs:
* LeNet5 > InceptionV3 > VGG16 > ResNet50 
* The validation accuracy of the models decreased when tested on the modified validation set compared to the original validation set. This decrease in accuracy indicates that the models are less effective at classifying the modified traffic signs than the original traffic signs. But it is worth noting that the decrease in validation accuracy was relatively small for some of the models, particularly VGG-16 and Inception-V3, which still achieved relatively high accuracy on the modified validation set. This suggests that these models may be more robust to changes in the training data than the other models.

3. Transferability:
* (LeNet5 and Inception-V3) ↑ 
* (ResNet50 and VGG-16) ↓
* When using transfer learning to fine-tune the models on the modified training set, the validation accuracy increased for some models (LeNet5 and Inception-V3) and decreased for others (ResNet50 and VGG-16). Overall, these results suggest that the effectiveness of transfer learning can vary depending on the specific model and the task at hand. In this case, transfer learning was able to improve the performance of some models on the modified validation set, but had a negative effect on the performance of others. It's important to carefully consider the capabilities and limitations of different models when choosing a model for a specific task and to carefully evaluate their performance on the relevant data.
