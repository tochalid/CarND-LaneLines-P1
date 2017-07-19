# **Finding Lane Lines on the Road** 

## Writeup Chalid Mannaa, Term1 - 07/2017

### Ubuntu 16.04 LTS, Python 3, Anaconda, IPython/Notebook

---

**Finding Lane Lines on the Road**

The goals of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report (pls see following)

[//]: # (Image References)

[image0]: /initial_img_whiteCarLaneSwitch.jpg "Initial"
[image10]: /gray_img_whiteCarLaneSwitch.jpg "Grayscale"
[image11]: /blur_img_whiteCarLaneSwitch.jpg "Gauss Blur"
[image12]: /canny_edges_img_whiteCarLaneSwitch.jpg "Canny Edges"
[image13]: /masked_img_whiteCarLaneSwitch.jpg "Polynom Mask"
[image14]: /hough_lines_img_whiteCarLaneSwitch.jpg "Hough Lines"
[image15]: /weight_img_whiteCarLaneSwitch.jpg "Draw Line"

![alt text][image0]
---

### Reflection

### 1. Pipeline Description. The draw_lines() function contains trigonometric logic, averaging and extrapoltion in oder to draw a single line for left and right lane edges.

My pipeline consisted of 5 steps and returns one image with detected lane lines.
1. Grayscale the image 
2. Gaussion Blur for better accuracy 
3. Canny edge detection 
4. Polynom Mask to find the region of interest 
5. Hough algorithm to detect lines  

![alt text]([image10])
![alt text]([image11])
![alt text](image12])
![alt text]([image13])
![alt text]([image14])

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...
TODO

![alt text]([image15])

### 2. Potential shortcomings in this pipeline


One potential shortcoming would be what would happen when the car changes lane(s) and multiple line markings would cross the region of interest?  

Another shortcoming could be ...in general additional scenary eg. curves, hills, weather conditions, other cars, reflection could undermine the detection process in current configuration. 


### 3. Two possible improvements to this pipeline with additional data and CNN technology

A possible improvement would be additional test data to further fine-tune parameters. However, Additional "manual" parameter tuning eg.in Canny & Hough function can be time-consuming, specifically utilizing Notebook IDE.

Another potential improvement could be to utilize convolutional neural networks to learn the detection from bigger and more diverse image data.
