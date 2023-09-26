# Multiclass-Classification-of-Kidney-Ailments-using-VGG16

# Introduction
Kidneys play a major role in the human excretion system. The nutrients obtained from various sources are digested and metabolized by the body. The toxic substances which are harmful to the human body are excreted by the excretory system. Kidneys help in removing waste from the body and balance the body fluids.Early detection of Kidney ailments can reduce the long-term impact of kidney failures which gradually lead to death. 

The main aim of this project is to effectively classify the computed tomography scans into Cyst, Tumor, Normal, and Stone Classes by extracting the significant features. The motivation behind this project was to develop an efficient deep learning model that can assist medical professionals by providing a support system for the decisions taken and comparing the results in real time.

# Methodology
* To use the VGG16 model to extract the relevant features from the computed tomography scans.
* Visualizing the features from each convolution layer of the VGG16 model to analyze which parts of the scan, the model has concentrated more.
* To use the extracted features from the model to build a random forest classifier for classifying the scans into cyst, normal, stone, and tumor.
* Determining the performance of the classification model through the confusion matrix and classification report.

# Models
* VGG16
* Random Forest Classifier
 
# Dataset
A secondary dataset collected from Picture Archiving and Communication System (PACS) from different hospitals in Dhaka, Bangladesh where patients were already diagnosed with having a Kidney tumor, cyst, normal, and stone findings are used for the feature extraction and classification. This dataset is publicly available on [Kaggle](https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone/code?select=CT-KIDNEY-DATASET-Normal-Cyst-Tumor-Stone). We will be using the pre-trained model - VGG16, for the feature extraction and the  Random Forest Classifier for the classification of CT scans. 

# Results

Out of the 1200 samples in the test set, 1190 test data were predicted correctly achieving an accuracy of 99.16%. 6 of the Stone classes were predicted as Normal, and 1 scan of the Stone Class was predicted as belonging to the Cyst class by the model. Out of the 300 scans belonging to the Normal Class 98% of them were predicted correctly by the model. 98% of the samples are actually belonging to the Normal Class out of all samples that were predicted to be of the Normal Class.  98% of the samples were predicted correctly as belonging to the Stone class out of all the samples that actually belong to the Stone Class. Cyst and Tumor classes have obtained an F1-score of 100%. The model's performance over the entire dataset is 99%. 

# Conclusion
The current study focussed on extracting the features from the CT scans using the VGG16 model that enabled us to effectively classify the ailments. Based on the features extracted from the model, the images were classified into their respective classes with the help of random forest classifier and was able to achieve an accuracy of 99.16%. Moreover, CT scans provide the ability to image even small differences at the cross-sections and have high contrast. Besides, the dataset used for this study used both contrast and non-contrasted CT scans, increasing the quality of the data.

# References
* (https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone/code?select=CT-KIDNEY-DATASET-Normal-Cyst-Tumor-Stone)
* (Islam MN, Hasan M, Hossain M, Alam M, Rabiul G, Uddin MZ, Soylu A. Vision transformer and explainable transfer learning models for auto detection of kidney cyst, stone and tumor from CT-radiography. Scientific Reports. 2022 Jul 6;12(1):1-4.)
* ( N. Narmada, V. Shekhar and T. Singh, "Classification of Kidney Ailments using CNN in CT Images," 13th International Conference on Computing Communication and Networking Technologies (ICCCNT), Kharagpur, India, IEEE, 2022, pp. 1-5, doi: 10.1109/ICCCNT54827.2022.9984256.)
  
    
