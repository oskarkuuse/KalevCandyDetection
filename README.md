# Kalev Candy Detection Competition

This repository is an overview of the Kalev Candy Detection Competition code and data, which was developed for the project in the Deep Learning in Computer Vision course at University of Tartu in the spring of 2024. 
The original authors of the project are Karl Oskar Kuuse, Karl-Erik Kanal and Paula Marie Loopere.

## Premise

The goal of the project was to come up with a computer vision problem, which could be turned into a Kaggle competition for other students. 
Our team created an original dataset of 501 images containing different candies by the brand Kalev, with the goal of training deep learning models that would be able to detect them. 
The original competition page with more information can be found [here](https://www.kaggle.com/competitions/kalev-candy-detection-competition).

## Structure

The folder `Dataset` contains the original training and testing data splits with the bounding box annotations for the training data. 
The original images were collected by us and labelled using Label Studio.

The folder `CompetitionSetup` contains an introductory notebook for the competitors and also the Kaggle custom metric script used with the solution file (originally not accessible to the competitors).

Folder `Models/Benchmark` contains the final benchmark for the competition trained by us. The model utilized is a medium-sized YOLOv8. Folder `Models/OtherCompetition` also contains our training notebooks and solutions for the other four competitions created by other students, which we participated in:
- [Bird Genus Multi-class Image Classification](https://www.kaggle.com/competitions/bird-genus-multi-class-image-classification#)
- [Image Classification: Real or AI-Generated Photo](https://www.kaggle.com/competitions/image-classification-real-or-ai-generated-photo)
- [SofaVision](https://www.kaggle.com/competitions/sofavision)
- Urban Issues Image Classification

All of the models utilize some size and variant (detection/segmentation) of the YOLOv8.

Note that all the notebooks are currently copied from the Kaggle system, where they were originally created (in order to utilize Kaggle's GPU resources). 
Hence the main goal of this repository is to collect the different notebooks and give an overview of the project, but they could also be run locally with minor changes.
