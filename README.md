# Classification-of-Bowling-Action-using-Pose-Estimation


This project introduces a novel method of using Pose Estimation to classify a legal bowling action in the sport Cricket.

This work utilizes a Spatial Temporal Transformer with Graph Convolution Network (STGCN) to extract joint features, coordinates and calculates the angle between the elbow and arm at various time stamps for evaluation.

This system is evaluated on a custom made dataset of cricket bowling actions which has been released in the public domain. The dataset contains front-on camera angle bowling videos. The aim is to provide quicker decision making and a more accessible technology



## Environment Variables

The project is developed under the following environment:

Python 3.8.10 

PyTorch 2.0.0

CUDA 11.9

## Datasets
The pose estimation model is tested on two publicly available datasets: Humans3.6M and MPI-INF-3DHP. 
The classification model is then tested on a bowling action dataset.
A sample of the dataset is is shown in fig 1.
!['BowlingAction'](https://github.com/HimanshuS11/Classification-of-Bowling-Action-using-Pose-Estimation/blob/main/photos/bowlingaction.png)

The description of the datasets is given in table 1
Dataset       | Characteristics | Year
------------- | -------------   |------  
Humans3.6M    | 1,376 videos    | 3600k poses, 11 subjects
MPI-INF-3DHP  | 1.3M frames    |3 outdoor settings, 8 subjects
Bowling Action Dataset  | 30 videos    | 20 legal, 10 illegal actions

##Result

For frames of the video 2D and 3D pose estimation is done and P1-MPJPE error (in mm) and P2-Error on 2D ground truth (in mm) is calculated with the results shown in table 2.
Dataset       | P1 | P2
------------- | -------------   |------  
Humans3.6M    | 42.5    | 26.5
MPI-INF-3DHP  | 17.1    |-

Output of Pose Estimation Model
