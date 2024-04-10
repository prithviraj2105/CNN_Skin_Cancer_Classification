# CNN Assignment
> Build CNN model to classify types of skin cancer based on skin images.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project is part of course study assignment. The course is Advanced Certification Program in Machine Learning and Deep Learning (ACP in ML & DL) conducted by IIIT Banglore.
- The project is to build a multi-class classification model using a custom convolutional neural network in TensorFlow.
- To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

The steps followed were:
- Created train & validation dataset from the train directory with a batch size of 32. Resized images to 180*180.
- Created first CNN model and trained the model for ~20 epochs. Observed that the model is Overfitting.
- Tried Image augmentation strategy to increase variability and also added dropout layers to prevent overfitting. Observed that model accuracies for both train and validation dataset were low indicating underfitting.
- Checked for Class imbalance. Observed class imbalance and low number of samples for some classes compared to others. Augmented dataset with new 500 images for each class. Trained final model for ~30 epochs, giving the model more time to learn to prevent underfitting. Observed increased accuracies and no underfitting.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

Data augmentation, class imbalance handling and adding dropout layers greatly improved model performance.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Jupyter Notebook - version 6.5.4
- Python - version 3.11.5
- numpy - version 1.24.3
- pandas - version 2.0.3
- seaborn - version 0.12.2
- matplotlib - version 3.7.2
- Keras - version 3.1.1 
- Tensorflow - version 2.16.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
<!-- Give credit here. -->
- This project is done with reference to a example (CIFAR-10 Classification with Python) covered in the Advanced Regression module.


## Contact
Created by [@prithviraj2105] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->