Problem Statement:

The objective is to develop a Convolutional Neural Network (CNN) model capable of accurately identifying melanoma, a severe form of skin cancer responsible for 75% of deaths related to skin cancer. Early detection is critical, and an automated solution that analyzes images and alerts dermatologists about the presence of melanoma can significantly reduce the manual workload involved in diagnosis.

Dataset Overview:

The dataset comprises 2,357 images of malignant and benign oncological conditions, sourced from the International Skin Imaging Collaboration (ISIC). These images are categorized based on ISIC classifications. While most categories are evenly distributed, melanomas and moles have a slightly higher representation. The dataset includes the following skin conditions:

Actinic keratosis

Basal cell carcinoma

Dermatofibroma

Melanoma

Nevus

Pigmented benign keratosis

Seborrheic keratosis

Squamous cell carcinoma

Vascular lesion

Note: Do not use any pre-trained models or transfer learning techniques. The focus should be on creating a fully custom model.

Project Workflow:

Data Exploration and Preparation:

Load and understand the dataset.

Define file paths for training and testing images.

Dataset Creation:

Partition the dataset into training and validation sets with a batch size of 32.

Resize images to 180x180 pixels.

Dataset Visualization:

Implement a visualization function to display one sample image from each of the nine categories.

Model Development and Training:

Construct a CNN model to classify the nine categories accurately.

Normalize pixel values to the range (0,1) by rescaling the images.

Select an appropriate optimizer and loss function.

Train the model for approximately 20 epochs.

Analyze the model’s performance and determine if there is any evidence of overfitting or underfitting.

Addressing Overfitting/Underfitting:

Apply suitable data augmentation techniques to mitigate overfitting or underfitting.

Model Development with Augmented Data:

Rebuild the CNN model using the augmented dataset.

Normalize pixel values to the range (0,1).

Choose an appropriate optimizer and loss function.

Train the model for approximately 20 epochs.

Assess the results to determine if the issues identified earlier have been resolved.

Class Distribution Analysis:

Evaluate the distribution of classes in the training dataset.

Identify the class with the fewest samples and the dominant classes in terms of sample proportion.

Handling Class Imbalances:

Address class imbalances in the training dataset using the Augmentor library.

Model Development with Balanced Data:

Develop a CNN model to classify the nine categories using the balanced dataset.

Normalize pixel values to the range (0,1).

Select an appropriate optimizer and loss function.

Train the model for approximately 30 epochs.

Document findings and evaluate whether the adjustments have resolved any prior issues.

By following this pipeline, the project aims to create a robust model capable of accurately detecting melanoma and other skin conditions, contributing significantly to automated medical diagnostics.
