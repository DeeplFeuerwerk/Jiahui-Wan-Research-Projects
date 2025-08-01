# LiDAR-Fisheye Camera Integration

This repository contains the implementation of two research papers focusing on LiDAR and fisheye camera integration for autonomous driving applications.

## Paper 1: Fisheye Camera and LiDAR Fusion for Autonomous Following Vehicles

### Overview
This work tackles the challenge of sensor fusion between LiDAR and fisheye cameras specifically for autonomous vehicle following applications. The research addresses a significant gap in current literature, as most existing work focuses on LiDAR-pinhole camera integration.

### Key Contributions
- **Joint Calibration Framework**: Develops a calibration technique to ensure spatial consistency between LiDAR and fisheye sensors
- **Theoretical Target Localization**: Creates a mathematically grounded algorithm for precise target detection and tracking
- **Robust Performance**: Demonstrates consistent accuracy even under challenging conditions like occlusions and background clutter
- **Enhanced Field of View**: Leverages fisheye cameras' superior coverage compared to traditional pinhole cameras

### Performance Highlights
- Achieves sub-10% relative squared error across varying distances and viewing angles
- Maintains high precision in complex real-world scenarios
- Provides superior environmental coverage for dynamic driving conditions

## Paper 2: Extrinsic Calibration of LiDAR and Fisheye Camera Based on Deep Learning and Geometric Optimization

### Overview
This research focuses on solving the extrinsic calibration problem between LiDAR sensors and fisheye cameras using advanced machine learning techniques. The work fills a critical gap in sensor calibration research, which has traditionally concentrated on LiDAR-pinhole camera pairs while neglecting the unique challenges of fisheye lenses.

### Key Contributions
- **Hybrid Calibration Approach**: Combines neural network prediction with geometric refinement for optimal accuracy
- **Two-Stage Pipeline**: Initial deep learning estimation followed by geometric optimization post-processing
- **Large-Scale Validation**: Comprehensive testing methodology using extensive real-world data
- **Practical Applications**: Designed for autonomous driving, surveillance, and robotic perception systems

### Technical Innovation
- **Neural Network Prediction**: AI-based initial estimation of transformation matrices
- **Geometric Refinement**: Mathematical optimization to enhance calibration precision
- **Error Reduction Strategy**: Systematic approach to minimize alignment errors through combined methodologies

### Performance Achievements
- Over 90% improvement in point cloud alignment accuracy with deep learning
- Additional 50%+ enhancement through geometric post-processing
- Validated on nearly 20,000 real-world sensor data pairs
- Demonstrates high reliability across diverse practical scenarios

## Installation
- git clone https://github.com/DeeplFeuerwerk/Jiahui-Wan-Research-Projects.git
- cd Jiahui-Wan-Research-Projects
