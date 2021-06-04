# Pneumonia X-Ray Detection

**Authors**: David Tian, Christopher de la Cruz

## Overview

Our project was to create an image classification model that given an x-ray could determine whether a child has pneumonia or not. We specifically looked into and outlined how an x-ray of a child with pneumonia is different from other x-rays. Pneumonia x-rays have characteristic white blobs of shapes in the lungs which also makes the x-ray less clear (called infiltrates). We used different CNN architectures on our different models and found that a regularized LeNet-5 model (a specific type of CNN architecture) seems to work best. This analysis can be used by any medical institution looking to further their understanding of x-rays of pneumonia.

## Business Problem

Given a chest x-ray image, can we build a CNN model that can accurately predict whether a person has pneumonia or not.

![image](https://user-images.githubusercontent.com/78755809/120658438-70e02700-c453-11eb-885f-091419cfbc3b.png)

## Data

Our dataset consisted of 5856 chest x-rays from Mendely data (https://data.mendeley.com/datasets/rscbjbr9sj/3)

![image](https://user-images.githubusercontent.com/78755809/120658523-82293380-c453-11eb-9159-a3ed3d62cb91.png)
![image](https://user-images.githubusercontent.com/78755809/120658535-848b8d80-c453-11eb-91d1-342cc4885e0e.png)
![image](https://user-images.githubusercontent.com/78755809/120658547-86555100-c453-11eb-9b2a-6cbd8dd3fba7.png)

## Methods

For preprocessing, we resized each image to be 128x128 pixels. We leveraged neural networks and convolutional neural networks to detect whether an x-ray contained pneumonia or not.

## Best Results

Our strongest model was a regularized LeNet-5 network of 3 layers (alternating convolution and max pooling layers) that was able to achieve an accuracy of 96% on the training set and 79% on the testing set.

## Conclusions

While we were relieved to have one high-performing model given our 3-day time window, we realize that we've just scraped the surface of the different CNN architectures. Given more time and stronger computing power, we'd like to explore the other types of architectures and be able to experiment with more regularization. 

## For More Information

Please review our full analysis in our Jupyter Notebook or our presentation: https://docs.google.com/presentation/d/1QXtbg0Zaz7P9He8mpOi8chDeMgruxyUjylWO7_J0Pdw/edit#slide=id.g774478e1d0_0_10

For any additional questions, please contact **Christopher de la Cruz at cdelacruz2013@gmail.com, David Tian at dt1086@stern.nyu.edu**

## Repository Structure

```
├── README.md                                         <- The top-level README for reviewers of this project
├── Pneumonia Detection - Phase 4 Project.pdf         <- PDF version of project presentation
├── Pneumonia Detection Analysis.ipynb                <- Narrative documentation of analysis in Jupyter notebook 
├── data                                              <- Both sourced externally and generated from code     
```
