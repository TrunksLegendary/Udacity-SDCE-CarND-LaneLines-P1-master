# **Finding Lane Lines on the Road**

## 1. Describtion of my pipeline.

The Pipeline used 6 steps to obtain a image with detected lanes:

>**1st**  

After reading the images, convert the images to  a grayscale  

>**2nd**  

The Images are further processed with the gaussian_blur function to smooth the edges  

>**3rd**  

The edges are then obtained with the canny function.

>**4th** 

The region that interests function is used to mask the area ofhte image that may contain lines.
  
>**5th** 

Using the Hough transform, we find the lines. 

>**6th**  

The detected lane lines are the ndrawn on the original images.
 

The pipeline works fine for the images and two videos with simpler conditions except that I have 2 lines for each side. 

For the challenge.mp4 video, there was significant difficultyto detect stable reliable lines due to the road curvature, condition, or unclear or missing road lines. I tried to overcome this by tweaking the varibles of the funtions, but was unsucessful.


>### 2. Shortcomings with your current pipeline

My pipeline can't divide the lines correctly on the curved lane.  

The Optional Challenge I could not clean it up anymore that this.  


>### 3. Suggest possible improvements to your pipeline

A possible improvement to compensate for adverse road conditions would be to use additional cameras from differnt positions and compare the detected images. Perhaps images from differnt angles product accurate lane detection based on certain types of road conditions. 
