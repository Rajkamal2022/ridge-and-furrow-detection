# ridge-and-furrow-detection

## Description
Automated detection and segmentation of medieval ridge and furrow features from LiDAR-derived visualisations using YOLOv8.

## Pipeline
1. LiDAR preprocessing (RVT visualisations)
2. RGB composite creation
3. Tiling and JPEG conversion
4. Automated label generation
5. YOLO model training and evaluation

## Models
- YOLOv8n Bounding Box Detection
- YOLOv8n-seg Segmentation (Original Polygons)
- YOLOv8n-seg Segmentation (Refined Polygons)
- YOLOv8n-seg Segmentation (Refined + Checkerboard Split)

## Test Dataset
The Northumberland clipped test set (104 labelled tiles out of 1,155) produced lower automated metrics 
due to limited ground truth coverage and due to lack of properly labelled test dataset. 

## Results
- Northumberland validation map showing 428 medieval RNF, 444 post-medieval agriculture, 
  202 modern agriculture, 36 coastal, and 33 other predictions from 1,151 manually classified tiles.
- 82% site-level detection rate (127/154 known sites detected).
