                                          MSc Data Science Thesis

# Vector Capsule Network for wild animal species recognition in Camera trap images

## Abstract
The most critical task in Ecology is observing and studying the wild animals in their natural habitat. Camera traps are the most helpful tools for ecologists and researchers for effective and constant monitoring of wild animals. Monitoring wildlife using camera traps is necessary as it helps researchers to understand human impacts on wildlife, and also help management to
make better decisions. However, annotating a large amount of camera trap data is time-consuming. Hence, auto tagging of the wild animal species in camera traps is of great importance, and its gaining speed as more and more deep learning solutions are being implemented on a variety of problems. One such computer-assisted system could be an auto-tagging tool which can classify diverse animal species in real-time. This work is an attept to present a new and novel deep neural networks called 'Capsule Network' as a solution to the problem of classifying wild animal species. Capsule Network is the latest development in Artificial Intelligence and is a new and exciting approach to computer vision. It has shown excellent results on various image recognition problems as per the research published so far. The work further tests the robustness of the newly introduced 'Capsule Network,' by comparing its performance with the Convolutional Neural Network. The results achieved indicate that the Capsule Networks are better at understanding images than ConvNets.

## Hypothesis
The camera trap images of wild animals are the kind of images where Convolutional Neural Networks may have a problem, because of species exhibiting a variety of poses and therefore, Capsule Networks can be expected to outperform Convolutional Neural Networks. Capsule Network has obtained state-of-the-art results on the dataset with the objects with affine transformations (https://arxiv.org/pdf/1710.09829.pdf), and can, therefore, be expected to perform better than Convolutional Neural Networks on camera trap images.

## Research Question 
Is Capsule Network better than Convolutional Neural Network in classifying wild animal
species in camera trap images?

## Dataset
An annotated camera-trap dataset of 20 species commonly found in North - America is used for training the model. The dataset contains 15826 images of 20 species namely Agouti, Bird spec, Coiban Agouti, Collared Peccary, Common Opossum, European
Hare, Great Tinamou, Mouflon, Ocelot, Paca, Red Brocket Deer, Red Deer, Red Fox, Red Squirrel, Roe Deer, Spiny Rat, White Tailed Deer, White-nosed Coati, Wild Boar, and Wood Mouse. The dataset contains a collection of gray-scale and color images. 

The images captured at night are in gray-scales and images captured in daytime are in colored.

Every image contains only one species out of 20 species. 80% of the dataset, i.e., 12660 images is used for training and the rest 20% for testing.

Link to Dataset Repo 
https://data.world/deana/camera-traped-wild-animals-images
or
https://drive.google.com/open?id=14vII7LJP8Hv-Uz4Av5DA33_Hyz95PL0I


![](Images/Page_00.png)
![](Images/Page_01.png)

## Convolutional Neural Network architecture used for wild animal species classification.

The architecture consists of two convolution layer with ReLU activation function and followed by a pooling layer with a dropout of 50%, and a final layer, a fully connected layer.

INPUT -> CONV1 -> ReLU -> CONV2 -> ReLU -> POOL -> DROPOUT -> FC -> ReLU -> DROPOUT - > FC - > SOFTMAX

![](Images/CNNArch.png)

#### CNN Specification








