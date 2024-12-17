so i am writing this to explain my thought process for the project.

Title : facial recognition for emotion detection like sad, happy etc

so i started by downloading the fer2013 dataset - figuered out how to download the dataset from kaggle

- then started to experiment on the cnn model. finally found that this model has best accuracy.
- Initially i only kept the conv layers and maxpooling layers as i learnt only that but finally got to know that batch normalization again increase the generalization of the model.
- so i added that also
- added some dropout layers to prevent overfitting
- finally softmax to get the probabilities of what the image represents

## **Model Architecture**
The CNN model is designed with the following layers:

1. **Input**: 48x48 grayscale image
2. **Conv2D Layers**: For feature extraction
3. **Batch Normalization**: Normalize activations for stability
4. **MaxPooling**: Reduces spatial dimensions
5. **Dropout**: Reduces overfitting
6. **Dense Layers**: Fully connected layers for classification
7. **Softmax**: Outputs probabilities for 7 emotion classes

so the performance matrix for the project will be added soon. I am GPU Poor please understand and also colab Freetier GPU sucks.

- but i will just say what i got
- i got around 70 - 90 accuracy on the model
- i took a different stand to train the model, like instead of putting in epochs, i trained the model for 10 epochs again and again
- what it did was it improved the accuracy at the end of each cell execution even more faster, so this helped me getting a good accuracy 

i didnt do the productization - no timeeeee....
