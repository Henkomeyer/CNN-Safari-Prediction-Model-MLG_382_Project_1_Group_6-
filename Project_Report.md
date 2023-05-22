# MLG_382_Project_1_Group_6
Use what you've learned to train a convolutional neural network model that classifies images of animals you might find on a safari adventure
-
## Team Members 
-----
* ### Roan Palm: 578632
* ### Vuyo Fortune Mathe: 578376
* ### Henko Meyer: 578420
---
# CNN Model Training Summary

The Convolutional Neural Network model we trained is a sequential model named "sequential4". The model architecture is outlined as follows:

## Model Architecture

- Input layer: 32 6x6 convolution filters applied to the input image with Rectified Linear Unit (ReLU) activation function
- Max pooling layer with 2x2 patch reduces dimensionality to 16x16
- Second convolution layer: 64 6x6 filters
- Second max pooling layer reduces dimensionality to 8x8
- Third convolution layer: 128 6x6 filters
- Third max pooling layer reduces dimensionality to 4x4
- Dropout layer to reduce overfitting
- Flatten layer to convert the 2D matrix data to a vector
- Dense output layer with 10 units, one for each class

The model has a total of 392,810 parameters, all of which are trainable.

## Training Process

The model was trained for 10 epochs. The training loss started at 1.3872 and decreased to 0.0318 by the last epoch, indicating that the model was learning and improving its performance as training progressed. Similarly, the training accuracy improved from 0.3510 to 0.9899 over the 10 epochs.

Validation loss and accuracy were also recorded during the training process to monitor the model's performance on unseen data. The validation loss started at 1.2048 and decreased to 0.0003 by the last epoch. Similarly, the validation accuracy improved from 0.7500 to 1.0000 over the 10 epochs.

## Conclusion

The model showed excellent performance with the training accuracy reaching 98.99% and the validation accuracy reaching 100.00% after 10 epochs. This indicates that the model generalized well to unseen data and achieved a high level of accuracy. However, it is worth noting that the model might be overfitting the training data since the training accuracy is higher than the validation accuracy.

Please find below the model performance plot:

![Model Performance Plot](https://cdn.discordapp.com/attachments/543906136861179925/1109997556500545656/image.png)

!![Model Performance Plot 2](https://github.com/Henkomeyer/MLG_382_Project_1_Group_6/assets/84342604/1d6eaa60-2eb2-4c7c-91f6-957f3c3c49f1)


Dataset Information:
- Training images: 396 images belonging to 4 classes.
- Test images: 4 images belonging to 4 classes.
