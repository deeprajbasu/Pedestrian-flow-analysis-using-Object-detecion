#      Pedestrian / Commuter flow analysis with Object Detection


###### To do
> analyse movement of detected pedestrians to classify them as 'incoming' or 'outgoing'

> try to use a better detector such as yolo or retina net


> display number of people present 


> use [Unsupervised Segmentation using MASON](https://github.com/JosephKJ/MASON) to retrain with cleaner dataset

> use a more sophisticated tracking method to reduce errors while tracking

    
    
    

<p align="left">  
<img src="https://raw.githubusercontent.com/deeprajbasu/Pedestrian-flow-analysis-using-Object-detecion/master/3.gif" width="45%" align='left'>
<img src="https://raw.githubusercontent.com/deeprajbasu/Pedestrian-flow-analysis-using-Object-detecion/master/2.gif" width="45%" align="left" >       
<img src="https://raw.githubusercontent.com/deeprajbasu/Pedestrian-flow-analysis-using-Object-detecion/master/1.gif" width="45%" align="left" >   
<img src="https://raw.githubusercontent.com/deeprajbasu/Pedestrian-flow-analysis-using-Object-detecion/master/4.gif" width="45%" align='left'>
</p>




## Dataset

[Stanford Drone Dataset](https://cvgl.stanford.edu/projects/uav_data/) dataset is used for training my pedestrian detector.
[Dataset UTILS](https://github.com/JosephKJ/SDD-Utils) used for processing the raw dataset for creating tf-records for training 

## Training

[ssd_resnet_50_fpn_coco](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf1_detection_zoo.md) model was used from Tensorflow object Detection api for transfer learning 

## Object Tracking 
[simple centroid tracking](https://www.pyimagesearch.com/2018/07/23/simple-object-tracking-with-opencv/) Technique from PyImageSearch was implemented in this project to work with the detections 



<p align="left">  
<img src="https://raw.githubusercontent.com/deeprajbasu/Pedestrian-flow-analysis-using-Object-detecion/master/Optflow.gif" width="45%" align='left'>
</p>

## Optical Flow
optical flow output.
perhaps quality of detections can be improved by detected on optical flow features instead of raw data, 
