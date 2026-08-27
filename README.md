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
