# PCA on Semantic Segmentation with Detectron2

PCA to calculate longest diagonal of C3S crystals from semantic segmentation with Detectron2 output.

## About

This repository is for an academic research in Federal University of Ceará, Campus Russas, Brazil.
It features the application of the PCA (Principal Component Analysis) algorithm on the masks of C3S crystals, segmented by an architecture of mask-RCNN. This repository contains code for the use of a specific architecture of mask-RCNN on the Detectron2 computer vision API.

## The research

The measurement of C3S crystals is an important part of a stage of portland cement production, the clynker microscopy. It is mostly done by analists, by examinating microscopic images of the clynker (a subproduct of cement) and measuring the crystals manually, in computers, with the help of drawing software. The research is about automating this, and there's where the PCA algorithm enters.

The algorithm showed good approximated results for the longest diagonal of the polygons segmented by the network of the C3S crystals, and a very good performance. This repository aims to show these results.

## Contents

This repository contains two python notebooks:

- *'PCA_with_Detectron_Output.ipynb'*;
- *'PCA_with_Detectron_Output_COLAB.ipynb'*

Plus a '*requirements.txt*' file and the folder '*pytorch/*'.

The first noteboook is in case you want to clone this repository and run it in your computer.
The second notebook is for running in Google Colab environment.

The '*pytorch/*' folder contains the pre-trained weights. They are needed so that we don't need to go through the process of training the network again. The weights are loaded by the network, which makes it ready for inference.

The '*requirements.txt*' file contains the names of the libraries that need to be installed in order to be used locally.

## Running in your machine

When running in your machine, use the *'PCA_with_Detectron_Output.ipynb'* notebook. The other one will only work in colab.
There's no need to manually install the libraries in '*requirements.txt*', for there's already code in the notebook that does that. 
Just make sure to have `pip` installed and well-updated.

After opening the notebook with a software from your choice, just run all cells in sequence.

## Running in Google Colab

When running in Colab, use the notebook *'PCA_with_Detectron_Output_COLAB.ipynb'*. The other one will not work properly there.
It's very recommended to run in Google Colab with GPU hardware accelerator. The GPU helps accelerating the inference process.

After opening the notebook in Colab, run all cells in sequence. 