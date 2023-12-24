---
title: CalorMe
draft: false
tags:
 - keras
 - tensorflow
 - flutter
 - computer-vision
---

##### [Read my article here](https://arielycliu.medium.com/classifying-food-with-computer-vision-a473249cf2f2)

##### [Check out the Github here](https://github.com/arielycliu/calorme)

![CalorMe Demo](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/001/661/873/datas/gallery.jpg)


## 🔍What it does
CalorMe is a mobile app that allows users to take their nutritional choices into their own hands. Users simply take or upload a picture of their next meal to the CalorMe platform and, with the help of computer vision and deep learning, users can see important nutritional information, such as calorie count and macronutrient breakdown. 

---


## 🔨How we built it
**For the AI portion:**
We used Keras with TensorFlow and coded everything in Jupyter notebooks. I used the data from the Food-101 dataset [food dataset](https://www.kaggle.com/kmader/food41?select=images). 

We started off with our own convolutional neural network but quickly realized we would achieve better results with shorter training times by using transfer learning. We tried three different bases of different pre-trained models: InceptionV3, VGG16, and MobileNetV2 [Keras Pre-trained models](https://keras.io/api/applications/). InceptionV3 worked the best so we used this base and continued to optimize it to achieve a validation accuracy of 86% and a training accuracy of 97%. 

**For the Mobile App portion:**
We created the mobile app using Google's Flutter framework. Flutter enables you to create native-looking and performing apps for Android, iOS, Windows, and even the web all from one codebase. 

Creating the front-end with Flutter was relatively easy, with an MVP being able to be produced in just a few hours. Flutter had packages for image selection and specific UI elements, allowing us to develop without recreating the wheel. The classification of the uploaded picture is done through TensorFlow Lite (TFLite), a package that allowed us to integrate our trained neural network with the app. Finally, once the image is classified, an API request is made via HTTPS to Edamam, providing the nutritional information in a JSON string. This is finally deserialized to a map object and the relevant information is retrieved and presented to the user. 