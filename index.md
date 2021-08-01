# Analyzing Social Distancing Based on Sensory Inputs
<h2>Weekly Updates</h2>

### [Week 1](https://docs.google.com/presentation/d/10ShJHYYFKcQgGqVLqGvah1pI3n8cUgC-pHTAbpTq5bU/edit?usp=sharing)

* Created Orbit and Safegraph accounts
* Intro to command line and SSH
* Learning about [project background](https://dl.acm.org/doi/pdf/10.1145/3417991)

### [Week 2](https://docs.google.com/presentation/d/1BQxArk1C2sRHngOjus9_ZxEkWO5-X4jzyPZdKtqA9M0/edit#slide=id.gdf5cfffc92_2_0)

* Set up project page
* Plan: detect single person using YOLO, use them as anchor to create patches, count the people in each patch, and account for overlap
* Created Overleaf documentation

### [Week 3](https://docs.google.com/presentation/d/1iC-iT_pJ0wLGpHe-jpq336eBVQtAhqbGP4ktapv_ZIM/edit?usp=sharing) 

* Accessed quad server and data
* Intro to Keras and Jupyter notebook
* YOLO tutorial for object detection

### [Week 4](https://docs.google.com/presentation/d/1Oem8g_Sa2jdCDE677N2vLKdRGkU70E-g_ZYWBtIVHio/edit#slide=id.ge0c48ac287_0_0) 

* Ran YOLO on quad server on small image set
* Set up Pedestron model on server
* Data visualization is live

### [Week 5](https://docs.google.com/presentation/d/1aMaNLTRuP8yg_G7ZaASCPXCzR2NJFCF0wWpVe4Htq1s/edit#slide=id.ge0c48ac287_0_8)

* Abandoned Pedestron, not well-maintained
* Ran full YOLO on ~800 dashcam images
* Got coordinates of people in images
* Created new plan for patch creation

### [Week 6](https://docs.google.com/presentation/d/1L_Y9ebGH6Eh2lV5zaIPwBvrQBcG91oZZQFBg30Iqz7Y/edit?usp=sharing)

* Expanded rectangular patches around the subject
* Accounted for out-of-frame errors when making bounding boxes
* Made a simple function to calculate social distancing from camera-person distance in the 3D perspective
* Brainstormed the idea of projecting a line of the same height as a person within the 3D perspective view

### [Week 7](https://docs.google.com/presentation/d/1mUUeUaShCxW-Fm66W5QrSoKZiaxzdamT2c7Ni0zyQHM/edit?usp=sharing)
* Tested and improved image cropping script on a 100-image set
* Increased resolution of cropped out image patches and tested HD patches through YOLO for people detection -- images pre-processed with ESPCN works best
* Formulated a distance detector using weighted euclidean approximation that can estimate the distance between people and how many people each person is around with the help of YOLO

### [Week 8](https://docs.google.com/presentation/d/1sxaUvzb8Z18OYT1ZFd_HudDcpWQN6w8dhFUv-rN7oBI/edit?usp=sharing)
* Created and populated month-wise image directories for Manhattan
* Ran the images through YOLO to separate people images and create patches and ran the patches through super resolution 
* Compiled data of images, timestamps, locations, and quantified social distancing
* Created different time bins and validated our results

### [Week 9](https://docs.google.com/presentation/d/18DIcUvgcpOQKyfX-tceZOX1Pz7mrIY2b_BipZatWpKI/edit?usp=sharing)
* Processed images for whole month of July for all boroughs
* Made a temporal graph for image count of Manhattan per month
* Aggregated Manhattan data per day and generated a bubbleplot that accounts for social distancing
* Generated a bubble plot for social distancing as it depended on time of day
* Obtained a POI dataset and scraped its Google category

  
[_______](https://github.com/mshankar58/winlab-social-distancing-2021/edit/main/index.md)

