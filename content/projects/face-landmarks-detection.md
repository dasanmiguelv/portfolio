---
title: "Face Landmarks Detection using CNN"
description: "Can computers really understand the human face?"
dateString: May 2020
draft: false
tags: ["DL", "AI", "Python", "PyTorch"]
showToc: false
weight: 203
cover:
    image: "projects/face-landmarks-detection/cover.jpg"
--- 
### 🔗 [Colab Notebook](https://colab.research.google.com/drive/1TOw7W_WU4oltoGZfZ_0krpxmhdFR2gmb)
### 🔗 [Blog Post](../../blog/face-landmarks-detection)

## Description

In this project, I trained a neural network to localize key points on faces. **Resnet-18** was used as the model with some slight modifications to the input and output layer. The model was trained on the official **DLib Dataset** containing **6666 images** along with corresponding **68-point landmarks** for each face. Additionally, I wrote a custom data preprocessing pipeline in **PyTorch** to increase variance in the input images to help the model generalize better. The neural network was trained for 30 epochs before it reached the optima.

During inference, **OpenCV Harr Cascades** are used to detect faces in the input images. Detected faces are then cropped, resized to (224, 224), and fed to our trained neural network to predict landmarks in them. The predicted landmarks in the cropped faces are then overlayed on top of the original image.

users don’t have to install any dependency. They can just use the `docker run` command with the path to their clippings file along with their Notion API key and database ID.

In this project, I implemented the paper **[Show, Attend and Tell: Neural Image Caption Generation with Visual Attention](https://arxiv.org/abs/1502.03044)**. The neural network, a combination of **CNN** and **LSTM**, was trained on the **MS COCO** dataset and it learns to generate captions from images. 


> Presented in the 4th International and 19th National Conference on Machine and Mechanisms (**iNaCoMM 2019**)

> Published in the **Springer 2019**