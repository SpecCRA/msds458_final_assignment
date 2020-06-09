# EDA & Experimental Notes:

# Experimental Classifier Details:

1. Labels: sirna_id
2. input: images
3. isolate experiment and cell types too

# Problems

1. Featurewise centering not working. Meant to use with flow, not flow from dataframe
    * https://github.com/keras-team/keras/issues/3679

## Dataset notes

* Moving forward with already parsed dataset
    * filtered treatment only
    * train/test set was pre-labeled

* Testing on HUVEC cell types
    * Optimize for each cell type because they all look different

* Image data gen adding noise helped regularize accuracies 
* It did trail off after a while though

## Definitions

## Well type
1. negative control: not exposed to experimental treatment or any other treatment; expected to have NO EFFECT
2. positive control: not exposed to experimental treatment but exposed to something intended to CREATE INTENDED EFFECT
3. treatment: group that is not exposed to positive treatment but only experimental treatment

# References:

1. Tuning transfer learning
    * https://medium.com/starschema-blog/transfer-learning-the-dos-and-donts-165729d66625
2. Learning rate scheduler
    * https://machinelearningmastery.com/using-learning-rate-schedules-deep-learning-models-python-keras/
3. Different pre-trained layers
    * https://www.pyimagesearch.com/2017/03/20/imagenet-vggnet-resnet-inception-xception-keras/
4. Second place solution
    * https://www.kaggle.com/c/recursion-cellular-image-classification/discussion/110457
5. Image data generator
    * https://machinelearningmastery.com/how-to-configure-image-data-augmentation-when-training-deep-learning-neural-networks/
6. Adjusting learning rates through training
    * https://machinelearningmastery.com/using-learning-rate-schedules-deep-learning-models-python-keras/


# Questions

1. Pre-trained networks?
2. How to adjust?
3. Simplicity vs complexity?