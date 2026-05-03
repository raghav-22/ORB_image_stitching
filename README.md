# ORB feature based image stitching for images
# Image Stitching
Image stitching is a computer vision technique used to combine multiple overlapping images into a single seamless image, often called a panorama. It is widely used in photography, robotics, and medical imaging.

The process typically involves detecting key features in each image, matching those features across images, estimating a transformation (homography) to align them, and then blending the images to remove visible seams.

# Common steps:
Feature detection (e.g., SIFT, ORB)
Feature matching between images
Homography estimation for alignment
Image warping and stitching
Blending for smooth transitions

Libraries like OpenCV provide built-in support to implement image stitching efficiently.

In simple terms, image stitching helps create a wider or more detailed view of a scene by merging multiple images into one.

This is a python script for doing the same. Here I used ORB features to identify each feature in an image and using that the images are stitched together. ORB is a pre-built function available on openCV.
The data for the program are cropped regions of images, stored in a folder. The path of the folder is given as input. Program iterate through the folder and joins image based on common feature.

# Input
img1.jpg img2.jpg img3 img4

# Output
stiched.jpg

# How to run the code
1. Clone the repository in your machine
2. Install requirements.txt using pip
3. Add your data on same folder
4. Run stitch-image.py
