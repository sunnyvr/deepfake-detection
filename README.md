# deepfake-detection
## Description ##
This project intends to show how to use [Python](https://www.python.org/ "Python"), [Keras](https://keras.io/ "Keras"), and [TensorFlow](https://www.tensorflow.org/ "TensorFlow") to build a deep learning-based deepfake detection model from the ground up. The proposed deepfake detector is based on the state-of-the-art EfficientNet structure, with certain network layer tweaks, and the example models were trained on a large and diverse set of deepfake datasets.<br />
Face detection is carried out with the help of a [MTCNN face detector](https://github.com/ipazc/mtcnn "MTCNN face detector") for Keras. A list of JSON items is returned by the detector. The three primary keys in each JSON object are 'box, confidence, and keypoints'. <br />
### General Idea ###
Each video goes through a face detector which focuses on the facial features and draws a box around it and gathers around ~300 frames (face images) per video. This is then compressed down and resized from 1920x1080 to ~360x200 which significantly reduces filesize since there are around 3 million images gathered. These images are then classified if they're "*fake*" or "*real*" which are marked by the ***metadata.json*** file. Once these images are split up they're fed into a basic CNN deep learning algorithm which learns what are fake and what are real. After the model has been trained with different epochs, the test videos are fed into the model and predictions are made whether the videos are fake or not.
### DeepFake Dataset ###
* [Kaggle DeepFake Challenge](https://www.kaggle.com/c/deepfake-detection-challenge "Kaggle DeepFake Challenge") (471 GB)<br />
![picture alt](https://github.com/aaronchong888/DeepFake-Detect/raw/master/img/sample_dataset.png)

## Let's Begin! ##
### Prerequisites ###
* Python 3
* Keras
* TensorFlow
* OpenCV
* MTCNN
