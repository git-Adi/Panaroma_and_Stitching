# Image Processing with OpenCV

This repository contains Python code for advanced image processing tasks including feature detection, keypoint matching, and image stitching to generate panoramas. The implementation leverages OpenCV libraries to accomplish these tasks.

## Project Structure

- `keypoint_detection.py`: Script for detecting keypoints and computing descriptors in images.
- `feature_matching.py`: Script for matching features between two images using Brute-Force and FLANN based matchers.
- `homography_computation.py`: Script for computing the homography matrix between matched keypoints.
- `image_warping.py`: Script for perspective warping of images based on the computed homography.
- `image_stitching.py`: Script for stitching images to create a panorama, with both blended and unblended options.

## Features

1. **Keypoint Detection and Descriptor Computation**
   - Conversion of images to grayscale for processing.
   - Detection of keypoints and computation of descriptors using OpenCV functions.

2. **Feature Matching**
   - Initialization and use of both Brute-Force and FLANN based matchers.
   - Application of the ratio test to filter out reliable matches.

3. **Homography Computation**
   - Extraction and reshaping of coordinates from matched keypoints.
   - Calculation of left and right homography matrices for image alignment.

4. **Image Warping**
   - Application of perspective warping to align images based on the computed homography.

5. **Image Stitching**
   - Stitching of images into a single panorama.
   - Both blending and non-blending stitching methods are implemented.

## Usage

To run the image processing scripts, ensure you have Python and OpenCV installed. Each script can be executed individually to perform the corresponding image processing task. Example:

```bash
python keypoint_detection.py
