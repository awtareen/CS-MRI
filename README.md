# Multi-layer Basis Pursuit for Compressed Sensing MR Image Reconstruction

# This repository contains a Compressed Sensing (CS) MRI framework for MRI undersampled image restoration for follwing paper.
A. Wahid, J. A. Shah, A. U. Khan, M. Ahmed and H. Razali, "Multi-Layer Basis Pursuit for Compressed Sensing MR Image Reconstruction," in IEEE Access, vol. 8, pp. 186222-186232, 2020, doi: 10.1109/ACCESS.2020.3028877.

## Overview

Compressive Sensing (CS) is a widely used technique in biomedical signal acquisition and reconstruction. The technique is especially useful for reducing acquisition time for magnetic resonance imaging (MRI) signal acquisitions and reconstruction, where effects of patient fatigue and Claustrophobia need mitigation. In addition to improving patient experience, faster MRI scans are important for time sensitive imaging, such as functional or cardiac MRI, where target movement is unavoidable. Inspired from recent research works on multi-layer convolutional sparse coding (ML-CSC) theory to model deep neural networks, this work proposes a multi-layer basis pursuit framework which combines the benefit from objective-based CS reconstructions and deep learning-based reconstruction by employing iterative thresholding algorithms for successfully training a CS-MRI restoration framework on GPU and reconstruct test images using parameters of the trained model. Extensive experiments show the effectiveness of the proposed framework on four MRI datasets in terms of faster convergence, improved PSNR/SSIM, and better restoration efficiency as compared to the state of the art frameworks with different CS ratios.

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

