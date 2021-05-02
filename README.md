# GazeML_torch
Reproduction of https://github.com/swook/GazeML (paper: https://arxiv.org/abs/1805.04771v1) by PyTorch.

## Requirement
```
pytorch
tensorboard
numpy
opencv
imutils
dlib
scipy
```

## Example
![GazeML_torch_v0.2_jun1](https://imgtu.com/i/ger3Oe)

![GazeML_torch_v0.2_jiabin](https://imgtu.com/i/cXfwhn)

![GazeML_torch_v0.2_jun2](https://imgtu.com/i/ger3Oe)

## Webcam Demo
```
python demo_webcam.py
```
dlib models: https://github.com/davisking/dlib-models

I use dlib mmod_human_face_detector to detect face region.

Then, i use dlib shape_predictor_5_landmarks to get eye landmarks for clippling eye region.

After that, i use the model_based model from https://arxiv.org/abs/1805.04771v1 to estimate Gaze.
