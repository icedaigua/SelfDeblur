# Self-supervised Linear Motion Deblurring

This repository contains the code to reproduce the results from the paper "Self-supervised Linear Motion Deblurring"

We present a differentiable reblur model for self-supervised motion deblurring. We are able to train the networks
with two consecutive blurry images and do not require any ground truth sharp image for supervision. During inference,
our network takes a single blurry image as an input and procude the corresponding sharp estimate, as in the example:
<img src="demo/demo_fastec.gif" height="250px"/> <img src="demo/demo_real.gif" height="250px"/>

You can find detailed usage instructions for training your own models and using pretrained models below.

If you find our code or paper useful, please consider citing:
```
@article{LiuRAS2020,
  author = {Peidong Liu and Joel Janai and Marc Pollefeys and Torsten Sattler and Andreas Geiger},
  title = {Self-supervised Linear Motion Deblurring},
  journal = {Robotics and Automation Letters},
  year = {2020}
}
```

## Dependencies installation
To train or test the model, you need to install the dependent packages via
```
pip install -r requirements.txt
```
The code is tested with PyTorch 0.4.0 and 1.1.0 with CUDA 9.0.

#### Install correlation package
```
cd ./correlation_package
python setup.py install
```

#### Install reblur_package
```
cd ./reblur_package
python setup.py install
```

## Demo with our pretrained model

## Datasets
In this work, we proposed two new datasets. The synthetic dataset
(i.e., Fastec dataset) is synthesized with a high speed global
shutter camera (~1200 FPS). The camera is mounted on a ground vehicle.

## Evaluation with our pretrained model

## Training with our datasets

## Training with your own dataset

