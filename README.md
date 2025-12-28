# Assignment 2: 3D Vision & Camera Calibration

Advanced computer vision assignment focusing on 3D reconstruction, camera calibration, and point cloud processing.

## Overview

This assignment covers fundamental concepts in 3D computer vision:
- Camera intrinsic and extrinsic parameter estimation
- Homography transformation for image alignment
- 3D point cloud registration using Iterative Closest Point (ICP)
- 3D-2D projection and camera geometry

## Contents

### Main Scripts

- **`camera-calibration.ipynb` / `camera-calibration.py`** - Problem 3: Camera Calibration & Projection
  - Estimates intrinsic camera parameters (focal length, principal point, skew)
  - Calculates extrinsic parameters (rotation and translation matrices)
  - Reprojects 3D points to 2D image space

- **`homography-alignment.ipynb` / `homography-alignment.py`** - Problem 4: Homography & Image Alignment
  - Computes homography matrices between image pairs
  - Performs perspective transformation and image warping
  - Validates correspondence matches

- **`icp-point-cloud.ipynb` / `icp-point-cloud.py`** - Problem 5: ICP Algorithm & Point Cloud Registration
  - Implements Iterative Closest Point (ICP) algorithm
  - Registers 3D point clouds through rotation and translation
  - Computes transformation matrices for alignment

### Data Files

- **`camera-parameters.json`** - Camera intrinsic and extrinsic parameters
  - Focal length, principal point, skew coefficient
  - Rotation matrices and translation vectors for multiple views

- **`homography-matrices.csv`** - Homography transformation matrices
  - Contains H matrices for image pair alignments

- **`icp-transformations.csv`** - ICP registration results
  - Transformation parameters from point cloud registration

- **`assignment-report.pdf`** - Detailed assignment report with results and analysis

## Key Concepts

### Camera Calibration
Determining the internal camera parameters that relate 3D world coordinates to 2D image coordinates.

### Homography
A 3×3 transformation matrix that maps pixel coordinates between two images taken from different viewpoints of a planar scene.

### Point Cloud Registration (ICP)
Algorithm to find the optimal transformation between two point clouds by iteratively minimizing the distance between corresponding points.

## Technical Stack
- Python 3
- NumPy for numerical computation
- OpenCV for image processing
- PyTorch (potential deep learning components)

## Results
All outputs are saved in CSV and JSON formats for easy integration with other systems.
