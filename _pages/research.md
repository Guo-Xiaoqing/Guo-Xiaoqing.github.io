---
#layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

# Learning from Massive Unlabeled Data

Since the data distribution bias depends on the sample size, the scarce labeled data distribution often deviates from the desired one due to the small sample size, which inevitably leads to the overfitting problem of the optimized model. Fortunately, the unlabeled data is abundant and easy to access in real clinical practice. To make adequate use of unlabeled data along with scarce labeled data, we first investigate the semi-supervised learning (SSL) methods in medical image diagnosis and segmentation. These SSL methods are capable of building better models that compensate for the lack of labeled training data, and are demonstrated to be beneficial for enhancing the generalizability of automated medical image analysis models. Moreover, we rethink the overfitting problem caused by scarce labeled data and propose a new strategy, coined Labeled-to-unlabeled Distribution Translation (L2uDT), by taking the advantages of data augmentation and SSL methods, aiming at alleviating the labeled data distribution bias problem. 

#### Relevant Work/Publications:
* <a href="https://ieeexplore.ieee.org/document/9541376" target="_blank">Semantic-oriented Labeled-to-unlabeled Distribution Translation for Image Segmentation</a> [TMI'22]
* <a href="https://doi.org/10.1016/j.media.2020.101733" target="_blank">Semi-supervised WCE Image Classification with Adaptive Aggregated Attention</a> [MedIA'20]
* <a href="https://ieeexplore.ieee.org/document/9098417" target="_blank">Complementary Network with Adaptive Receptive Fields for Melanoma Segmentation</a> [ISBI’20]

![Words](https://github.com/Guo-Xiaoqing/Guo-Xiaoqing.github.io/raw/master/images/massive_unlabeled_data.png)


# Learning with Scarce Labeled Data

Deep learning methods generally require large amounts of annotated data to prevent overfitting problem, which is a common concern when the model fitted to a limited training set results in a poor generalization ability to test data. However, high-quality annotated datasets are scarce in the medical domain, especially in *medical image segmentation* and *rare disease diagnosis*. Because manual pixel-wise annotations in medical image segmentation requires professional medical knowledge as well as a high degree of concentration, and it is hard to collect sufficient training data for rare diseases in practice. Consequently, the lack of abundant annotated datasets becomes a bottleneck to deep learning-based methods in medical image analysis. We are interested in learning with scarce labeled data through data augmentation and few-shot learning.

#### Relevant Work/Publications:
* <a href="https://www.sciencedirect.com/science/article/abs/pii/S1361841522000469" target="_blank">Non-equivalent images and pixels: confidence-aware resampling with meta-learning mixup for polyp segmentation</a> [MedIA'22]
* <a href="https://link.springer.com/chapter/10.1007/978-3-031-16437-8_49" target="_blank">Disentangle then Calibrate: Selective Treasure Sharing for Generalized Rare Disease Diagnosis</a> [MICCAI'22]
* <a href="https://ieeexplore.ieee.org/document/9305717" target="_blank">Learn to Threshold: ThresholdNet with Confidence-Guided Manifold Mixup for Polyp Segmentation</a> [TMI’21]

![Words](https://github.com/Guo-Xiaoqing/Guo-Xiaoqing.github.io/raw/master/images/scarce_labeled_data.png)

