# chest x-rays
Identifying pneumonia using chest x-rays and deep learning (mobilenet)

## Objective
Find a deep learning model that can predict, with the reasonable accuracy, if a patient has pneumonia or not, based on his or her x-ray image.


## Dataset
[Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

- 5,863 images, 2 categories


Reference study: https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5


## Configurations evaluated
1. Convolutional Neural Network (CNN) with 4 conv layers and 2 fully connected layers
2. InceptionV3 pre-trained model 
3. Xception pre-trained model 
4. MobileNet pre-trained model (transfer learning)
5. MobileNet (pre fully train followed by fine tuning)


## Best results achieved
- Validation Accuracy       => 0.952


## Best model
The configuration that produced the best accuracy was:

- MobileNet fully training, and then finetuning
- batch size = 32
- epochs = 100 pre-training, additional 30 for fine tuning


Please check the code for hyperparameter values (file cxrays_mobilenet_finetune.ipynb)
