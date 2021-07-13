# deepfake-detection
## Description ##
MSc Project on DeepFake video detection.<br /><br />
This project intends to show how to use [Python](https://www.python.org/ "Python"), [Keras](https://keras.io/ "Keras"), and [TensorFlow](https://www.tensorflow.org/ "TensorFlow") to build a deep learning-based deepfake detection model from the ground up. The proposed deepfake detector is based on the state-of-the-art EfficientNet structure, with certain network layer tweaks, and the example models were trained on a large and diverse set of deepfake datasets.<br />
Face detection is carried out with the help of a [MTCNN face detector](https://github.com/ipazc/mtcnn "MTCNN face detector") for Keras. A list of JSON items is returned by the detector. The three primary keys in each JSON object are 'box, confidence, and keypoints'. <br />
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
