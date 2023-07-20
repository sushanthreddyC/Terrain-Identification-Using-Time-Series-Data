# Terrain-Identification

## Background

Humans naturally develop walking capability that is energy efficient, stable, environment adaptive, and robust. Lower limb amputations, unfortunately, disrupt this ability; individuals with lower limb amputations usually depend on prosthetic devices to restore the basic walking function. Lower-limb robotic prosthetics can benefit from context awareness to provide enhanced comfort and safety to the amputee. In this work, we aim to develop a terrain identification system based on inertial measurement units IMU streams collected from the lower limb. The system for a prosthetic leg uses visual and inertial sensors though, but we are willing to observe if terrain identification without the visual data is viable. With such information, the control of a robotized prosthetic leg can be adapted to changes in its surrounding.


## Data Description

Data consists of at several sessions from 6 different subjects including IMU data from a sensor on the leg of a participant, and the labels come from annotations of terrain type from a synchronized data stream. We only make use of the IMU data for this project. This work is inspired by this research project: https://research.ece.ncsu.edu/aros/paper-tase2020-lowerlimb/. There are in total 4 classes for the data

## Evaluation Metrics

Accuracy, F1-Score

## Models implemented

### Baseline Model - Random Forest with over+under-sampling

Results : 

![image](https://github.com/psvkaushik/Terrain-Identification/assets/86014345/99d3ea35-7f24-4b46-a41b-19fb1b472d06)



### Final Model - CNN + BiDirectional LSTM

![image](https://github.com/psvkaushik/Terrain-Identification/assets/86014345/2fedc2d5-f55b-42c6-8d8e-1bc9dd5b18e5)

Results : 

![image](https://github.com/psvkaushik/Terrain-Identification/assets/86014345/ce9648b5-6a24-4f24-b25c-cd9438a6e90c)

