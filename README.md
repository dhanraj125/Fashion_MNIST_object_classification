# Fashion MNIST object classification

The objective of this case study is the object classification using Fashion MNIST Dataset which contain 60000 instances. For object classification two deep learning algorithms have been used, basic ANN (Artificial Neural Network) and CNN (Convolutional Neural Network. By using CNN we have got 97% training accuracy while 92% of testing accuracy.




## Dataset

Fashion-MNIST is a dataset of clothing images. Each example is a 28x28 grayscale image, associated with a label from 10 classes. The 10 classes represent different types of clothing, such as T-shirt/top, trouser, pullover, dress, coat, sandal, shirt, sneaker, bag, and ankle boot.



## Methods

Two neural network algorithms have been used for this work, ANN and CNN. Hyperparameter tuning have performed for the the hyperparameters of ANN algorithms. for image classifcation CNN have performed better than the ANN.



## Hyperparameter tuning

For hyperparameter tuning RandomizedSearchCV from sklearn is used. Hyperparameters such as number of layers, number of hidden layers, learning rate, epoches, and batch size are tuned from the sequential ANN. 



## Training 

![training and validation accuracy](https://github.com/dhanraj125/mnist_object_detection/blob/main/plots/hyperparameter_tuning.PNG)

The above figure shows the traning and validation accuracy by using different methods such as dropout, Batch normalization. First run is the default run without batch normalization and dropout, second run is by using only batch normallization, dropout run is by using dropout of 20%, and the last run is the run using both batch normalization and dropout of 20%.

## Evaluation

### sequential ANN accuracy

![ANN](https://github.com/dhanraj125/mnist_object_detection/blob/main/plots/ANN.png)

This graph shows the training and validation accuracy per the epochs. This run uses both batch normalization and 20% dropout



![CNN](https://github.com/dhanraj125/mnist_object_detection/blob/main/plots/cnn.png)

This graph shows the training and validation accuracy per epochs. This is a run of final CNN algorithm.


The highest accuracy is got by using CNN algorithm. The final training accuracy got is 97% and validation accuracy got is 92%.

> Final Accuracy achieved= 86.15%
