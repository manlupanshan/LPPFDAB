# LPPFDAB
This repository contain two part：1.Code about how to use matlab connect the Zemax 2. Image reconstruction model bulid used the learnable physical priors and frequency domain attention 
# Prerequisites
1.)Matlab 2021a. Too early versions cannot be used. 

2.)zemax 18.9. Version 19 has compatibility issues and does not work well.

3.)python3

NVIDIA GPU + CUDA cuDNN

pytorch 1.7 or 1.9, the code is slightly different.

# Installation for python
requirements：
numpy ~= 1.14.3

scipy ~= 1.0.1

future ~= 0.16.0

matplotlib ~= 2.2.2

pillow ~= 5.0.0

opencv-python ~= 3.4.0

scikit-image ~= 0.14.0

pyaml

easygui

# Steps to use
1 Matlab connection zemax

Zemax Optic Studio open a file,  Click 'Programming'、'Interactive Extension' connect to the ZOS-API.
Use Matlab open 'MATLABZOSConnection.m' and run it. 

2 Use the genetic algorithm to dynamic optimization the phase mask

Use Matlab open 'MATLABStandaloneApplication.m' and add code to the '% Add your custom code here...'

3. Use psf which obtained by simulation or real photography to generate the encoded data. Or you can use a Optical System with phase mask get the  encoded data, but it is really really hard to complete.

4. Prepare the train and val data

5. Train the model, and use test it

# Code

Recently we are preparing a thesis, the specific code will be released after streamlining and organizing. 
   
