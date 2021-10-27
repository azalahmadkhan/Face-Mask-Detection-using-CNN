# Face-Mask-Detection-using-CNN

### Dataset
I used kaggle dataset of 10,000 images (5,000 masked and 5,000 unmasked) and split it into 80:20 ratio for training and testing purpose.
Link to dataset: https://www.kaggle.com/ashishjangra27/face-mask-12k-images-dataset

### IDE 
I used google colab to train this CNN.

### CNN

Since dataset consists of RGB images therefore its pixels were in 0-255 range.
First layer in the model scaled those values to 0-1 range.

#### Model
input--->Conv2D+ReLU--->MaxPool--->Conv2D+ReLU--->MaxPool--->Conv2D+ReLU--->MaxPool--->Dropout--->Flatten--->Fully Connected--->Fully Connected--->output

Dropout layer was inserted to avoid overfitting.

### Optimizer
Adams optimizer is used in the model because it gives much higher performance with deep learning models.

### Accuracy Scores 
accuracy: 0.9990 
loss: 0.0028
val_accuracy: 0.9995
val_loss: 0.0026 

Therefore we can say that model has 99.95% accuracy in unknown models.
