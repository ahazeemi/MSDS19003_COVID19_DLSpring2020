# MSDS19003_COVID19_DLSpring2020

This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes

## Dataset
https://drive.google.com/a/itu.edu.pk/uc?id=1-HQQciKYfwAO3oH7ci6zhg45DduvkpnK&export=download%27

# Part 1 

## Models:


### Training on all layers:

res18_entire.pth (https://drive.google.com/file/d/1ncpcMC1b1hRQH8JoOQPYWdoyAGUAApnU/view?usp=sharing)

vgg16_entire.pth (https://drive.google.com/file/d/1-2UXfpnjJG2uNoes0upuOKKjdYuzX14u/view?usp=sharing)

### Training on fully connected layers only:

res18_FC_Only.pth (https://drive.google.com/file/d/1-1m_hyohkuPjB7Bm5ec-JTfOdMyc7HNY/view?usp=sharing)

vgg16_FC_Only.pth (https://drive.google.com/file/d/1--Tj8lepeMVBhjLGD-KyswcUtxpxf1C7/view?usp=sharing)

## Results (ResNet-18 and VGG-16 models trained on Chest X-Rays dataset)

### ResNet-18 Model 

**Accuracy on test data:**
94.5%

**Confusion Matrix:**
|         |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 538 | 77 |
| Actual Normal      | 5      |   880 |

### VGG-16 Model
**Accuracy on test data:**
94.93%

**Confusion Matrix:**
|         |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 546 | 69 |
| Actual Normal      | 7      |   878 |


## Results (Transfer learning on ResNet-18 and VGG-16 models trained on ImageNet - training only the fully connected layers)

### ResNet-18 Model 

**Accuracy on test data:**
93%

**Confusion Matrix:**
|         |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 528 | 87 |
| Actual Normal      | 19      |   866 |

### VGG-16 Model
**Accuracy on test data:**
93.06%

**Confusion Matrix:**
|         |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 534 | 81 |
| Actual Normal      | 23      |   862 |



### Summary

|         |Whole Network Training       | FC layer training  |
| ------------- |:-------------:| -----:|
| ResNet      | 94.5 | 93 |
| VGG      | 94.93     |   93.06 |


# Part 2

## Dataset
https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view?usp=sharing


## Models:

vgg16_focal_loss.pth: https://drive.google.com/file/d/1-8VWoJI0-xKAARyNlHSbM6FsvcRxp0s5/view?usp=sharing
res18_focal_loss.pth https://drive.google.com/file/d/1-AmvECf0su2LFlD-odsgTLHEMebp8Kvc/view?usp=sharing

## Results (without focal loss)

### VGG-16
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/task1vgg.png" width="350">

### ResNet-18
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/task1resnet.png" width="350">

## Results (with focal loss)

### VGG-16

#### F1-Score curve
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/task2vgg.png" width="350">

#### Confusion Matrix (multi-label)
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/confusion_matrix_vgg_task2.png" width="350">

### ResNet-18

#### F1-Score curve
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/task2resnet.png" width="350">

#### Confusion Matrix (multi-label)
<img src="https://github.com/ahazeemi/MSDS19003_COVID19_DLSpring2020/blob/master/Images/confusion_matrix_resnet_task2.png" width="350">


