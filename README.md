# retinopathy_image_recognition
A first foray into image processing and recognition, using Kaggle's retinopathy dataset. 

# augmentation:
Tried a number of image augmentation and downsampling/upsampling techniques to try to get the models to generalize better and more effective distinguish among all 5 class labels. Result were...ok, but beg the question of whether I employed too many image augmentation techniques (I used four). On a subsequent attempt, I would probably start with only greyscale images and perhaps 2 basically augmentation techniques (e.g. flip and sharpen). Regardless, more experimentation necessary. 

# models:
The CNN pretrained with VGG16 base using early stopping certainly performs the best, though we could certainly try different, more complex architectures with more time. 

XGBoost did not perform well, though I could have done more to regularize and tune other hyperparameters. 

Perhaps unsurprisingly, the SVM was insanely computationally inefficient, but I thought I would try it out regardless with a few different hyperparameters.

# computation:
Courtsey of the GPUs on UChicago's cloud environment. 
