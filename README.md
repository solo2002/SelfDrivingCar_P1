# **Finding Lane Lines on the Road** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project you will detect lane lines in images using Python and OpenCV.  OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.  

To complete the project, two files will be submitted: a file containing project code and a file containing a brief write up explaining your solution. We have included template files to be used both for the [code](https://github.com/udacity/CarND-LaneLines-P1/blob/master/P1.ipynb) and the [writeup](https://github.com/udacity/CarND-LaneLines-P1/blob/master/writeup_template.md).The code file is called P1.ipynb and the writeup template is writeup_template.md 


Reflection
---

1. Describe the pipeline
    (1) Convert to gray scale
    (2) Apply Gaussian smoothing
    (3) Define parameters for Canny and apply
    (4) Select the region of interest
    (5) Hough line transformation
    (6) Find the fit line via linear regression
    (7) Draw lines

2. Identify any shortcomings
    (1) When selecting the region of interest, the size parameter is hard coded.
    (2) This pipeline works for two test videos, but fails when testing challenge videos.
3. Suggest possible improvements
    (1) Need to test more parameter setting to find a better combination.
    (2) Instead of linear regression (first order), higher order (for curve line) may have a better performance.

