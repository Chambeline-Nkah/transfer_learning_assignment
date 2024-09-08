1. Problem statement

Early and accurate detection of plant diseases remains a challenge in the agricultural sector, and this has drastically affected global food security. Manual methods used by farmers, such as visual inspection, are unreliable as they are time-consuming and limited in scale. These methods tend to miss the early stages, thereby reducing productivity. By developing a deep CNN image classifier for plant disease detection, it is possible to automate the processes, thereby improving accuracy and efficiency and leading to increased crop yield and more sustainable agricultural practices.

2. About the dataset

The dataset (https://www.kaggle.com/datasets/muhammadardiputra/potato-leaf-disease-dataset) contains images of potato leaves with three common diseases: early blight, late blight, and healthy leaves. The dataset consists of a total of 1,500 images, with 500 images for each class (early blight, late blight, and healthy leaves). The images have a resolution of 256x256 pixels.

3. Overview of the Evaluation Metrics Chosen to Assess the Performance of the Fine-Tuned Models
To assess the performance of the fine-tuned models (VGG16, ResNet50, and InceptionV3), we utilized the accuracy and loss evaluation metrics:

4. Findings from the process
The following findings were obtained from the fine-tuned process:
- VGG16:


    Strengths: The VGG16 model achieved a high test accuracy of 91.67% and a low test loss of 0.3138. This indicates that VGG16 effectively learned to classify the potato disease images, demonstrating its effectiveness in feature extraction.

    Limitations: While VGG16 performed well, it is a relatively large model, and thus took a longer time during the training process despite the fact that it used just 2 epochs. Thus, its performance might not be optimal for all types of datasets, especially if the dataset is imbalanced.

- ResNet50:


    Strengths: ResNet50 achieved a test accuracy of 69.79% and a test loss of 0.7447. The architecture's use of residual connections allows for training deeper networks without the vanishing gradient problem, which can be beneficial in complex tasks.

    Limitations: ResNet50's performance was lower compared to VGG16 and InceptionV3. Thus this suggests that it may require further fine-tuning or a larger dataset to improve its accuracy. Additionally, the model’s complexity can lead to overfitting if not managed properly.

- InceptionV3:


    Strengths: InceptionV3 achieved the highest test accuracy of 97.40% and the lowest test loss of 0.0828. This model's architecture, which captures multi-scale features, allows it to perform exceptionally well on diverse datasets, making it particularly effective for image classification tasks.

    Limitations: Its complexity can also be a drawback.



In conclusion, the findings highlight the strengths of transfer learning in the context of the potato disease classification problem as it allows us to leverage pre-trained models that have already learned feature representations from large datasets. However, the limitations observed in some models, particularly ResNet50, indicate that transfer learning is not a one-size-fits-all solution. The effectiveness of transfer learning can vary based on the dataset's characteristics, the specific model architecture, and the need for further fine-tuning. Thus in transfer learning, there should be a careful consideration of model choice and dataset properties as it is essential for optimal performance. 





![Screenshot (76)](https://github.com/user-attachments/assets/af6034a7-84ff-41ce-9e26-91563e80f64b)
