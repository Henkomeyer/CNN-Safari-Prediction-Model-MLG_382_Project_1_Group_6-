# MLG_382_Project_1_Group_6
### Task: 
Use what you've learned to train a convolutional neural network model that classifies images of animals you might find on a safari adventure.
# CNN Model Training Summary

The Convolutional Neural Network model we trained is a sequential model named "sequential4". The model architecture is outlined as follows:

## Model Architecture

* Input layer: 32 6x6 convolution filters applied to the input image with Rectified Linear Unit (ReLU) activation function
* Max pooling layer with 2x2 patch reduces dimensionality to 16x16
* Second convolution layer: 64 6x6 filters
* Second max pooling layer reduces dimensionality to 8x8
* Third convolution layer: 128 6x6 filters
* Third max pooling layer reduces dimensionality to 4x4
* Dropout layer to reduce overfitting
* Flatten layer to convert the 2D matrix data to a vector
* Dense output layer with 10 units, one for each class

The model has a total of 392,810 parameters, all of which are trainable.

## Training Process

The model was trained for 10 epochs. The training loss started at 1.5732 and decreased to 0.6765 by the last epoch, indicating that the model was learning and improving its performance as training progressed. Similarly, the training accuracy improved from 0.4250 to 0.7607 over the 10 epochs.

Validation loss and accuracy were also recorded during the training process to monitor the model's performance on unseen data. The validation loss started at 1.2427 and decreased to 0.8608 by the last epoch. Similarly, the validation accuracy improved from 0.5526 to 0.7103 over the 10 epochs.

## Conclusion

The model showed satisfactory performance with the training accuracy reaching 76.07% and the validation accuracy reaching 71.03% after 10 epochs. This indicates that the model generalized well to unseen data. However, there is some evidence of overfitting since the training accuracy is higher than the validation accuracy.

Please find below the model performance plot:
![Model Performance Plot](https://media.discordapp.net/attachments/543906136861179925/1109814196784353300/download.png?width=435&height=468)

Further improvements might be achieved by tweaking the model architecture, using regularization techniques, or applying data augmentation.
