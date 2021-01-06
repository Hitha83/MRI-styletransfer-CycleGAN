# MRI-styletransfer-CycleGAN

One of the complicated tasks in medical imaging is to diagnose MRI(Magnetic Resonance Imaging). Sometimes to interpret the scan, the radiologist needs different variations of the imaging which can drastically enhance the accuracy of diagnosis by providing practitioners with a more comprehensive understanding.
But to have access to different imaging is difficult & expensive. With the help of deep learning, we can use style transfer to generate artificial MRI images of different contrast levels from existing MRI scans. This will help to provide a better diagnosis with the help of an additional image.

## Problem Statement
To build a Generative adversarial model(modified U-Net) which can generate artificial MRI images of different contrast levels from existing MRI scans.

Using CycleGAN to translate the style of one MRI image to another, which will help in better understanding of the scanned image. Using GANs ,create T2 weighted images from T1 weighted MRI image and vice-versa.

## Project Pipeline
The project pipeline can be briefly summarized in the following four steps:

Data Understanding: Here, you need to load the data and create the dataset for it.
Image Processing In this step, you will have to process the images using different steps
Model-Building & Training: This is the final step at which you have to create your Generators & Discriminators using a modified U-Net architecture(similar to CycleGAN). You also have to define the loss function & training step for model training.

## Understanding the dataset

The training dataset consist of two folders TrainT1 and TrainT2 which are T1-weighted and T2-weighted MRI scans resepectively.

## Image Processing

1.Process the images with normalisation

2.Data augmentation

3.Apply the function to both the datasets

4.Visualise the MRI images after processing

## Model Building & Training
The architecture of generator is a modified U-Net.

1.Create your Generator & Discriminator

2.Define the loss functions

3.Create the train_step function

