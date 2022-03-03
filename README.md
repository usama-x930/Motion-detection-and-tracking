# Motion detection and tracking
## Introduction
Motion detection is the process of detecting a change in the position of an object relative to its surroundings or a change in the surroundings relative to an object. The background of our video stream is largely static and unchanging over consecutive frames of a video.  If we can model the background, we monitor it for substantial changes.
## Methodology
<p align="center">
  <img src="Figs/methodology.jpg" width="800" title="hover text">
  
</p>

### Step 1:
Background image is a baseline image. This image is used as a reference for detecting object. Frame difference is calculated between the reference image and the image having an object.

  <img src="Figs/st1.jpg" title="hover text">

