
# ECE-GY 7123 Introduction to Deep Learning Mini-Project

In this mini-project you are tasked with coming up with a modified residual
network (ResNet) architecture with the highest test accuracy on the CIFAR10 image classification dataset, under the constraint that your model has no
more than 5 million parameters.





## team members
1. Ankur Aggarwal (aa10336)
2. Anupam Tiwari (ast9885)


## Abstract
Abstract
Residual Networks (ResNets) are widely employed in image classification tasks. In this project, we developed and trained a customized ResNet model for CIFAR-10 image classification, focusing on maximizing test accuracy while keeping the model size within a fixed budget of 5 million trainable parameters. Model size, often measured by the number of trainable parameters, is crucial when deploying models on devices with limited storage capacity, such as IoT or edge devices.

In this report, we introduce our innovative residual network design, which contains less than 5 million parameters. Our ResNet model achieves a remarkable test accuracy of 85.39% on the CIFAR-10 benchmark when combined with appropriate training strategies and hyperparameters. The models and code can be accessed in this repo

## Set-up 
run the main.ipynb to reproduce the results 



## Description of files in the repository 
- main.py : code to train and test ResNet architectures 
- plots: graphs
- report: detail report 

## Accuracy
| Model             | Acc.        |
| ----------------- | ----------- |
| Our Model         | 85.36%      |


# Hyperparameters in our final model's architecture 

| Parameter                    | Our Model       |
| ---------------------------- | --------------- |
|number of residual layers     |3                |
|number of residual blocks | [4, 4, 3]| 
|convolutional kernel sizes |[3, 3, 3] |
|shortcut kernel sizes |[1, 1, 1] |
|number of channels |64 |
|average pool kernel size |8|
|batch normalization |True |
|dropout |0 |
|squeeze and excitation |True|
|gradient clip |0.1|
|data augmentation |True|
|data normalization |True|
|lookahead |True |
|optimizer |SGD|
|learning rate (lr)| 0.1|
|lr scheduler |CosineAnnealingLR|
|weight decay |0.0005|
|batch size |128 |
|number of workers |16|
|Total number of Parameters| 4,697,742|

## System Specification
Python Version: >3.9
PyTorch Version: 1.0+



