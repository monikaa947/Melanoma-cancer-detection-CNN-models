# Cancer detection multiclass classification CNN model
> Building CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- In this project, I will build a multiclass classification model using a custom convolutional neural network in TensorFlow. 

 
- I'm going to build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early.
- What is the business probem that your project is trying to solve?

    Building CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- What is the dataset that is being used?
    
    The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


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

    Going to build custom model instead of any pre-trained model using Transfer learning.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- First model is buit using general CNN layers which indicate overfitting due to the significant gap between training and validation performance. Applying regularization, improving data augmentation, and addressing class imbalance will likely improve the model's generalization ability and reduce validation loss.
- Second model buit using sequential's default image augment strategy, added more layers which results, the low accuracy across both training and validation datasets that indicates a fundamental issue with either the dataset, model architecture, or training process. Which need more focus on increasing model complexity, enhancing augmentation strategies, experimenting with hyperparameters (learning rate, optimizers), leveraging transfer learning for improved results.
- After analysing class imbalance of dataset found some points Seborrheic keratosis (80 samples, 4.0%) has least samples, some dominant classes in dataset like Basal cell carcinoma (17.6%),  Pigmented benign keratosis (19.7%), Melanoma (19.3%) in terms proportionate number of samples. This indicate very high difference in range of class images. To approach this problem try other data augmentation strategies.
- At Final model building using "Augmentor" data augment python library,performs reasonably well, with balanced training and validation metrics. To push the performance further, consider data augmentation, regularization, and hyperparameter tuning. A slight improvement in validation accuracy and reduction in validation loss would make the model even more robust.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Tensorflow - version 2.13.1
- Augmentor - version 0.2.12
- Matplotlib
- Counter

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [@monikaa947] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
