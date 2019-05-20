# Week 4 Assignment

In this assignment, we had to create 4 different notebooks with our understanding on CNN. 

The goal was to reach 99.4 validation accuracy with parameters less than 15k. The dataset on which we were supposed to work on was [MNIST Handwritten Dataset](<http://yann.lecun.com/exdb/mnist/>). 
Each code was a development from the previous code. The first code file was supposed to be a Vanilla code, that means we could not use extra features. 

Below, I've explained how I have proceeded from the first code file to the fourth code file. Also, I've listed the number of parameters and the max accuracy achieved under each code. The training accuracy and the validation accuracy listed are at the epoch at which I've got the highest validation accuracy.



### Code 1

In the first code block, there was no limit on the number of parameters which we could have but the only condition we had was that the architecture of the model had to be a vanilla model. The only additions we could use were the 1x1 and Max Pooling.

**Number of trainable parameters:** 58,538

**Training Accuracy:** 99.58% 

**Validation Accuracy:** 99.22%



### Code 2

In the second code file, the changes made in the model architecture are: Adding Batch Normalization Layers, Changing the number of channels and changing the batch size. These are the three improvements in the second code file. 

**Number of trainable parameters:** 15,586

**Training Accuracy:** 99.60% 

**Validation Accuracy:** 99.30%



### Code 3

In the third code file, the changes made are: Addition of Dropout, Changing the Optimizer from Adam to SGD and Changing the learning rate. 

**Number of trainable parameters:** 11,530

**Training Accuracy:** 97.30% 

**Validation Accuracy:** 97.01%



### Code 4

In the fourth code file, the changes made are: Addition of Dropout layer after each Batch Normalization Layer, Adding callbacks and changing the kernel size.

**Number of trainable parameters:** 11,516

**Training Accuracy:** 97.40% 

**Validation Accuracy:** 99.40%