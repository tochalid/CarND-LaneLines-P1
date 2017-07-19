# **Finding Lane Lines on the Road** 

## Writeup Chalid Mannaa, Term1 - 07/2017

### Ubuntu 16.04 LTS, Python 3, Anaconda, IPython/Notebook

---

**Finding Lane Lines on the Road**

The goals of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report (pls see following)


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Pipeline Description. The draw_lines() function contains trigonometric logic, averaging and extrapoltion in oder to draw a single line for left and right lane edges.

My pipeline consisted of 6 steps and returns an image with detected lane lines.
1. Grayscale the image 
2. Gaussion Blur for better accuracy 
3. Canny edge detection 
4. Polynom Mask to find the region of interest 
5. Hough algorithm to detect lines  

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
