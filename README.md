# Facial-Expression-Recognition-using-Keras

# Description
In this project we are presenting the real time facial expression recognition of seven most basic human expressions: ANGER, DISGUST, FEAR, HAPPY, NEUTRAL SAD, SURPRISE.
This model can be used for prediction of expressions of both real time video of the user via webcam or any downloaded video. However, in both the cases we have to provide video to the model. In case of real time video the image should be taken at any point in time and feed it to the model for prediction of expression. The system automatically detects face using HAAR cascade then its crops it and resize the image to a specific size and give it to the model for prediction. The model will generate seven probability values corresponding to seven expressions. The highest probability value to the corresponding expression will be the predicted expression for that image.

# Dataset
https://www.kaggle.com/deadskull7/fer2013

# How to run the model

After downloading data from the aforementioned sources you have to structure the data into separate folders corresponding to the seven class labels. Then you can use the code in the file "Facial_Expression_Training.ipynb" to train the model.Then for the real time prediction you can run the file "main.py" and go to the web browser and type "0.0.0.0:5000" to see the video feed.<br/>
You can add the path of any video you would like to test in the 'camera.py' file- "self.video = cv2.VideoCapture('Desktop/Project/videos/facial_exp.mkv')"<br/>
If you want to use the webcam you can simply change the code in 'camera.py' file- "self.video = cv2.VideoCapture(0)"<br/>

# Prerequisites

You need to have installed following softwares and libraries in your machine before running this project.

Python 3<br/>
Anaconda: It will install ipython notebook and most of the libraries which are needed like seaborn, matplotlib, numpy, PIL.<br/>
OpenCV<br/>
Tensorflow<br/>
Keras<br/>

# Built With

ipython-notebook - Python Text Editor.<br/>
OpenCV - It is used for processing images.<br/>
Keras - Deep Learning Library.<br/>
Tensorflow - It is used for machine learning applications.<br/>
Matplotlib: It is a plotting library for Python and is used to plot graphs for accuracy and loss per epoch.

