# Data Preparation & Processing for CRF-Net
The Camera-Radar Fusion Network (CRF-Net) [2] is one of the few papers that have utilised the rich Nuscenes datasets [1]. The main reason for selecting this dataset is its vast variety of data using camera, radar and even LiDar and also acquried from different locations, say from front of the car to the back of th car. As the data is rich, it also requires some preparations and processing to be done. This repository here is meant for the segregation of the datasets. 

The Complete Nuscenes Datasets can be downloaded from the following website: 
> https://www.nuscenes.org/nuscenes

The Full Dataset (v1.0) part of 'trainval' are the set of files that are to be downloaded. Note that the entire size of the datasets is as high as 400gb. 
The files from 'part1' to 'part10' contains all the data from different sensors ;

For Radars, 
> RADAR_FRONT_RIGHT , RADAR_FRONT_LEFT , RADAR_FRONT , RADAR_BACK_RIGHT, RADAR_BACK_LEFT (Total: 5 folders)

For Cameras, 
> CAM_FRONT , CAM_FRONT_RIGHT , CAM_FRONT_LEFT , CAM_BACK , CAM_BACK_RIGHT , CAM_BACK_LEFT (Total: 6 folders)

For Lidar, 
>LIDAR_TOP (Total: 1 folder)

All the files in the above subfolders should be contatenated into a single folder of the same name. A naive method is to manually copy all the contents to a common folder but at a cost of time. So, the effective way is to write a small piece of code which can finish the work in a jiffy ! 

The code is being written in Jupyter notebook, running each of the cell, with by substituting the path of the datasets should be sufficient !! 



[1] Holger Caesar et al. “nuscenes: A multimodal dataset for autonomous driving”. In: Proceedings of the IEEE/CVF conference on computer vision and pattern recognition. 2020,pp. 11621–11631.

[2] Felix Nobis et al. “A deep learning-based radar and camera sensor fusion architecture for object detection”. In: 2019 Sensor Data Fusion: Trends, Solutions, Applications (SDF). IEEE. 2019, pp. 1–7
