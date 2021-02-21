# Loading data in python 

## Source:
Loading in your own data - Deep Learning basics with Python, TensorFlow and Keras p.2
by: sentdex
Link: https://youtu.be/j-3vuBynnOE

## Summary:
I have loaded images from the microsoft kaggle cats and dogs library.

## Libraries:
* os - miscellaneous OS interfaces
* numpy
* matplotlib
* cv2 - bindings for computer vision
* pickle - binary protocol for serializing and de-serializing a Python object structure


## Functions:
create_training_data(): A function that, for each image in each category, tries to read the image, resize it and append it to the training_data list. If an error is encountered, we skip to the next image. 

## Notes:
* We define the data directory and the categories
* We use os.path.join to get the path to each categories directory
* We load the images using cv2.imread, in the greyscale map
* We use cv2.resize so we can reduce the computing requirements
* We split the tuples in training_data into the common notations : X and y
* We get the transposed matrix representation using the np.array.reshape function
* We save our new data using pickle (we convert it into a byte stream)
