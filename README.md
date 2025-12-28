# Image Stitching

This repository contains a Python implementation of an **image stitching pipeline** using OpenCV. The pipeline can generate panoramas from 2 or more overlapping images using feature detection, feature matching, homography estimation, warping, blending, and color correction.

## Features / Experiments

In this project, we implemented and compared different image stitching approaches:

- Feature detectors: **ORB** and **SIFT**
- Feature matchers: **FLANN** and **Brute Force**
- Homography estimation: **RANSAC**
- Warping, blending, and histogram matching for color consistency
- Progressive stitching for multiple images (2+)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/nguyen1oc/Image-Stitching.git
cd Image-Stitching
```
2. Change the input of images:
```bash
img0 = cv2.imread('/content/drive/MyDrive/*.jpg')
img1 = cv2.imread('/content/drive/MyDrive/*.jpg')
```

## Data

You can test the pipeline using your own images or sample images from the OpenCV test repository: [stitching test data](https://github.com/opencv/opencv_extra/tree/4.x/testdata/stitching).

## Google Colab

You can run the experiments directly in Google Colab using this notebook:  
[Open in Colab](https://colab.research.google.com/drive/1WOOvzP7u7qvt-4NhqanoaNtRMK-MKt8r#scrollTo=_LKbVyy0hrQ5)

## Example

### Example 1: Simple test images
<p float="left">
  <img src="test/a1.png" width="150" />
  <img src="test/a2.png" width="150" />
  <img src="test/a3.png" width="150" />
</p>
Output panorama:  
<img src="test/resulta.png" width="450" />

### Example 2: Boat images
<p float="left">
  <img src="test/boat1.jpg" width="120" />
  <img src="test/boat2.jpg" width="120" />
  <img src="test/boat3.jpg" width="120" />
  <img src="test/boat4.jpg" width="120" />
</p>
Output panorama:  
<img src="test/resultboat.png" width="480" />

