# Project Name
> Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A AI/ML solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis. 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- To build a CNN based model which can accurately detect melanoma. This is a multiclass classification model using a custom convolutional neural network in Tensorflow.
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- model is overfitting on first trail CNN model with limited layers. There is quite good difference between training accuracy (88%) and validation accuracy (55%)
- Augmentation and adding dropout layers shows improvement on reducing the overfitting. But training accuract is too low, 49%
- Verified the class imblances, this can impact the training accuracy.
        1)seborrheic keratosis has least number of samples -  77 images ( 3.2%)
        2)pigmented benign keratosis has more number of samples - 462 images (20.6%)
- Adding more number of samples in dataset, increases the training accuracy. Augmentor helps to modify the images and adds more number of samples in the data set.
- Training accuracy and validation accuracy are not close each other, model is overfiting, this needs to be studied further.
- Noticed quite good oscialations on validation accuracy(~80% to 85%) between epochs while training the model with more epochs.
- Model accuracy can be improved by adding further more datasets and choosing the optimimum layers in CNN model.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy                         1.24.3
- pandas                        1.5.3
- matplotlib                    3.7.1
- tensorflow                    2.16.1
- keras                         3.1.1
- python                        3.11.3
- glob                          0.7
- augmentor                     0.2.12




<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project is Upgrade assignment to learn CNN model better.
- Thanks to Upgrade and professors for sharing the knowledge about CNN.


## Contact
Created by [@sgragupathi] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->