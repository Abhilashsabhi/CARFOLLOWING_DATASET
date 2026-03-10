# Multimodal Car-Following Dataset for Benchmarking Longitudinal Driving Models

## Overview

This repository provides a multimodal car-following dataset collected using synchronized camera, LiDAR, and GNSS sensors across multiple cities in India. The dataset captures naturalistic longitudinal vehicle interactions under heterogeneous traffic conditions.

From the multimodal recordings, we extract standardized car-following trajectories consisting of:

- Relative distance
- Relative velocity
- Ego vehicle speed
- Lead vehicle speed

These features are used for benchmarking classical, learning-based, and reinforcement learning car-following models.

## Dataset Statistics

- Total driving distance: ~150 km
- Cities: Salem, Bengaluru, Dindigul, Kurnool
- Total recording duration: ~3 hours
- Scene duration: 15–60 seconds
- Sampling rate: 10 Hz
- Extracted features: distance, relative speed, ego speed, lead speed

## Sensor Setup

Data were collected using the following sensors:

- Monocular camera
- 3D LiDAR
- GNSS receiver

All sensors were time-synchronized and recorded using ROS2 bag files.

dataset/
│
├── raw_data/
│   ├── ros2_bags/
│   └── sensor_logs/
│
├── processed_data/
│   ├── trajectories/
│   │   ├── scene_001.csv
│   │   ├── scene_002.csv
│   │   └── ...
│
## Dataset Availability

A sample subset of the dataset is included in this repository for demonstration and reproducibility purposes.

The full dataset will be made publicly available upon acceptance of the associated paper at IEEE ITSC.
