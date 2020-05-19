# Ship Detection using Satellite Imagery

The aim of this project is to accurately classify satellite images that contain ships and furthermore detect the ships on a pixel level in relation to the image as a whole.

Ship detection is a vital aspect of maritime surveillance as it allows the monitoring of maritime traffic, illegal fishing and sea border activities. This is typically carried out using Automated Identification Systems (AIS) which use VHF radio frequencies to wirelessly broadcast the ships location, destination and identity to nearby receiver devices on other ships and land-based systems. 

AIS are very effective at monitoring ships which are legally required to install a VHF transponder, but fail to detect those which are not, and those which disconnect their transponder. So how do you detect these ‘dark’ ships? Using satellite detection!

- marwinkalo@gmail.com
- https://www.linkedin.com/in/marwan-kalo/


### Executive Summary

![Test Image](./images/training_image_ships.png)

The use of satellite detection of ships will significantly bolster the arsenal of stakeholders in maritime surveillance. Used in conjunction with AIS, satellite detection can flag previously unidentified ships and build up a more accurate picture of the world's seas and oceans that are becoming ever more crowded. Some key challenges that this form of surveillance will attempt to tackle are: illegal fishing operations, maritime accident identification and illegal border immigration. 
In the last decade, numerous companies have deployed survelliance satellites in an attempt to bolster their monitoring capabilities. In turn, detection algorithms such as the one I propose will offer an automated approach to analysing the imagery fed back. 

To first identify whether or not there are ships in a satellite image is the first piece of the puzzle and I tackled this with an image classification approach. Using convolutional neural networks, I was able to correctly identify images containing ships 98% of the time. Next, the objective was to detect and delineate the ships from the image background to identify the ships more accurately, on a pixel-level. 

My final convolutional neural network model for the first stage consisted of four convolutional and pooling layers along with two fully-connected, dense layers. I also included five dropout layers to decrease the model's complexity and in turn reduce overfitting. It performed very strongly on the training and test data - both 98%. The data for the first part was taken from Planet's Open California dataset (https://www.kaggle.com/rhammell/ships-in-satellite-imagery).

The second part of the project involved using a region-based convolutional neural network........


Lastly, you say in one or two sentences why this matters. 
For example, now as opposed to before this data analysis, you can now predict X better than Y. 

The goal of this project was to create a `regression/classification` model that was able to predict `what you set out to do`.

> If you are able to swap out the text here with what your case example is you will demonstrate the following:
> 1. You get why what you're doing 'matters'
> 2. You are able to take ill defined problems and turn them into something a data scienst can solve
> 3. You show off your analystical and modeling chops.
> 4. You are able to communicate technical things you do.

### More Information

Below your Executive Summary, you can document whatever you feel would be of interest to a future employer.
Here I would especially suggest diving a bit deeper into your methodology and including images that you are proud of from the project. 
Remember, that people will probably judge your github project page within 45 seconds tops, you want it to look as clean as possible. 

Write documentation that looks like someone you would want to work with.

### Show Off Your Data Viz

![Everyone Likes a Pairplot](figures/seaborn-pairplot-3.png)

> Image taken from `seaborn` [documentation](https://seaborn.pydata.org/generated/seaborn.pairplot.html)

**DO NOT PUT THE GOOD BITS OF YOUR PROJECT BURRIED AWAY AT THE BOTTOM OF YOUR README, YOU ARE NOT WRITING A DETECTIVE NOVEL**


