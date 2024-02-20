# Lung-Cancer-Detection

This project is an academic project created for the course SDS 384: Scientific Machine Learning

Team Members - Shreya Shukla, Reem Fashho, Amanda Nowacki

### Motivation
The primary objective of our project was to evaluate the performance of various neural network-based models in **classifying cancerous and non-cancerous lungs**. Specifically, we aimed to achieve binary classification, distinguishing between lungs with tumors and those without. To accomplish this, we employed four different architectures: 2D CNN, VGG-16, ResNet-50, and DenseNet201. To validate cancerous locations within the lung images, we employed the LIME (Local Interpretable Model-Agnostic Explanations) explainability technique. **By leveraging LIME, we gained insights into the specific areas within the lung images that influenced the model's decision-making process.**

### Dataset
Our data set is the Chest CT-Scan Images Dataset uploaded to Kaggle by Mohamed Hany. https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

The dataset includes CT slices of non-cancerous chest tissue and three types of chest cancers: adenocarcinoma, large cell carcinoma, and squamous cell carcinoma.

<img width="325" alt="Screenshot 2024-02-19 at 8 50 42 PM" src="https://github.com/shreyashukla01/Lung-Cancer-Detection/assets/30028998/8319984d-8e11-448e-bc8c-f8b1e4e7f09c">

### Methods

1. **Classification Performance Comparison -** In this part, we assessed how well four algorithms can distinguish between healthy healthy and unhealthy patients with a form of pulmonary cancer.  The algorithms we used for this task are VGG16, 2D CNN, ResNet50, and DenseNet201.
2. **Performance Comparison on Augmented Data -** In this part, we checked model's performance on augmented data. The data was augmented by cropping the images by 25 pixels, flipping 50% of all training images vertically, and applying a Gaussian blur to the images.
3. **Performance Comparison on modified images -** To check the robustness of models - VGG16 and ResNet50 we decide to see performance gradient for classification of images by making changes to the contrast of images, introducing gaussian noise into the images and undersampling images using different strides.

<img width="342" alt="Screenshot 2024-02-19 at 8 59 01 PM" src="https://github.com/shreyashukla01/Lung-Cancer-Detection/assets/30028998/af4d6e3b-6c27-4f4b-8193-d71b168c4677">  <img width="342" alt="Screenshot 2024-02-19 at 8 58 35 PM" src="https://github.com/shreyashukla01/Lung-Cancer-Detection/assets/30028998/084df374-8fde-48ec-bb36-45ae4a668f8a"> 

4. **LIME Explainability for cancel location detection -** We explored LIME technique to identify regions within the images that contributed to positive predictions indicating cancerous labels.

   <img width="342" alt="Screenshot 2024-02-19 at 9 01 54 PM" src="https://github.com/shreyashukla01/Lung-Cancer-Detection/assets/30028998/74a3a644-0c1b-433e-89f9-217e269560a7">

   As seen in Figure above, the green area is spread across the different parts of the lung including the center, where the location of cancer is for the squamous lung cancer type. 

