# MSDS19003_COVID19_DLSpring2020

This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes

## Dataset
https://drive.google.com/a/itu.edu.pk/uc?id=1-HQQciKYfwAO3oH7ci6zhg45DduvkpnK&export=download%27

## Results (ResNet-18 and VGG-16 models trained on Chest X-Rays dataset)

### ResNet-18 Model 

**Accuracy on test data:**
94.5%

**Confusion Matrix:**
|         |Predicted Normal        | Predicted Infected  |
| ------------- |:-------------:| -----:|
| Actual Normal      | 538 | 77 |
| Actual Infected      | 5      |   880 |

### VGG-16 Model
**Accuracy on test data:**
94.93%

**Confusion Matrix:**
|         |Predicted Normal        | Predicted Infected  |
| ------------- |:-------------:| -----:|
| Actual Normal      | 546 | 69 |
| Actual Infected      | 7      |   878 |


## Results (Transfer learning on ResNet-18 and VGG-16 models trained on ImageNet - training only the fully connected layers)

### ResNet-18 Model 

**Accuracy on test data:**
93%

**Confusion Matrix:**
|         |Predicted Normal        | Predicted Infected  |
| ------------- |:-------------:| -----:|
| Actual Normal      | 528 | 87 |
| Actual Infected      | 19      |   866 |

### VGG-16 Model
**Accuracy on test data:**
93.06%

**Confusion Matrix:**
|         |Predicted Normal        | Predicted Infected  |
| ------------- |:-------------:| -----:|
| Actual Normal      | 534 | 81 |
| Actual Infected      | 23      |   862 |
