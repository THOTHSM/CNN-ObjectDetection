Ninjacart: CV Classification

Problem Statement:
    Ninjacart is India's largest fresh produce supply chain company. They are pioneers in solving one of the toughest supply chain problems of the world by leveraging innovative technology. They source fresh produce from farmers and deliver them to businesses within 12 hours. An integral component of their automation process is the development of robust classifiers which can distinguish between images of different types of vegetables, while also correctly labeling images that do not contain any one type of vegetable as noise.
    As a starting point, ninjacart has provided us with a dataset scraped from the web which contains train and test folders, each having 4 sub-folders with images of onions, potatoes, tomatoes and some market scenes. We have been tasked with preparing a multiclass classifier for identifying these vegetables. The dataset provided has all the required images to achieve the task.

Context:
This dataset contains images of the following food items: noise-Indian market and images of vegetables- onion, potato and tomato.

Summary:
    Model Architecture Development:
        Designed a CNN model with multiple convolutional layers, batch normalization, and dropout to prevent overfitting.

    Data Preparation:
        Resized images to 224x224 pixels to fit the VGG16 architecture.
        Implemented data augmentation techniques to enhance the diversity of the training dataset.

    Model Compilation and Training:
        Compiled the model using the Adam optimizer and sparse categorical crossentropy loss.
        Trained the model on the dataset, achieving the following accuracy values:
            Epoch 1: Accuracy: 70.17%, Val Accuracy: 94.96%
            Epoch 2: Accuracy: 95.15%, Val Accuracy: 97.89%
            Epoch 3: Accuracy: 98.38%, Val Accuracy: 98.92%

    Performance Monitoring:
        Utilized callbacks such as early stopping, learning rate reduction, and model checkpointing to optimize training.
        Evaluated model performance using metrics like accuracy and validation loss.

    Confusion Matrix Analysis:
        Generated confusion matrices to assess classification performance for the onion, potato, and tomato categories, identifying areas of confusion.

    VGG16 Transfer Learning:
        Leveraged a pretrained VGG16 model, adding custom layers for classification, and trained it to improve accuracy significantly.

    Final Results:
        Achieved impressive accuracy rates during training and validation, with the final model showcasing high effectiveness in classifying the target categories.

    Insights and Conclusions:
        Derived actionable insights from the analysis, emphasizing the importance of data-driven decision-making for enhancing business outcomes.
