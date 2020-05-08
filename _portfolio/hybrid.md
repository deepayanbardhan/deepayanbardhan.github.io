---
title: "Hybrid Image Generation"
excerpt: "Blending images by averaging them in the frequency domain<br/><img src='/images/hybrid-cover.jpg'>"
collection: portfolio
---

## Brief Overview of the project

Hybrid Image is an image that can be perceived in one of two different ways. The view depends on the viewing distance. It is based on how human beings process visual input. It is very commonly used trick for optical illusions.

A popular example of a hybrid image is shown below:

<img src="/images/hybridimg.jpg" alt="caption needed" width="400" height="300">

Looking at the picture from a short distance, one can see a sharp image of a man, with only a hint of blurry distortion hinting at the presence of an overlaid image. Viewed from a distance in which the fine detail blurs, the unmistakable face of a cat emerges.

Similarly, in the example I have taken 2 images - First of the KFC logo and second of the Macdonald's mascot. They are converted to their frequency domain and then a weighted frequency image is generated with certain proportions of each image. That newly generated image is now converted back to the spatial domain using inverse fourier transform to represent the combined image.

Let us consider the 2 images below for the experiment:

<img src="/images/kfc.jpg" alt="caption needed" width="300" height="250"> | <img src="/images/mac.jpg" alt="caption needed" width="320" height="250">

This is the combined image finally generated when mixed in frequency domain

<img src="/images/hybrid.jpg" alt="caption needed" width="300" height="250">

This is the combined image finally generated when mixed in spatial domain

<img src="/images/mean.jpg" alt="caption needed" width="320" height="250">

We can tweak the combination ratio to get one of the image as more prominent one than the other. If we remove the high frequencies of one of the images and combine with the low frequency of the other image we can get a exact hybrid image.

As it can be clearly seen from the examples above, when it comes to blending images, using the frequency domain yields a much better result than compared to the spatial domain. Using the spatial domain might not lead to something visually meaningful as well. However, mixing in the frequency domain retains all the features. Thus, mixing images for the purpose of visual observations, is better visually if done using frequency domain.

My python code for this can be found [here](https://github.com/deepayanbardhan/hybrid-image-generation/blob/master/hybrid-image-generation.py)
