# ANALYSIS OF DEEP LEARNING MODELS FOR INDIAN FOOD CLASSIFICATION


This project was inspired by a podcast that YouTube recommended me in mid October introducing me to Prof. Bagler from IIIT Delhi. While going through his Google Scholar profile I was inspired to implement a research papr[1] published by his team.

## Context
As a case study, I implement popular Deep Learning Models for Image Classification in the context of Indian food platters, known for their complex presentation that poses a challenge for the automated detection of dishes.

Starting with the 15 most popular Indian dishes, the objective is to identify the state-of-the-art model through a **comparative analysis** of deep-learning-based architectures.

Among other culinary traditions, Indian cuisine is known for its visually complex platters, making dish detection a challenging problem. Collecting platter images with manual dish annotations is a necessary precursor for building an accurate dish classification and detection system. This software could have wide ranging potential from diet logging to culinary recommendations, food delivery systems and so much more. 

## Dataset

Despite its rich and diverse culinary heritage, the shortage of labeled collections of Indian food images is a significant challenge in developing accurate and effective models for food classification, dish detection, and recipe recommendations.

I've identified 15 most popular traditional Indian dishes and scraped images for these Instagram and Google Images containing traditional Indian food dishes using Python and extensions.

Thus compiled, the ‘IndianFood15’ dataset consists of 9601 labeled images with 15 food classes (650 images for each class). The average number of platter images for each dish class was 671±135 Among the outlier classes were dal makhani(482) and kaju katli(532), momos (1029), and biryani (874).

This Dataset was divided into Training, Validation and Testing Dataset in the ratio of 70 : 15 : 15 

![image class distribution](https://github.com/user-attachments/assets/4fec495f-5040-4902-8c77-2b1d4730039d)


4 popular Deep Learning Model Architectures chosen for this comparative analysis study are as follows, along with Logged Training and Validation Results through each epoch during the training phase:

**1. AlexNet**

<img src="assets/alexnet loss.png" alt="alexnet loss" width="45%" /> <img src="assets/alexnet accuracy.png" alt="alexnet acc" width="45%" />

**2. VGG16**

<img src="assets/vgg16 loss.png" alt="vgg loss" width="45%" /> <img src="assets/vgg16 accuracy.png" alt="vgg acc" width="45%" />

**3. Resnet152**
   
<img src="assets/resnet loss.png" alt="resnet loss" width="45%" /> <img src="assets/resnet accuracy.png" alt="resnet acc" width="46%" />

**4. DenseNet169**
   
<img src="assets/densenet loss.png" alt="densenet loss" width="45%" /> <img src="assets/densenet accuracy.png" alt="densenet acc" width="46%" />


The Accuracy of these models on the Testing Dataset was measured along 3 metrics, and results are as follows:

| **Classification Model** | **mAP (%)** | **F1 (%)** |**P (%)**  | **R (%)**  |
|:--------------------:|:-------:|:------:|:------:|:------:|
| AlexNet              | 26.54   | 28.30  | 32.99  | 32.99  |
|**VGG16**               | **94.83**   | **88.81**  | **89.35**  | **88.65** |
| ResNet152            | 92.22   | 84.67  | 85.45  | 84.49  |
| DenseNet169          | 93.41   | 83.86  | 85.31  | 84.35  |

## Links and References

[1] G.Bagler, M.Goel, “Framework for automated diet logging and nutrition management”

[2] <a href="https://youtu.be/_RgdXdaX6_E?si=9U2NUBlUSvurmvf_" target="_blank">Conversation with Ganesh Bagler : Computational Gastronomy with 'food for thought'</a>

