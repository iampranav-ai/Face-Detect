# Face Detection using OpenCV & Python

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/organization/repository)
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)

First of all make sure you have OpenCV installed. You can install it using pip: `pip install opencv-python`.

Face detection using Haar cascades is a machine learning based approach where a cascade function is trained with a set of input data. 
OpenCV already contains many pre-trained classifiers for face, eyes, smiles, etc.. 

In this project I am using the face classifier. You can experiment with other classifiers as well.

You need to download the trained classifier XML file (haarcascade_frontalface_default.xml), which is available in OpenCV’s GitHub repository (https://github.com/opencv/opencv/tree/master/data/haarcascades). It is also available in this project. Save it to your working location.

## A few things to note:

The detection works only on grayscale images. So it is important to convert the color image to grayscale. (line 12)

Faces contains a list of coordinates for the rectangular regions where faces were found. We use these coordinates to draw the rectangles in our image.

Similarly, we can detect faces in videos. As you know videos are basically made up of frames, which are still images. So we perform the face detection for each frame in a video.

Hope you found this useful.
