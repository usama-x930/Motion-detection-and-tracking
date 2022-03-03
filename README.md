# Motion detection and tracking
## Introduction
Motion detection is the process of detecting a change in the position of an object relative to its surroundings or a change in the surroundings relative to an object. The background of our video stream is largely static and unchanging over consecutive frames of a video.  If we can model the background, we monitor it for substantial changes.
## Methodology
<p align="center">
  <img src="Figs/methodology.jpg" width="800" title="hover text">
  
</p>

### Step 1:
Background image is a baseline image. This image is used as a reference for detecting object. Frame difference is calculated between the reference image and the image having an object.

  <img src="Figs/st1.jpg" width="100" title="hover text">
  
### Step 2:

The next step is conversion to grayscale and gaussian smoothing. It removes the noise from the image since noise can affect the edge detection results. The gaussian kernel is calculated using the formula: 
<img src="Figs/gauss.jpg" width="100" title="hover text">

Gaussian filter is convolved with the image to remove the noise and smoothened the image.
<img src="Figs/conv.jpg" title="hover text">

### Step 3:
[![Watch the video]("dilate.avi")]("dilate.avi")
