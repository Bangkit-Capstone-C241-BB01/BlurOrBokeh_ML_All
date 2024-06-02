# Machine Learning Role on Modelling

This repository serves as a summary of our ML work on Google Colab. The following notebooks are reflected from our workspace on Google Drive at [this link](https://drive.google.com/drive/folders/1RGJoxtWvnND563kQw57r1kUIIQe5HLzu). Do note that not all files are pushed to GitHub but only some important files.

## Pre-project Exploration
We do simple implementation about proof of concept using Laplacian method. The notebook is available at [Project Proposal](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Project_Proposal.ipynb)

## Exploration
The complete summary of each model performance is available at [Model Performance Summary](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/%5B0%5D_Model_Performance_Summary.ipynb), but here are some key notes:

| Notebook Filename | Description | Best Accuracy (%) |
|-----------------|-----------------|-----------------|
| [TL with InceptionV3](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_InceptionV3.ipynb) | Use InceptionV3 (all layers) pre-trained model with fine-tuning | 95.61 ✴️ |
| [Plain Deep Learning Approach](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Plain_Deep_Learning_Approach.ipynb) | Only plain deep learning or basic CNN | 77.08 |
| [End-to-End Deep Learning Approach](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/End_to_End_Deep_Learning_Approach.ipynb) | Embed object detection model to main model and train on this big model | 65.79 |
| [TL with InceptionV3 (mixed3)](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_InceptionV3_(mixed3).ipynb) | Use InceptionV3 (until layer mixed3) pre-trained model with fine-tuning | 85.96 |
| [TL with Variance](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_Variance.ipynb) | Use InceptionV3 (mixed3) pre-trained model with custom layer to calculate variance of Laplacian | 90.35 |
| [TL with FFT](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_FFT.ipynb) | Use InceptionV3 (mixed3) pre-trained model with custom layer to preprocess input using Fast Fourier Transform | 80.70 |
| [TL with FFT and Variance](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_FFT_and_Variance.ipynb) | Use InceptionV3 (mixed3) pre-trained model with custom layer to preprocess input using Fast Fourier Transform and calculate variance of Laplacian | 54.39 |
| [TL with Custom Weighted Loss](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_Custom_Weighted_Loss.ipynb) | Use InceptionV3 (mixed3) pre-trained model with custom loss that weights misclassified on blur class higher than other classes | 83.30 |
| [Hand Designed Approach](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Hand_Designed_Approach.ipynb) | Manually find threshold that seperate each class, however, this idea was dropped due to its unfavorable spread on scatter plot | Unknown |

Note: Best accuracy is calculated on the dataset provided by Braincore available at [this link](https://drive.google.com/drive/u/5/folders/1clhOFdWTYSxA_DwNp-4_B9NvYzizU856).

## Performance Exploration (Trial and Error)
1. [Transfer Learning + Variance Approach - Test Random Initialization](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Transfer_Learning_%2B_Variance_Approach_Test_Random_Initialization.ipynb)
2. [TL with InceptionV3 (mixed3) Retrained](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_InceptionV3_(mixed3)_Retrained.ipynb)

Summary of each attempt is available at [this link](https://docs.google.com/document/d/1_wMoe67zms_sX22tSYWRSqcihyM6Hmtmuvmzmk9k07Q)

## Final Model Performance Overview
![Accuracy and Loss](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Images/Accuracy%20and%20Loss.png)

![Confusion Matrix on Test Set](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Images/Confusion%20Matrix%20on%20Test%20Set.png)
![Confusion Matrix on Validation Set](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Images/Confusion%20Matrix%20on%20Validation%20Set.png)

## Current Exploration
[Completed]
