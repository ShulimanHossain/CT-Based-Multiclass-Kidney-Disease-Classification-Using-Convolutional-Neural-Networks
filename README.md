#  CT Scan Image Classification using Deep Learning

## Introduction
This project applies deep learning techniques to automatically classify CT scan images of kidneys. Multiple pretrained CNN architectures along with a custom-built CNN model are trained using TensorFlow. The models are evaluated using standard performance metrics to compare their effectiveness.

## Dataset
- Source: Kaggle (https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone)
- Classes:
  - Normal  
  - Stone  
  - Tumor  
  - Cyst  
- Preprocessing:
  - Image resizing (e.g., 224×224)
  - Normalization
  - Train/Validation split

##  Exploratory Data Analysis (EDA)
- Checked class distribution  
- Visualized sample images  
- Handled class imbalance using class weights  

##  Models Used

###  Transfer Learning Models
- ResNet50  
- VGG16  
- EfficientNetB0  

###  Proposed Model (Custom CNN)
- Conv2D + MaxPooling layers  
- Batch Normalization  
- Dropout  
- Dense layers  

##  Training Details
- Framework: TensorFlow / Keras  
- Loss Function: Categorical Crossentropy  
- Optimizer: Adam  
- Metrics: Accuracy  
- Techniques:
  - Data augmentation  
  - Class weighting  

##  Evaluation Metrics
- Accuracy  
- Loss  
- Precision, Recall, F1-score  

##  Results
| Model            | Accuracy 
|------------------|----------
| ResNet50         | 69.76%     
| VGG16            | 89.10%     
| EfficientNetB0   | 76.84%      
| Custom CNN       | 95.5%     


## Conclusion
This project shows that deep learning models can effectively classify kidney CT scan images into Normal, Stone, Tumor, and Cyst categories. Among the tested models, pretrained CNNs performed better overall, while the custom CNN provided a lightweight alternative. These results highlight the potential of deep learning in supporting medical image analysis.
