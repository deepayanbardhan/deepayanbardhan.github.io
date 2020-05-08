---
title: "Texture Segmentation"
excerpt: "Separating textures using Mixture Model and EM algorithm<br/><img src='/images/texturesegmentation-cover.jpg'>"
collection: portfolio
---

## Brief Overview

![Python 3.6](https://img.shields.io/badge/Python-3.6-brightgreen.svg)    ![Problem Kaggle](https://img.shields.io/badge/Problem-Segmentation-blue.svg)     ![Problem Kaggle](https://img.shields.io/badge/data-PragueTextureSegmentationDataGenerator-orange.svg)

The basic idea of the code is to identify various textures or patterns from a given image. There are several images and each of those images have a mixture of various patterns. The task is to segment these various textures or to segregate them so that it can be easily understood that how the textures are different. For example, in the picture provided below, a human eye can clearly see and understand that there are 3 different patterns in the image and our task is to segment each of them individually such that each of the segmented mask can be used to select a particular pattern. However, the problem is not very trivial to be solved by a computer algorithm as the patterns, although are repeating to an extent, can come in various types and sizes.

<img src="/images/test_ip/tm1_1_1.png" width="200">

The method implemented to solve the problem is by using Gaussian Mixture of Models and Expectation Maximization.

### Sample Input / Output

Input Image           |  Output Image
:-------------------------:|:-------------------------:
<img src="/images/test_ip/tm1_1_1.png" width="200">   |  <img src="/images/test_op/test1r.png" width="200"> 
<img src="/images/test_ip/tm3_1_1.png" width="200">  |  <img src="/images/test_op/test3.png" width="200">
<img src="/images/test_ip/tm18_1_1.png" width="200">  |  <img src="/images/test_op/test18.png" width="200">
<img src="/images/test_ip/tm19_1_1.png" width="200">  |  <img src="/images/test_op/test19.png" width="200">
<img src="/images/test_ip/tm20_1_1.png" width="200">  |  <img src="/images/test_op/test20.png" width="200">

### Plot of log-likelihood values vs number of components over 20 iterations

<img src="/images/test_op/llhvsnoi1.png" width="600">

The log-likelihood values keeps on increasing with the increase in the number of components which is obvious but an indeal value of n_comps can be determined using the knee technique, i.e. checking the point of maximum reduction of variance for a particular value of n_comps . However, it has not been implemented in the code.

For the code check the [github repo](https://github.com/deepayanbardhan/TextureSegmentation).

The image data was obtained from the [The Prague Texture Segmentation Datagenerator](https://mosaic.utia.cas.cz/index.php?act=bench_form).

### Instructions to run the code:

Run the [plot.py](https://github.com/deepayanbardhan/TextureSegmentation/blob/master/plot.py) file to run the code. To obtain output for only a single value of n_comps - remove the loops in plot.py and just pass a single value of n_comp. Also the input to provide is in the deepcode.py file
