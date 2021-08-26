# vehicle-model-detection-using-yolov3-on-Raspberry-Pi
vehicle model detection using yolov3 on Raspberry Pi

## Overall Discrption
I previously impelement a project in computer vision to recognize vehicle model with YOLOv3 [link](https://github.com/behnoudshafizadeh/vehicle-Recognition-using-deep-learning-algorithm-). as a result, we compelet this by doing that on raspberry Pi module. 
(Notice : the requirement of this project is similar to this [link](https://github.com/behnoudshafizadeh/License-Plate-Detection-using-Raspberry-PI-YOLOV3-) on raspberry Pi)

## Structure of main folder
```
input directory : input images
output directory : the results of the algorithm
utils directory : packages and fuctions used in yolov3 algorithms
converted.weights : weights for model recognition (trained before)
detect.py : main code using yolov3 structure for detecting objects
models.py : the structure of yolov3 neural network (activatation fuction, upsampling function, ...)
objecttomodels.names : the labels in this project (different kind of vehicle models)
yolov3-35clstomodels.cfg : configuration file for designing the layers in vehicle yolov3 neural network
```
![model](https://user-images.githubusercontent.com/53394692/130983449-e865f27d-bf88-4cc9-ba37-97311f0b94c9.png)

## Test
for running and testing the algorithms, we use following instruction :
```
python3 detect.py --source input --weights converted.weights --cfg yolov3-35clstomodels.cfg --names objecttomodels.names --img-size 416
```
and see results in `output` directory, such as below :

|                        output                                       |     
| ------------------------------------------------------------------- | 
| ![vehcle detection-2](https://user-images.githubusercontent.com/53394692/130984060-3676d426-1a2a-491e-b783-90c8edf30a6c.png)  |
| ![vehicle detection-1](https://user-images.githubusercontent.com/53394692/130984114-b8e412a8-2fdc-49b1-8764-f188a20758d8.png) |
| ![vehicle detection-5](https://user-images.githubusercontent.com/53394692/130984159-a51f40e7-5d5e-4363-b2f0-13c9799a43a5.png) |
| ![vehicle detection-3](https://user-images.githubusercontent.com/53394692/130984370-394838a2-7914-46c7-9b95-d3aaa4fc6e19.png) |
| ![vehicle detection-4](https://user-images.githubusercontent.com/53394692/130984450-369de9a8-1134-42df-9b3c-dc15b1472efb.png) |
| ![vehicle detection-6](https://user-images.githubusercontent.com/53394692/130984507-ca3ce12e-3d33-4f2f-8ca4-17d6a2e6b2b0.png) |





























