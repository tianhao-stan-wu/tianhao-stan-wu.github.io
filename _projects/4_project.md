---
layout: page
title:  Music Genre Classification
description: ML class project
img: assets/img/project4/spectro.png
importance: 1
category: class project
---

Collaborator: &nbsp;[Lorena Yan](https://tianyi-lorena-yan-me.web.app/) &nbsp;&nbsp;&nbsp;[Ryan Wang](https://www.linkedin.com/in/ryanyxw/)

[[Project Github]](https://github.com/Lorenayannnnn/csci467_music_genre_classification)

<br>
Abstract:

In this project, we address the task of music genre classification (MGC) with machine learning methods. 

The baseline method utilizes softmax regression and achieves a 24.24% test accuracy. Further inspection into the results reveals the need for techniques that can capture more fine-grained details while being more perceptive of global patterns. 

The second method involves a single CNN model that achieves 57.5% test accuracy. Then we ensemble several CNN models together and make predictions using the majority vote, which resulted in a 63.6% test accuracy. Both these CNN-based approaches struggle to classify spectrograms not representative of their genres. In these cases, models fail to extract useful information from the spectrograms. 

The third approach is to train Wav2Vec pretrained models with an ensemble-based learning method. More specifically, we combine a weaker model of smaller number of parameters for capturing biases with a main model for capturing more robust features together. This approach obtains a test accuracy of 74.8%. Although Wav2Vec2-based model still faces difficulties in identifying music genres with high instrumentation and melody variations (such as country music), this attention-based model achieves a relatively higher accuracy compared to the aforementioned two methods.

<br>

Complete [final report](/assets/pdf/project4/report.pdf) here
