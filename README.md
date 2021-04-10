# midas_task2

-----Subtask 1----

Preprocessing of images - Given images was of 1200x900 pixels resizing them into 28x28 size pixels as firstly it will make computing weights and updating them less computational expensive also this far outweighs the effects on accuracy due to this resizing as even after this model achieves accuracy of 96%, changed the images to grayscale.

Model building - Considered/experimented  2 models for comparing accuracy and found that it is essential to keep a dropout layer for preventing overfitting and the architecture should also have normal convolutional and pooling layers.

Training - Considered 80 epochs and 32 batch size after fine tuning to achieve the best results as it leads to more frequent model parameters updates.

-----Subtask 2 ------

The model using pretrained weights outperforms the one with randomly initialsed weights but only slightly. The convergence time is better the first converges much quickly than the latter also the final accuracy on the test set of pretrained model is better than randomly initialsed one by significant amount.

Errors in %
Pretrained - 0.77
Randomly 0 0.89

However the randomly initialsed model is much closer to the validation set finally than the one which is pretrained the reason being that we might have overfit the pretrained model due to the headstart of model parameters.

-----Subtask 3 ------

Labels were not given so randomly initialsed labels to introduce noise in the dataset, proceed in the direction of fine tuning the existing state of the art classification models on this training dataset to solve the classification problem
