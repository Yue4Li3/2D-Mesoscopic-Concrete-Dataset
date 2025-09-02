# 2D Mesoscopic Concrete Dataset

## Overview
This dataset contains 150 mesoscopic 2D concrete models for research on concrete mesostructure, durability, and data-driven modeling.

Each model consists of:
- A `.jpg` image showing the mesoscopic cross-section
- A `.csv` file containing pixel-level data (aggregate vs mortar)

## File Naming Convention
Files are named as:

    AGin_<size>_<agg%>_<id>.jpg
    AGin_<size>_<agg%>_<id>.csv

where:
- <size> = specimen size in mm (100, 150, 200)
- <agg%> = aggregate volume fraction (20, 30, 40, 50, 60)
- <id> = model index number

Example:
- `AGin_200_30_2.jpg` → 2nd model, size = 200 mm × 200 mm, aggregate = 30%  
- `AGin_200_30_2.csv` → pixel-level data for the same model  

## Dataset Content
- Sizes: 100 mm × 100 mm, 150 mm × 150 mm, 200 mm × 200 mm
- Aggregate fractions: 20%, 30%, 40%, 50%, 60%
- Total models: 150

## Usage
- Use `.jpg` for visualization, segmentation, and image-based ML training.
- Use `.csv` for numerical modeling or direct pixel data processing.

## Citation
If you use this dataset, please cite:

[Your Name]. "2D Mesoscopic Concrete Dataset." GitHub, 2025. DOI: (to be added)

## License
- Open for academic and non-commercial research.
- Commercial use requires written permission from the author.
- © 2025 [Your Name]. All rights reserved.

## Contact
Maintainer: Yue Li
Affiliation: Tongji University 
Email: yue.li@tuwien.ac.at