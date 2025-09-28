# Crown-Root Ratio (CRR) Dental Dataset

## Overview
This dataset contains processed dental X-ray images with segmentation masks for crown and root regions, specifically designed for Crown-Root Ratio analysis in dentistry.

## Dataset Statistics
- **Total Images**: 400
- **Successfully Processed**: 400 (100%)
- **Image Resolution**: Mostly 640x640 pixels
- **Format**: JPG images with PNG masks

## Dataset Structure
```
processed_labelme_dataset/
├── images/                 # Original dental X-ray images
├── annotations/           # LabelMe JSON annotation files
├── masks_crown/          # Binary masks for crown regions
├── masks_root/           # Binary masks for root regions
├── masks_combined/       # Combined crown+root masks
├── masks_multiclass/     # Multi-class segmentation masks
├── plots/               # Analysis plots and visualizations
├── splits/              # Train/validation/test splits
│   ├── train.txt        # Training set (280 images, 70%)
│   ├── val.txt          # Validation set (60 images, 15%)
│   └── test.txt         # Test set (60 images, 15%)
├── manifest.csv         # Complete dataset manifest
├── true_crr.csv         # Crown-Root Ratio calculations
└── processed_info.json  # Processing metadata
```

## Crown-Root Ratio Statistics
- **Mean CRR**: 0.738 ± 0.200
- **Range**: 0.270 - 2.125
- **Median**: 0.721
- **25th Percentile**: 0.616
- **75th Percentile**: 0.828

## Data Splits
The dataset is split into three sets with stratified sampling:
- **Training**: 280 images (70%)
- **Validation**: 60 images (15%)
- **Test**: 60 images (15%)

## File Formats
- **Images**: JPG format
- **Masks**: PNG format (binary and multi-class)
- **Annotations**: JSON format (LabelMe compatible)
- **Metadata**: CSV and JSON formats

## Usage
This dataset can be used for:
- Dental image segmentation
- Crown-Root Ratio analysis
- Automated dental diagnosis
- Machine learning model training for dental applications

## Mask Classes
- **0**: Background
- **1**: Crown region
- **2**: Root region

## Citation
If you use this dataset in your research, please cite appropriately.

## License
Please ensure proper attribution when using this dataset.

## Contact
For questions or issues regarding this dataset, please contact the maintainer.
