# Video Classification: Facial Expression Detection

Learning to recognize a person's facial expressions on a video takes two steps.  The first step is object detection.  The algorithm should be able to see a video and and be able to recognize a person's face. The object detection section of the algorithm is done with the Open CV (Computer Vision) library from Python.

After the face is detected, the algorithm uses a CNN model to classify the person's facial expression.

## Data

The dataset used was from the Kaggle facial expression recognition competition, which can be found [here](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data). It contains over 35,000 images, with each one classified with one of the following 7 emotions: (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).

## Models
The Pytorch model uses a ResNet 50 architecture with transfer learning.  The Keras model uses a simple 4-layer convolutional neural network (CNN) architecture.  The accuracy of both models is roughly the same (around 40%), but when we use the OpenCV library to detect and capture human faces, the algorithm becomes very accurate as you can see see by images of the video captures below.

## Results
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/happy.png" width="360" />
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/surprised.png" width="360" />
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/sad.png" width="360" />
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/scared.png" width="360" />
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/angry.png" width="360" />
<img src="https://github.com/mlsmall/Facial-Expression-Detection/blob/master/Expressions/neutral.png" width="360" />


## References

The following sources were used to help create the models in this repo:

https://github.com/omar178/Emotion-recognition
https://github.com/MauryaRitesh/Facial-Expression-Detection-V2

