## Ship image detection model

This project is a simple image classification model for identifying ships in satellite imagery. The model was made in Jupyter Notebook in an Anaconda distribution, and uses conda for package management.

The dataset used is available at https://www.kaggle.com/datasets/rhammell/ships-in-satellite-imagery/data, and should be downloaded locally and the address saved as images_path in the model.ipynb file.
The dataset consists of 4000 80x80px images in RGB colors, sourced from satellite imagery of the San Francisco Bay and the San Pedro Bay in California provided by Planet.com. 1000 of these include a ship, the remaining 3000 don't; the file name for each image includes the coordinates, Planet's scene ID for the image it's sourced from, and label of whether the image contains a ship or not.


## What's next

As it is now, the model is functional and has an acceptable accuracy rate. The accuracy could likely be improved through more complex hyperparameter tuning and adjustements to the model architecture used.
Additionally, the model could adjusted from what it currently is to be a program capable of processing any provided satellite image and identifying ships in it - adding this would primarily require an extra step be added for separating an image into 80x80 squares (possibly doing so in multiple ways if the image dimensions aren't perfectly divisible by 80), and adding a way of marking the detected ships on the originally submitted image together with the coordinates they're located at. This version of the model could be utilised for predicting ship movement based on changes in location over time, based on satelite image data collected over a period of time.
