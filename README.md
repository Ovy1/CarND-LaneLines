**Finding Lane Lines on the Road**
** Running the Code **

    Simply open P1.ipynb in Jupyter Notebook
    Execute all of the code
    Video's and images will be displayed after running


---
This project implements a pipeline to process an image or video of a car driving on a road with lane lines. The code will identify the lane lines and draw red lines over the original image/video.

### Reflection

The pipeline consist of 5 steps:

a) converting the images to grayscale,
b) Applying Gaussian smoothing function
c) Applying Canny Edge Detector function
d) Creating masked edges for ROI (region of interest)
e) Applying Hough Line Detector function
f) Drawing lane lines on the original image
In order to draw a single line on the left and right lanes, I modified the
draw_lines() function by using linear regression on candidate right/left lane line
segment endpoints, to create right/left lane line equations. 


