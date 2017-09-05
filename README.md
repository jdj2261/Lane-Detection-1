# **Finding Lane Lines on the Road** 



**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


## grayscale --> Gaussian smooth --> Canny edge detection --> ROI --> Hough transformation --> pic overlay

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...

Scenario 1
kernel_size = 5
low_threshold = 120
high_threshold = 200
min_line_len = 3
max_line_gap = 100

Scenario 2
kernel_size = 5
low_threshold = 80
high_threshold = 200
min_line_len = 3
max_line_gap = 100

Scenario 3
kernel_size = 7
low_threshold = 100
high_threshold = 200
min_line_len = 3
max_line_gap = 100

parameters optimization play a positive role in processing the image. But there are still some short lines detected of shadows, which requires a slope filter.
