# Custom_Object_Detection_tensorflow

- We are going to create a Deep Learning model using Tensorflow which can be trained to detect custom Object.
- We use Transfer Learning method.
- The Base Model we use is SSD MobileNet V2 FPNLite 320x320.
- The Base Model is available in Tensorflow Model Garden [TF_MODEL_GARDEN](https://github.com/tensorflow/models "TF_MODEL_GARDEN")

## Prerequisite
- Python 3
- Tensorflow
- Anaconda or mini-conda
- Jupyter Notebook

## Info
- The Over-all Steps are divided into two jupyter notebook
- The first notebook(Image Collection.ipynb) contains all the code which is used to collect the data for training and testing and image labeling.
- The second notebook(model.ipynb) contains all the code which deals with model creation/tweaking , evaluation and prediction.

## Image Collection.ipynb
In this notebook we setup our starting folders and collect the data which we will use for model training and testing and also label the image using [LabelImg](https://github.com/tzutalin/labelImg "LabelImg").

## model.ipynb
- In this notebook we first download and install the tensorflow object detection api from the tensorflow model garden.
- Then we create a label map for our model.
- Then we create Tfrecords using [GenerateTFRecord](https://github.com/nicknochnack/GenerateTFRecord "GenerateTFRecord").
- Now we import pipeline config file from the api folder and update it according to our custom objects/labels.
- Now we train and Evaluate our model .
