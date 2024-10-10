# Anomaly Detection in Intrusion Zones Using Deep Learning  

## Project Overview
This project focuses on developing deep learning models to detect anomalies in intrusion zones using a dataset designed for this purpose. By employing different architectures, including Dense Neural Networks and Convolutional Neural Networks (CNNs), the goal is to accurately predict and identify potential intrusions based on various features.

## Table of Contents
Introduction

Dataset

Model Architectures

Dense Neural Network

Convolutional Neural Network (CNN)

Evaluation Metrics

Results

Future Work


### Introduction
In an increasingly connected world, safeguarding against unauthorized access and intrusion is paramount. This project utilizes deep learning techniques to automatically identify anomalies in data associated with intrusion zones. By training models to reconstruct input data, we can detect significant deviations that indicate potential threats.

### Dataset
The data for this project is generated using a mathematical model of OTDR. Intrusions are simulated by introducing noise at random locations along the cable, utilizing sinusoidal variations to mimic real-world scenarios.

 Cable Length: A total of 4000 meters of cable is tested.
 Segmentation: The cable is divided into 97 zones, each approximately 41 meters long, to facilitate better data extraction and detection.
 Input Parameter: The difference in amplitude is used as the primary input for the models to detect anomalies related to intrusions.

### Model Architectures
 
 *Dense Neural Network*

Description: The first model is an autoencoder built using dense layers. This architecture aims to learn the intrinsic structure of the input data by minimizing reconstruction error.
Activation Functions: ReLU is employed to introduce non-linearity.
Loss Function: Mean Absolute Error (MAE) is used to quantify reconstruction loss.


*Convolutional Neural Network (CNN)*

Description: Two CNN architectures are implemented to leverage the strength of convolutional layers in extracting local patterns from the input features.
Layers: Each CNN consists of multiple Conv1D layers followed by Leaky ReLU activations and max pooling layers.
Loss Function: Similar to the dense model, MAE is used to assess model performance.

*Evaluation Metrics*
The performance of the models is evaluated using accuracy based on the detection of anomalies against known intrusion zones. A threshold envelope is created based on the mean and standard deviation of the prediction errors to identify anomalies effectively.


### Results
The models demonstrate varying performance metrics, with the Dense Neural Network showing promising results in terms of reconstruction accuracy. The CNN architectures further enhance feature extraction, leading to improved anomaly detection capabilities.

### Future Work
Model Optimization: Experimenting with hyperparameter tuning to improve model performance.
Additional Features: Incorporating more features to enhance the robustness of the anomaly detection.
Deployment: Exploring options for deploying the model in real-time intrusion detection systems.
Filter: Filtering out the different type of Intrusion in class as Threatening Intrusion or Non-threatening Intrusion



