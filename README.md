# Object Detection Hands
![image](https://user-images.githubusercontent.com/89865352/235805133-aa744d4b-3c66-4d65-b28d-8202678d9e3a.png)
![image](https://user-images.githubusercontent.com/89865352/235805147-48208717-572f-4b84-a6f0-7abe73e85021.png)
![image](https://user-images.githubusercontent.com/89865352/235805165-d1f1ef16-48c5-4a41-98b6-e41ea7a2483d.png)
## Purpose
For this project we trained a object detection model on 3 hand signals. Hello (wave), good (thumbs up), and small (pinch).
## Image Collection and Labelling
We collected images by webcam and labelled them using LabelImg, https://github.com/tzutalin/labelImg.
## Training
The model we used was ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8 from Tensorflow Model Zoo,https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md, which is part of the larger Tensorflow Object Detection API.
The data was transformed to TFrecords prior to training.
Using Tensorboard to visualize training, we can see that there was a downward sloping curve for the loss function, indicating successful training.
![image](https://user-images.githubusercontent.com/89865352/235806969-bc50a534-ed45-441a-aec9-ffca70e0787d.png)
## System
Everything was done locally on my own computer, using WSL, and training using GPU. Training took about 5 mins. 
