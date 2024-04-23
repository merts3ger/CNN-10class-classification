# CNN-10class-classification 
This project is dedicated to developing and training three subsequently enhanced CNN models to observe the impact of different architectures on image classification performance.     
The models are trained on [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) consisting of 60,000 images distributed across 10 classes.     
    
* For the pre-processing step, the images were converted into PyTorch tensors and their pixel values were normalized.     
* The first model is composed of convolutional layers for initial feature detection and pooling layers for dimensionality reduction, followed by dense layers for output classification. Next model modifies and extends this design by more output channels and a smaller kernel for finer feature detection. It also incorporates dropout layers to mitigate overfitting. For the last model, an extra convolutional layer is added along with batch normalization to stabilize learning.     
* The models' training progress is reported and also visualized through loss dynamics plots.      
* *Early Stopping* technique is implemented to stop the training process if there's no improvement in a model's loss over a certain number of epochs (defined by *patience*).         

Based on the evaluation of the models on the test data, a consistent improvement in performance was observed across the versions, increasing from an initial accuracy of 62% with the basic model to 79% accuracy with the third model, marking a 17% improvement.     

*While not part of this experiment design, incorporating data augmentation techniques and a systematic search for optimal hyperparameters would be an interesting direction for a subsequent project, as well as advancing further the final architecture.
