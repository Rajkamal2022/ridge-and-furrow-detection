# Ridge and Furrow Detection using YOLOv8

Automated detection and segmentation of medieval ridge and furrow earthworks 
from LiDAR-derived visualisations using YOLOv8n.

## MSc Data Science Dissertation
Durham University, 2026

## Structure

  - `bounding_box/` - YOLOv8n bounding box detection
  - `segmentation_original/` - YOLOv8n-seg with original polygons
  - `segmentation_refined/` - YOLOv8n-seg with refined polygons
  - `segmentation_checkerboard/` - YOLOv8n-seg with refined polygons and checkerboard splitting

Each folder contains:
- Training curves, F1 curves, confusion matrices
- Validation predictions and labels
- Training configuration (args.yaml) and metrics (results.csv)
- Model weights (best.pt, last.pt)

## Best Model
Refined segmentation with checkerboard splitting:
- Box mAP50: 0.569
- Mask mAP50: 0.594
- F1 Score: 0.60
- Northumberland transferability: 82% site-level detection rate
