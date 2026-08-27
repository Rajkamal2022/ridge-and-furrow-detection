# ridge-and-furrow-detection

## Description
Automated detection and segmentation of medieval ridge and furrow features from LiDAR-derived visualisations using YOLOv8.

 ## Training Dataset 
 - Midland region 
## Pipeline
1. LiDAR preprocessing (RVT visualisations)
2. Percentile Normalisation
3. RGB composite creation
4. Tiling and JPEG conversion
5. Automated label generations
6. YOLO models training and evaluations

## Models
- YOLOv8n Bounding Box Detection
- YOLOv8n-seg Segmentation (Original Polygons)
- YOLOv8n-seg Segmentation (Refined Polygons)
- YOLOv8n-seg Segmentation (Refined + Checkerboard Split)

## Test Dataset ( Northumberland)
##  Manual Results using YOLOv8n-seg with checkerboard splitting model
- Evaluated on 1,155 tiles (104 labelled, 141 instances)
- Box mAP@0.5: 0.178 | Mask mAP@0.5: 0.174
- Low automated metrics because only 104 of 1,155 tiles had ground truth labels. Correct detections on the remaining 1,051 unlabelled tiles were counted as false positives, artificially lowering the scores.
- Manual validation confirmed 82% site-level detection rate (127/154 known sites)
- 428 medieval RNF confirmed, 444 post-medieval and 202 modern agriculture false positives
- Expert review (Pett, D.) confirmed identifications were broadly correct
