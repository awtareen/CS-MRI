# Multi-layer Basis Pursuit for Compressed Sensing MR Image Reconstruction

# This repository contains a Compressed Sensing (CS) MRI framework for MRI undersampled image restoration for follwing paper.
A. Wahid, J. A. Shah, A. U. Khan, M. Ahmed and H. Razali, "Multi-Layer Basis Pursuit for Compressed Sensing MR Image Reconstruction," in IEEE Access, vol. 8, pp. 186222-186232, 2020, doi: 10.1109/ACCESS.2020.3028877.

## Overview

Deep Learning-based Compressive Sensing MRI Reconstruction

This repository provides the code and details for a novel multi-layer basis pursuit framework for Compressive Sensing (CS) Magnetic Resonance Imaging (MRI) reconstruction. The framework combines the strengths of objective-based CS reconstructions and deep learning by leveraging iterative thresholding algorithms. 
This approach enables:

Faster MRI Scans: Reduce acquisition times, mitigating patient discomfort and enabling time-sensitive imaging.
Improved Image Quality: Achieve superior Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index Measure (SSIM) compared to state-of-the-art methods.
Efficient Reconstruction: Our framework demonstrates faster convergence and improved reconstruction efficiency for various CS ratios across four MRI datasets.
Inspired by recent advancements in multi-layer convolutional sparse coding (ML-CSC) theory, our work proposes a deep learning-based CS-MRI restoration framework trained on GPUs.

This repository welcomes contributions and aims to be a valuable resource for researchers exploring deep learning applications in CS-MRI reconstruction.

# Repository Contents

This repository contains the following files:
-	train.ipynb: Script for training the CS-MRI model
-	test.ipynb: Script for testing the CS-MRI model
-	testdata: Directory containing MRI test images.
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

