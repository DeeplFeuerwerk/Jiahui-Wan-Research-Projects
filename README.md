# Jiahui-Wan-Research-Projects
My personal research projects on sensor fusion for robotics and autonomous driving applications.

This repository contains two of my research projects related to multi-sensor fusion for autonomous vehicles, specifically focusing on the integration of LiDAR and fisheye cameras.

Project 1: Extrinsic Calibration of LiDAR and Fisheye Camera Based on Deep Learning and Geometric Optimization
Summary:

This project addresses the challenge of extrinsic calibration between a LiDAR and a fisheye camera, a topic that has received limited research attention compared to LiDAR-pinhole camera systems. The proposed method uses a deep learning model to predict the extrinsic transformation matrix and then refines the result with a geometric optimization strategy.


Key Contributions:


Deep Learning Model: A deep learning-based method for extrinsic calibration of LiDAR and fisheye cameras.


Geometric Optimization: The introduction of a geometric optimization post-processing strategy to enhance calibration accuracy.


Performance: The deep learning model reduced point cloud alignment error by 91.6%, with the additional geometric post-processing further reducing the error by 52.4%.


Practical Application: The method demonstrates high accuracy, reliability, and robustness for real-world applications in autonomous driving, intelligent surveillance, and robotic perception.

Technical Details:


Training Data: The method uses 18,335 image-point cloud pairs for training. A unique data generation method is used to create a large number of training samples by applying new extrinsic transformations to initial data pairs.



Network Architecture: A dual-branch deep neural network is used to process fisheye camera images and point cloud data represented as Geometric Mapping Images (GMI). A spatial attention module is incorporated to improve feature extraction from sparse point clouds.



Loss Function: The loss function is based on point cloud alignment error, measuring the difference between point clouds transformed by predicted and ground-truth extrinsic parameters.

Project 2: Fisheye Camera and LiDAR Fusion for Autonomous Following Vehicles
Summary:

This paper presents a method for fusing LiDAR and fisheye camera data to enable accurate, real-time 3D localization of a target person for autonomous following vehicles. The method is applied in a real-world scenario, such as an autonomous cleaning vehicle following a person.




Key Contributions:


Fusion Method: A method to fuse fisheye camera and LiDAR data for accurate spatial localization of a target person.


Target Localization Algorithm: A robust target localization algorithm that performs well even in complex environments with foreground occlusions or background interference.


Wider Field of View: Demonstrates the advantage of using a fisheye camera, which provides a significantly wider field of view compared to a pinhole camera, enhancing its applicability in dynamic and cluttered environments.

Technical Details:


Calibration: The method employs a joint calibration technique to spatially align the LiDAR and fisheye camera.


Localization Process: It uses YOLO series models for object detection in fisheye images and a filtering method that shrinks bounding box edges to mitigate errors from occlusion and background interference. The point cloud is projected onto an adjusted region of interest (ROI') and then processed using an annular layer division and merging method to precisely locate the target.




Performance: The algorithm maintains a relative squared error within 10% across all tested distances and angles.
