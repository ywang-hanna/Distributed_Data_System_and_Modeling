# SMARTPHONE-BASED-HUMAN-ACTIVITY-RECOGNITION

## Introduction

Smart equipment has been a common necessity for people in modern daily life. The porta- bility characteristic makes those smart devices prolific data sources, making it possible to use data collected from human activities to predict certain types of behavior, which is helpful for further research in many other fields such as health monitoring and medical emergency. As different sensors on one device could get thousands of records per day, the volume of recorded data explodes, which means analysis and modeling would be chal- lenging for a single machine. Thus, we built a workflow based on a distributed system including Amazon S3 cloud storage, mongoDB, Amazon EMR cluster and SparkML in this project.

## Data Source

We use the data collected by the Department of Electrical and Computer Engineering in UCSD. They designed a mobile application which could be used on iPhone and Android smartphones as well as Pebble smartwatch to collect data on both sensor measurements and ground truth labels. The whole data set contains a total of 377,346 labeled examples (minutes) of sensor data from 60 users with 280 features from different sensors (e.g. accelerator, gyroscope, magnetometer, etc), which could be used in the analysis and model.

## Methodology

<img width="839" alt="mongdb" src="https://user-images.githubusercontent.com/40588854/54891862-499d7080-4e6c-11e9-9a8e-7903640a6888.png">

- Upload the data on S3
- Load S3 data to MongoDB
- Run SparkML on EMR cluster
- Model Improvement

## Result
For the purpose of reporting, our model includes 10 labels with highest frequencies: In- doors, At Homes, Sitting, Phone on Table, Lying Down, Sleeping, At School, Computer Work, Standing and Talking.

<p align="center">
<img width="310" alt="Screen Shot 2019-03-24 at 7 40 42 PM" src="https://user-images.githubusercontent.com/40588854/54891960-c29cc800-4e6c-11e9-8985-7e6b457e0946.png">
</p>

## Team
Yuhan Wang, Minchen Wang, Tianqi Wang, Zack Pan
