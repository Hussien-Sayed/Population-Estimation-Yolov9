# Population-Estimation-Yolov9
## Introduction
This is a challenge hosted on zindi platform that aims to helping people of Malawi to optimally deal with climatic disasters like floods,droughts and landslides. By designing an ML algorithm and utilizing satellite images, an estimation of the population in different areas can be made, thus Allowing more effective evacuation and aid delivery and helps improving response time to these disasters.

To estimate population, counting of different dwellings is performed using an ML model. The possible types are :
* Tin
* Thatch
* Other

## Used Model
An object detection YOLOv9 model is used to detect bounding boxes of different types of dwelling, then the results are used to produce a couning for each type. After some exploration of the errors made by the model, a possible improvement was to remove on-edge detections as these were mostly false positives.

## Evaluation
The model had a mAP.5 of 0.58 and a MAE of 0.42.
After the modification the MAE was reduced to 0.33.


