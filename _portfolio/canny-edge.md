---
title: "Canny Edge from Scratch"
excerpt: "Implementing Canny Edge Detector from Scratch<br/><img src='/images/edge0.png'>"
excerpt: "Implementing Canny Edge Detector from Scratch"
collection: portfolio
---

## Brief Overview

Edge detection is a very important aspect of image processing as it is important to mark boundaries or outlines in images many a times and there are many algorithms to perform the task of edge detection. But one of the most important algorithm that is used very commonly is known as Canny Edge Detector.

In this project, the steps of canny edge detection are performed without using any direct OpenCV packages. It will help to understand the working very elaborately. 

The steps of Canny Edge detector are shown below:

The original image on which the steps are performed:<br>
<img src="/images/canny/mr5.jpg" alt="caption needed" width="300" height="200"><br>

i) Blurring the image<br>
<img src="/images/canny/blur.png" alt="caption needed">

ii) Applying sobel filter to a get rough edges which are blurred<br>
<img src="/images/canny/sobel.png" alt="caption needed">

iii) Applying non-maxima suppression(NMS) to thin out the edges detected<br>
<img src="/images/canny/nms.png" alt="caption needed">

iv) Applying thresholding to remove unwanted edges and leave only those pixels that are to be concidered<br>
<img src="/images/canny/thresh.png" alt="caption needed">

v) Applying Hyterysis Thresholding to remove any inner edges as we are primarily looking of the major edges<br>
<img src="/images/canny/hyst.png" alt="caption needed">

For the code check the [github repo](https://github.com/deepayanbardhan/canny_edge).
