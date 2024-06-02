# Machine Learning Role on Modelling

This repository serves as a summary of our ML work on Google Colab. The following notebooks are reflected from our workspace on Google Drive at [this link](https://drive.google.com/drive/folders/1RGJoxtWvnND563kQw57r1kUIIQe5HLzu). Do note that not all files are pushed to GitHub but only some important files.

## Pre-project Exploration
We do simple implementation about proof of concept using Laplacian method. The notebook is available at [Project_Proposal.ipynb](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Project_Proposal.ipynb)

## Exploration
The complete summary of each model performance is available at [[0]_Model_Performance_Summary.ipynb](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/%5B0%5D_Model_Performance_Summary.ipynb), but here are some key notes:

- Only plain deep learning or basic CNN [Plain_Deep_Learning_Approach.ipynb](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Plain_Deep_Learning_Approach.ipynb) (best accuracy 77.08%)
- Manually find threshold that seperate each class [Hand Designed Approach](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Hand_Designed_Approach.ipynb) (best accuracy <70%)
- Embed object detection model to main model and train on this big model [End-to-End Deep Learning Approach](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/End_to_End_Deep_Learning_Approach.ipynb) (best accuracy 65.79%)
- Use InceptionV3 (mixed3) pre-trained model with custom layer to calculate variance of Laplacian [Transfer Learning + Variance](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Transfer_Learning_%2B_Variance_Approach.ipynb) (best accuracy 90.35%)
- Use InceptionV3 (mixed3) pre-trained model with custom layer to preprocess input using Fast Fourier Transform [FFT + Transfer Learning](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/FFT_%2B_Transfer_Learning_Approach.ipynb) (best accuracy 80.70%)
- Use InceptionV3 (mixed3) pre-trained model with custom layer to calculate variance of Laplacian and preprocess input using Fast Fourier Transform [FFT + Variance + Transfer Learning](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_FFT_and_Variance.ipynb) (best accuracy 54.39%)
- Use InceptionV3 (mixed3) pre-trained model with custom loss that weight blur higher than other classes [TL with Custom Weighted Loss.ipynb](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/FFT_%2B_Transfer_Learning_Approach.ipynb) (best accuracy 80.70%)
- Use InceptionV3 (all layers) pre-trained model with fine-tuning [Transfer Learning with InceptionV3](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/TL_with_InceptionV3.ipynb) (best accuracy 95.61%) ✴️

Note: Best accuracy is calculated on the dataset provided by Braincore available at [this link](https://drive.google.com/drive/u/5/folders/1clhOFdWTYSxA_DwNp-4_B9NvYzizU856).

## Performance Exploration (Trial and Error)
1. [Transfer Learning + Deep Learning Approach - Test Random Initialization](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Transfer_Learning_%2B_Variance_Approach_Test_Random_Initialization.ipynb)
2. [TL_with_InceptionV3_(mixed3)_Retrained.ipynb](https://github.com/Bangkit-Capstone-C241-BB01/BlurOrBokeh_ML_All/blob/main/Salinan_dari_Transfer_Learning_Approach.ipynb)

Summary of each attempt is available at [this link](https://docs.google.com/document/d/1_wMoe67zms_sX22tSYWRSqcihyM6Hmtmuvmzmk9k07Q)

## Current Exploration
[Completed]
