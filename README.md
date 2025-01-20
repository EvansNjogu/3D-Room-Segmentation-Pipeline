# 🏠 3D Room Segmentation Pipeline using Point Clouds and PointNet++


[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)
[![PointNet](https://img.shields.io/badge/Model-PointNet-orange)](https://github.com/yanx27/Pointnet_Pointnet2_pytorch)
[![Dataset](https://img.shields.io/badge/Dataset-S3DIS-2BAF2B)](http://buildingparser.stanford.edu/dataset.html)

---

A comprehensive pipeline for 3D room segmentation using point cloud data, integrating PointNet++, plane fitting and clustering techniques. This project covers the full process from data acquisition and preprocessing to segmentation and visualization, applied to datasets like **[Stanford 2D-3D Indoor Spaces (S3DIS)](http://buildingparser.stanford.edu/dataset.html)** and **[KITTI](https://www.cvlibs.net/datasets/kitti/)**.

---

## Project Overview  
The goal of this project is to build an accurate and efficient segmentation pipeline capable of processing large 3D indoor environments. By leveraging **PointNet++** for semantic segmentation and integrating traditional point cloud methods, the pipeline achieves high performance in segmenting and visualizing complex 3D spaces.

### Key Features:
- Data Acquisition & Preprocessing
   - Supports Stanford 2D-3D Indoor Scenes (S3DIS) and KITTI datasets.  
   - Downsampling, noise filtering and outlier removal using Open3D.  
   - Voxel downsampling and statistical outlier removal.  

- 3D Segmentation & Clustering 
   - Plane segmentation (RANSAC) to detect ground and walls.  
   - Region growing and DBSCAN for clustering and object detection.  
   - Semantic segmentation using PointNet++.  

- Visualization
   - Color-coded segmentation outputs.  
   - Real-time 3D point cloud visualization with Open3D.  
   - Confusion matrices and classification reports to evaluate performance. 


---

## Project Structure  

```
3D-Room-Segmentation-Pipeline/
 ├── 📁 assets 
 ├── 📁 docs
 └── 📂 notebooks 
```
---

## Results
Here are some outputs from the segmentation pipeline, showcasing various stages such as preprocessing, segmentation and PointNet predictions.

### Original Point Cloud
<img src="assets/original_pointcloud.png" alt="Original Point Cloud" width="400">

### Preprocessed Point Clouds

#### Radius Outlier Removal
<img src="assets/radius_outlier.png" alt="Radius Outlier Removal" width="400">

#### 3D Harris Corner Detection
<img src="assets/corner_detect.png" alt="3D Harris Corner Detection" width="400">

#### Ground Plane Segmentation
<img src="assets/ground_plane.png" alt="Ground Plane Segmentation" width="400">

### Semantic Segmentation for this Pipeline
<img src="assets/semantic_segmentation.png" alt="Semantic Segmentation" width="400">

### PointNet Semantic Segmentation
<img src="assets/pointnet.png" alt="PointNet Segmentation" width="400">

### Full pipeline run on Kitti
<img src="assets/kitti.png" alt="Kitti Test" width="400">

---

## Contact

For any questions or collaboration opportunities, feel free to reach out at [hey@njoguevans.me](mailto:hey@njoguevans.me).