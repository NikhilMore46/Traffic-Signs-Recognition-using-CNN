# Traffic-Signs-Recognition-using-CNN

# Introduction
When you go on the road, you see various traffic signs like traffic signals, turn left or right, speed limits, no passing of heavy vehicles, no entry, children crossing, etc., that you need to follow for a safe drive. Likewise, autonomous vehicles also have to interpret these signs and make decisions to achieve accuracy. The methodology of recognizing which class a traffic sign belongs to is called Traffic signs classification.

In this Deep Learning project, we will build a model for the classification of traffic signs available in the image into many categories using a convolutional neural network(CNN) and Keras library.

# Dataset for Traffic Sign Recognition
The image dataset is consists of more than 50,000 pictures of various traffic signs(speed limit, crossing, traffic signals, etc.) Around 43 different classes are present in the dataset for image classification. The dataset classes vary in size like some class has very few images while others have a vast number of images. The dataset doesn’t take much time and space to download as the file size is around 314.36 MB. It contains two separate folders, train and test, where the train folder is consists of classes, and every category contains various images.

# GUI for Traffic Signs Classifier
We will use a standard python library called Tkinter to build a graphical user interface(GUI) for our traffic signs recognizer. We need to create a separate python file named” gui.py” for this purpose. Firstly, we need to load our trained model ‘traffic_classifier.h5’ with the Keras library’s help of the deep learning technique. After that, we build the GUI to upload images and a classifier button to determine which class our image belongs. We create classify() function for this purpose; whence we click on the GUI button, this function is called implicitly. To predict the traffic sign, we need to provide the same resolutions of shape we used at the model training time. So, in the classify() method, we convert the image into the dimension of shape (1 * 30 * 30 * 3). The model.predict_classes(image) function is used for image prediction, it returns the class number(0-42) for every image. Then, we can extract the information from the dictionary using this class number.

# Conclusion
In this article, we created a CNN model to identify traffic signs and classify them with 95% accuracy. We had observed the accuracy and loss changes over a large dataset. GUI of this model makes it easy to understand how signs are classified into several classes.
