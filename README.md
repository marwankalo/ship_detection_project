# Ship Detection using Satellite Imagery

![Ships Present](https://github.com/marwankalo/ship_detection_project/blob/master/images/training_image_ships.png)

## Table of Contents

[1: Image Classification Notebook](https://github.com/marwankalo/ship_detection_project/blob/master/notebooks/ship_detection_stage_1.ipynb)

[2: Presentation](https://github.com/marwankalo/ship_detection_project/blob/master/reports/presentation_draft.pdf)

[3: Introduction](#Introduction)

[4: File Descriptions](#File-Descriptions)

[5: Executive Summary](#Executive-Summary)

[6: References](#References)

## Introduction

The aim of this project is to accurately classify satellite images that contain ships and furthermore detect the ships on a pixel level in relation to the image as a whole.

Ship detection is a vital aspect of maritime surveillance as it allows the monitoring of maritime traffic, illegal fishing and sea border activities. This is typically carried out using Automated Identification Systems (AIS) which use VHF radio frequencies to wirelessly broadcast the ships location, destination and identity to nearby receiver devices on other ships and land-based systems. 

AIS are very effective at monitoring ships which are legally required to install a VHF transponder, but fail to detect those which are not, and those which disconnect their transponder. So how do you detect these ‘dark’ ships? Using satellite detection!

- marwinkalo@gmail.com
- https://www.linkedin.com/in/marwan-kalo/

## File Descriptions

ship_detection_stage_1.ipynb - Notebook containing all of the steps for the initial image classification model

images - A directory containing images used to present my findings

reports - A directory containing the final memo and powerpoint presentaion

For reproducibility of this notebook please clone it onto your local device and visit the following sites for the data:

[Stage 1]((https://www.kaggle.com/rhammell/ships-in-satellite-imagery)

[Stage 2](https://www.kaggle.com/c/airbus-ship-detection/data)



## Executive Summary

The use of satellite detection of ships will significantly bolster the arsenal of stakeholders in maritime surveillance. Used in conjunction with AIS, satellite detection can flag previously unidentified ships and build up a more accurate picture of the world's seas and oceans that are becoming ever more crowded. Some key challenges that this form of surveillance will attempt to tackle are: illegal fishing operations, maritime accident identification and illegal border immigration. 
In the last decade, numerous companies have deployed survelliance satellites in an attempt to bolster their monitoring capabilities. In turn, detection algorithms such as the one I propose will offer an automated approach to analysing the imagery fed back. 

To first identify whether or not there are ships in a satellite image is the first piece of the puzzle and I tackled this with an image classification approach. Using convolutional neural networks, I was able to correctly identify images containing ships 98% of the time. Next, the objective was to detect and delineate the ships from the image background to identify the ships more accurately, on a pixel-level. 

My final convolutional neural network model for the first stage consisted of four convolutional and pooling layers along with two fully-connected, dense layers. I also included five dropout layers to decrease the model's complexity and in turn reduce overfitting. It performed very strongly on the training and test data - both 98%. The data for the first part was taken from Planet's Open California dataset (https://www.kaggle.com/rhammell/ships-in-satellite-imagery).

The second part of the project involved using a region-based convolutional neural network........


With the models I have proposed, maritime surveillance can now be carried out using a two pronged approach through the use of traditional AIS tracking as well as satellite detection.

In future, I would like to continue the project using geographical features to be able to simultaneously plot the position of each ship on a map to assist with tracking. Additionally, with access to AIS surveillance data, I would be able to build a model that identifies 'dark' ships - those that are picked up using satellite detection but not using AIS.

## References

[1 - Satellite Imagery can help on Maritime Surveillance](https://news.mongabay.com/2019/08/no-place-to-hide-for-illegal-fishing-fleets-as-surveillance-satellites-prepare-for-lift-off/)

[2 - ‘No place to hide’ for illegal fishing fleets](https://geocento.com/satellite-imagery-case-studies/satellite-imagery-can-help-on-maritime-surveillance/)
