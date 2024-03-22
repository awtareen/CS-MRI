# Multi-layer Basis Pursuit for Compressed Sensing MR Image Reconstruction

## This repository contains a Compressed Sensing (CS) MRI framework for MRI undersampled image restoration.

## Overview

Compressed Sensing MRI (CS-MRI) is a technique that can significantly accelerate MRI acquisition times by undersampling the k-space data. CS-MRI algorithms are designed to reconstruct high-quality images from undersampled k-space data by exploiting the sparsity of the MRI image in transform domain.

# Repository Contents

This repository contains the following files:
-	train.ipynb: Script for training the CS-MRI model
-	test.ipynb: Script for testing the CS-MRI model
-	testdata: Directory containing MRI datasets
-	masks_dir: Directory containing k-space sampling masks
-	Models dir : Directory containng saved papremeters after training ends.

# Datasets

The train and test images of Brain MRI are taken from ISTA-Net-PyTorch: https://github.com/jianzhangcs/ISTA-Net-PyTorch alongside additional datasets of Knee MR form HKL Kuala Lumpur for the research work.



# Usage:

To train the CS-MRI model, run the relevant Brain and Knee train files. after the paramters are saved, run test files to restore test images. The test files takes the parameters saved in models directory to restore images.



# Citation

Please cite the following paper if you use this work:

@article{wahid2020multi,
  title={Multi-layer basis pursuit for compressed sensing MR image reconstruction},
  author={Wahid, Abdul and Shah, Jawad Ali and Khan, Adnan Umar and Ahmed, Manzoor and Razali, Hanif},
  journal={IEEE Access},
  volume={8},
  pages={186222--186232},
  year={2020},
  publisher={IEEE}
}

