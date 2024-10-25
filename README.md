# Automated-Wetland-Classification-Using-CNN
# Automated Wetland Classification and Monitoring Using Convolutional Neural Networks

This project focuses on automated classification and monitoring of wetlands in Kajiado County, Kenya, utilizing Convolutional Neural Networks (CNNs) with Landsat 7 imagery. The objective is to accurately map wetlands, monitor changes over time, and develop spatially generalizable models for broader ecological applications.

## Project Overview

Wetlands are ecologically critical areas that serve various environmental functions but are at risk due to urbanization and climate change. Accurate, high-resolution wetland maps are essential for conservation efforts and informed policy decisions. This project applies CNNs, particularly VGG-16, to classify and monitor wetlands, generating high-precision maps with an accuracy of up to 94%.

### Objectives
1. **Main Objective**: Develop an automated system for wetland classification and monitoring using CNNs on Landsat 7 imagery.
2. **Specific Objectives**:
   - Characterize climatic, biophysical, and anthropogenic factors influencing wetlands.
   - Refine CNN architecture and parameters for improved wetland classification.
   - Validate model accuracy using ground truth data.

## Methodology

### Data Collection
Data was sourced from multiple platforms, including Google Earth Engine and USGS. The datasets used include:
- **Landsat 7 Imagery**: Provides multispectral data essential for wetland classification.
- **Digital Elevation Model (DEM)**: Used for topographic corrections.
- **MODIS and Rainfall Data**: Supports understanding of environmental impacts on wetlands.

### Data Preprocessing
- **Index Calculations**: Key indices such as NDVI, NDWI, MNDWI, SAWI, and SAVI were computed to capture soil moisture, vegetation health, and water extent.
- **Classification**: A Random Forest classifier was initially used to create land-use maps.
- **Accuracy Assessment**: Ground truthing was conducted to validate classification results.

### Model Architecture
The VGG-16 CNN architecture was selected for its effectiveness in feature extraction and classification accuracy. Training was performed using labeled datasets from various land cover types within Kajiado County.

### Software
- **Google Earth Engine**: Used for data preprocessing and index calculation.
- **Google Colab**: Used for training, testing, and evaluating the CNN model.
- **ArcMap**: Used for mapping and visualization.

## Results

The CNN model achieved:
- **Accuracy**: 94%
- **Precision**: 96.5%
- **Area Under Curve (AUC)**: 95.2%
- Model validation showed robustness across varied geographic areas, but retraining may be necessary for new geographies.

### Outputs
The project outputs include high-resolution maps of wetlands in Kajiado County. These maps can assist policymakers, conservationists, and researchers in monitoring wetland dynamics and planning conservation efforts.

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/richardk100/automated-wetland-classification-using-CNN.git
