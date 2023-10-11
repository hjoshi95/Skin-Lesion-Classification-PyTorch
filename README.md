# Skin-Lesion-Classification-PyTorch


I've tried to tackle this problem by using augmentor (https://augmentor.readthedocs.io/en/stable/) 
since there was a class imbalance in the dataset (https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic).

I apply augmentor on the train set and split that into the train and val set by not touching the test set. However, I believe that this has caused a distribution difference in the _new_ train-val
and the original given 'Test'set

In addition, I've trained this network on a resnet18 backbone using imagenet weights and statistics. Moreover, despite using augmentor to balance the class, 
I have also applied augmentation techniques and other _different_ image transformations to account for some techniques to make training more robust. 
The network seems to be a bit jerky at first but then tries to converge however, on the test set it performs a bit poorly atleast for a few classes. Seems like a classical case of overfitting 
but I am still thinking of ways to experimentally improve on this so would love some suggestions and feedback.

I hope this notebook provides you with some value :) 



