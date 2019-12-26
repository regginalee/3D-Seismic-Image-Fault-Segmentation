# 3D-Seismic-Image-Fault-Segmentation
![demo](https://github.com/Jun-Tam/3D-Seismic-Image-Fault-Segmentation/raw/master/images/demo_application.gif)

### Summary
This code demonstrates fault probability prediction on 3D seismic images using 3D Shallow U-Net model.
A large number of synthetic 3D seismic images are generated by randomly choosing parameters
to represent geological deformations, fault strike/dip, number of faults, central frequency of wavelet, etc.
This techinique has advantage against human labeling as fault labeling can be done automatically during data generation process.

### Configuration
```
GPU: NVIDIA GeForce GTX 1080 Ti
Model architecture: Shallow 3D U-net
Training Data: 200
Validataion Data: 20
Batch size: 3 (Data Augmentation)
Data Augmentation: z-axis rotation (Randomly choose from 0, 90, 180, 270 deg.)
Feature size: 128 x 128 x 128
```

### Field Data Application
Netherlands Offshore F3 Block (dGB Open Seismic Repository)
https://terranubis.com/datainfo/Netherlands-Offshore-F3-Block-Complete

### Reference
FaultSeg3D: Using synthetic data sets to train an end-to-end convolutional neural network for 3D seismic fault segmentation,Xinming Wu et al., Geophysics, 2019
