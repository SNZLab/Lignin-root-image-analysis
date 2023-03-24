# Lignin-root-image-analysis

Guide: How to run the notebook for estimating the amount of lignin in Arabidopsis seedlings through the virtual machine
1.	Open a terminal on your notebook.
2.	Log into the virtual machine by i) running “ssh username@ip-address”, where username and IP-address must be replaced accordingly, and ii) entering the password for the chosen user. Now you should be logged in.
3.	Now, the base environment is activated. However, we want to activate the environment root-env, in which all necessary Python libraries are already installed. Activate the conda environment root-env by running “conda activate root-env”. If successful, (root-env) instead of (base) will appear to the left of the username.
4.	Now, run “jupyter notebook”. Copy the URL starting with http://..., replace the "tuwzu6a-plantdevpostgres" with the IP-address and open it in the browser of your choice.
5.	You will now see all files stored in the virtual machine (in the directory you are currently located, i.e., /home/ovule). Open the folder Lignin-root-image-analysis by clicking on it.
6.	Upload all root images you want to analyse in the folder /images/root_images and delete old ones. Also, make sure to empty the folder /images/root_images_bin, where the binarized images of the uploaded root images will be stored.
7.	Open the notebook Image_analysis.ipynb. Now follow the instructions in the notebook, i.e., run the first code cell to import all necessary libraries, run the second code cell, which contains all necessary function definitions for downstream analysis, and finally, run the third cell to analyse all images saved in /images/root_images. The last cell can be run optionally, in case you wish to analyse one specific image only. Make sure to specify the correct path.
8.	An Excel file containing the grayscale intensities over the stained region, the cropped region and the whole image as well as the area of the stained region and the cropped region (in number of pixels) for all analysed images is now stored in the folder Lignin-root-image-analysis. Download it to view it in Excel. Additionally, in the folder /images/root_images_bin, you can now find the binarized versions of the analysed root images. Just download the folder or choose specific images for download.
9.	If you are done, close all tabs. Go back to your terminal and press "ctrl+c" twice. Type "exit" and press enter to disconnect from the virtual machine.
