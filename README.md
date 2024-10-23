# Ninjacart: CNN Classification
### Problem Statement
Ninjacart is India's largest fresh produce supply chain company, dedicated to solving significant supply chain challenges through innovative technology. They source fresh produce from farmers and deliver it to businesses within 12 hours. A key aspect of their automation process involves developing robust classifiers to distinguish between different types of vegetables while accurately labeling images that do not contain these vegetables as noise.

The dataset provided consists of images scraped from the web, organized into train and test folders, each containing four sub-folders for images of onions, potatoes, tomatoes, and various market scenes. Our task is to prepare a multiclass classifier to identify these vegetables.

### Goal
The goal of this project is to develop a highly accurate image classification model that can reliably distinguish between images of onions, potatoes, and tomatoes while effectively identifying non-vegetable images as noise. This classifier aims to enhance Ninjacart's automation processes and improve the overall efficiency of their supply chain operations.

### Context
The dataset includes:
- **Vegetables**: Onion, Potato, Tomato
- **Noise**: Images depicting Indian market scenes

### Summary of the Classification Process:

#### 1. Model Architecture Development:
- Designed a Convolutional Neural Network (CNN) with multiple convolutional layers, batch normalization, and dropout to mitigate overfitting.

#### 2. Data Preparation:
- Resized all images to **224x224 pixels** to align with the VGG16 architecture.
- Implemented data augmentation techniques to increase the diversity of the training dataset, enhancing model robustness.

#### 3. Model Compilation and Training:
- Compiled the model using the **Adam optimizer** and **sparse categorical crossentropy** loss function.
- Trained the model on the dataset with the following accuracy results:
  - **Epoch 1**: Accuracy: **70.17%**, Validation Accuracy: **94.96%**
  - **Epoch 2**: Accuracy: **95.15%**, Validation Accuracy: **97.89%**
  - **Epoch 3**: Accuracy: **98.38%**, Validation Accuracy: **98.92%**

#### 4. Performance Monitoring:
- Utilized callbacks such as **early stopping**, **learning rate reduction**, and **model checkpointing** to enhance training efficiency.
- Evaluated model performance through metrics like accuracy and validation loss.

#### 5. Confusion Matrix Analysis:
- Generated confusion matrices to analyze classification performance for onions, potatoes, and tomatoes, highlighting areas of potential confusion.

#### 6. VGG16 Transfer Learning:
- Leveraged a pretrained **VGG16** model by adding custom layers for classification, significantly improving accuracy.

#### 7. Final Results:
- Achieved high accuracy rates during both training and validation phases, demonstrating the model's effectiveness in classifying the target vegetable categories.

#### 8. Insights and Conclusions:
- Derived actionable insights from the analysis, underlining the importance of data-driven decision-making in enhancing business outcomes.

