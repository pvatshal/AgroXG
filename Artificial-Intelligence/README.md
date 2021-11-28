# AI Part of the Project

This directory consists the .ipynb files of different AI models along with their modified variants.

## Table of Content

- [Introduction](#introduction)
- [Information Regarding Dataset](#dataset-information)
- [Approach](#approach)
  - [Models Used](#models)
    - [EfficientNet-B0](#efficientnet-b0)
    - [InceptionResNet-V2](#inceptionresnet-v2)
  - [GLCM Feature Extractor](#glcm-feature-extractor)
- [Results](#results)
- [Discussion Over Results](#discussion-over-results)
  - [A.) Effect of model architecture](#a-effect-of-model-architecture)
- [Key-Takeaways](#key-takeaways)
- [References](#references)
- [Contribution](#contribution)

## Introduction

At the first, we tried VGG-19 with fully connected bottom layers where we recieved ~91.14% accuracy. After literature review, we planned to implement 2 models for the same task and select the best one performing. 

## Dataset Information

<table>
  <tr>
    <td align="center">Healthy Wheat</td>
    <td align="center">Wheat Loose Smut</td>
    <td align="center">Crown and Root Rot</td>
    <td align="center">Leaf Rust</td>
  </tr>
  <tr>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/01541.jpeg" width=250></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/0021.jpg" width=250></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/03621.jpg" width=250></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/0071.jpg" width=250></td>
  </tr>

## Approach

### Models

#### EfficientNet B0

<div align="center">
  <img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/block-diagram_EffNetB0.png" width=900 />
  <p> Block Diagram - EfficientNet-B0 </p>
</div>

[Implemented Model Structure Diagram](https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/Model_EffNetB0.png)


#### InceptionResNet V2

<div align="center">
  <img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/block-diagram_inceptionResnetV2.png" width=900 />
  <p> Block Diagram - InceptionResNet-V2 </p>
</div>

[Implemented Model Structure Diagram](https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/Model_EffNetB0.png)

## GLCM Feature Extractor

<div align="center">
  <img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/GLCM-features.JPG" width=900 />
  <p> GLCM - Features Formulas </p>
</div>


## Implementation 

<div align="center">
  <img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/Proposed-Model.jpeg" width=900 />
  <p> Proposed Model </p>
</div>

## Results

<table>
  <tr>
    <td></td>
    <td align="center">EfficientNet-B0</td>
    <td align="center">VGG19</td>
    <td align="center">InceptionResNet-V2</td>
  </tr>
  <tr>
    <td align="center" width=125> Accuracy Plots </td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/LossPlot_EffNetB0-Part1.png" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/LossPlot_VGG19.png" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/LossPlot_InceptionResNetV2.png" width=350></td>
  </tr>
 
  <tr>
    <td align="center" width=125 > Loss Plots </td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/AccPlot_EffNetB0-Part1.png" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/AccPlot_VGG19.png" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/AccPlot_InceptionResNetV2.png" width=350></td>
  </tr>
  
  
  <tr>
    <td align="center"  width=125> Categorical Accuracy Table </td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/CategoricalAccScoreTable.jpg" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/CategoricalAccScoreTable-VGG.jpg" width=350></td>
    <td><img src="https://github.com/caped-crusader16/AgroXG/blob/main/Artificial-Intelligence/CategoricalAccScoreTable-IncResv2.jpg" width=350></td>
  </tr>
</table>

## Discussion over Results

### A.) Effect of model architecture

## Key Takeaways

## References
-  L. A. Gatys, A. S. Ecker, and M. Bethge, “A Neural Algorithm of Artistic Style,” arXiv.org, 02-Sep-2015. [Online]. Available: [Link](https://arxiv.org/abs/508.06576). 
- S. Desai, “Neural Artistic Style Transfer: A Comprehensive Look,” Medium, 14-Sep-2017. [Online]. Available: [Link](https://medium.com/artists-and-machine-intelligence/neural-artistic-style-transfer-a-comprehensive-look-f54d8649c199).
- TensorFlow, “Neural Style Transfer: Creating Art with Deep Learning using tf.keras and eager execution,” Medium, 27-Sep-2018. [Online]. Available: [Link](https://medium.com/tensorflow/neural-style-transfer-creating-art-with-deep-learning-using-tf-keras-and-eager-execution-7d541ac31398)
- N. Kasten, “Art & AI: The Logic Behind Deep Learning ’Style Transfer’,” Medium, 12-Mar-2020. [Online]. Available: [Link](https://medium.com/codait/art-ai-the-logic-behind-deep-learning-style-transfer-1f59f51441d1).
- Leon A. Gatys, ”Image Style Transfer Using Convolutional Neural Networks”, . [Online]. Available: [Link](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf).

* * *

## Contribution

> [Manav Vagrecha](https://github.com/caped-crusader16), [Bhumiti Gohel](https://github.com/bhumiti28), [Vatsal Patel](https://github.com/pvatshal), [Jeet Shah](https://github.com/jds311)

## Support

Drop a ⭐ if you like our work. Contact any of us if you wish to have any suggestions or edits.


