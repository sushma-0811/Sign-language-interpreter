Sign Language Interpreter using Deep Learning
You can view the project demo on [YouTube](https://youtu.be/cg_wbt4KTiE?si=MqPauQISvAqnGHLx).

**Table of contents**
General info
Demo
Technologies and Tools
Setup
Process
Code Examples
Features
Status
Contact
General info


**Demo**

The entire demo of the project can be found on https://youtu.be/cg_wbt4KTiE?si=MqPauQISvAqnGHLx.


**Technologies and Tools**
Python
TensorFlow
Keras
OpenCV
Setup
Use comand promt to setup environment by using install_packages.txt and install_packages_gpu.txt files.

**python -m pip install -r install_packages.txt**


This will help you in installing all the libraries required for the project.

**Process**


Run set_hand_histogram.py to set the hand histogram for creating gestures.
Once you get a good histogram, save it in the code folder, or you can use the histogram created by us that can be found here.
Added gestures and label them using OpenCV which uses webcam feed. by running create_gestures.py and stores them in a database. Alternately, you can use the gestures created by us here.
Add different variations to the captured gestures by flipping all the images by using Rotate_images.py.
Run load_images.py to split all the captured gestures into training, validation and test set.
To view all the gestures, run display_gestures.py .
Train the model using Keras by running cnn_model_train.py.
Run final.py. This will open up the gesture recognition window which will use your webcam to interpret the trained American Sign Language gestures.


**Features**


Our model was able to predict the 44 characters in the ASL with a prediction accuracy >95%.

Features that can be added:
Deploy the project on cloud and create an API for using it.
Increase the vocabulary of our model
Incorporate feedback mechanism to make the model more robust
Add more sign languages
Status
**Project is: finished. **
