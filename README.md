<p align="center">
  
![GitBanner3](https://user-images.githubusercontent.com/98388088/158277311-535b2e53-190e-4060-a383-42e9f308ca75.png)

</p>
<hr>


<h1 align='center'> MNIST Image Classification Using Neural Networks (Pytorch) </h1>

<hr>


## Table of contents
- [Status and Details](#status-and-details)
- [Technology](#technology)
- [Introduction](#introduction)
    - [Project Description](#project-description)
    - [Objectives](#objectives)
- [Data Science Methodology](#data-science-methodology)
    - [Problem Formulation](#problem-formulation)
    - [Data Engineering Methods](#data-engineering-methods)
    - [Modeling](#modeling)
    - [Deployment](#deployment)
- [Conclusions](#conclusions)
- [Contributing Members and Contacts](#contributing-members-and-contacts)


## Status and Details
- **Project Status**: [Completed]
- **Date Coded**: 14/04/22
- **Link to Raw Data**: [https://archive.ics.uci.edu/ml/machine-learning-databases/00222/](https://www.kaggle.com/datasets/zalando-research/fashionmnist)
- **Notes**: Classification of MNIST Fashion dataset


## Technology
- **Language**: Python 3.6.9
- **Libraries**: torch, pandas, numpy, matplotlib, seaborn, scipy, sklearn, einops, random
- **Set up File**: N/A


## Introduction
The purpose of this project is to train a neural network to classify images of fashion. Training a machine to identify real world objects is of great interest. Appications include the improvement of self driving cars. If a self driving car can identify certain road signs, for example a 30mph sign, it can adjust its setting accordingly.


### Project Description
The dataset used for this project was the MNIST Fashion dataset. It is a huge dataset designed specifically for deep learning neural networks. It has 60,000 training images with 10,000 test images. The images are 28x28 greyscale images of 10 variations of fashion items such as t-shirts, shoes etc. The dataset is augmented to quadruple the amount of observations.

Using Pytorch, a neural network has been trained to identify items of clothing with an accuracy of 88%. Upon analysis of the results, the model has most difficulty distinguishing shirts from other similar items such as t-shirts or pull overs. 


### Objectives
- Transform and augment initial dataset.
- Using Neural Networks, train a model to classify items of clothing from an augmented dataset of 240,000 observations.
- Identify what the model struggles to classify and why.


## Data Science Methodology
The below subsections outline the standard methodology of data scientists.


### Problem Formulation
When a machine can be trained to identify and classify real world images, it can be extremely beneficial to society. An example of this includes facial recognition for the Iphone. The model must learn your face and identify that it is you in order to unlock the phone. There are many further societal benefits such as the classification of images of cancerous tumours.


### Data Engineering Methods
- **Data Transformation**: Convert image to tensor, flatten tensor to vector form,
- **Data Preprocessing**: Data augmentation, Split images into patches, image rotation, apply greyscale, normalisation
- **Data Visualisation**: Each step of data transformation and preprocessing is visualised. Confusion matrix visualised.
- **Machine Learning**: Deep learning


### Modeling 
Using a variation of the MLP, a model is trained using MNIST Fashion dataset. The dataset is transformed to allow it to be fed to the model. The data is augmented by splitting images in 2 and rotating them by 180 degrees. The resultant dataset is 240,000 observations. The model had an accuracy of 88% which is quite high for this particular dataset.


### Deployment
The model was deployed on a previously unseen dataset of 24,000 images. The model has an accuracy of 88%, with most of the incorrect classifications coming from the confusion of shirts with t-shirts and pull overs. Without such similar items, I would expect the accuracy to be in the low to mid 90's.


## Conclusions
An accuracy of 88% is observed with most incorrect classifications coming from the confusion of shirts, t-shirts and pull overs. Without such similar items, it is estimated that the accuracy could be as high as the mid 90's (likely low 90's). This model is not well suited for medicinal classification (such as tumour identification), however the accuracy is high for this particular dataset.  


## Contributing Members and Contacts
**Team Lead: [Daniel Elston](https://github.com/Daniel-Elston)**

|Name     |  GitHub Handles   |  
|---------|-----------------|
| Daniel Elston | [Git DE](https://github.com/Daniel-Elston)   |

Please feel free to contact me if you have any questions, require any further information or wish to contribute.<br/>
Email 1: delstonds@outlook.com<br/>
Email 2: ec21024@qmul.ac.uk
