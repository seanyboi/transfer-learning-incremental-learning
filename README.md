# Transfer Learning (Incremental Learning)

### STEP 1

Create the config file for common variables to be used.

### STEP 2

Divide the dataset into the format that Keras accepts

### STEP 3

Take the dataset and divide them into batches. Once divided into batches the images are then preprocessed and ran through the ResNet-50 network pre trained on ImageNet to extract features. Labels are encoded and the appropriate label is placed into a row along with the feature vector for the image.

### STEP 4

A Keras ImageDataGenerator  object that is used to apply data augmentation, randomly translating, rotating, resizing, etc. images on the fly. The reason for doing so is to reduce overfitting. Data Generators are used because we are assuming that all the data cannot fit into memory.

Firstly we yield batches of labels + data to the network so it can be trained. Classification algorithm using Neural Networks.


Dataset can be found here: https://mmspg.epfl.ch/downloads/food-image-datasets/
