# Crop_mapping # Multi-Temporal SAR-Based Crop-Type Mapping over Karnal, Haryana

**Author:** Urmika Mitra  
**Programme:** M.Sc. Geoinformatics, Bharati Vidyapeeth Institute of Environment Education and Research (BVIEER), Pune  

## Project Overview
This project presents an independent crop-mapping investigation utilizing multi-temporal Synthetic Aperture Radar (SAR) imagery over Karnal District, Haryana, for the Kharif season[cite: 5]. The primary objective is to classify major agricultural classes—specifically **Paddy Rice**, **Upland Crops**, and **Fallow Land**—using Sentinel-1 SAR backscatter time-series data and a Random Forest supervised classifier implemented in Google Earth Engine (GEE)[cite: 1, 5].

## Study Area
* **Location:** Karnal District, Haryana (Indo-Gangetic Plain)[cite: 1]
* **Season Monitored:** Kharif Season[cite: 1, 5]
* **Target Classes:** Paddy Rice, Upland Crops, Fallow Land[cite: 1, 5]

## Methodology & Workflow
1. **SAR Preprocessing:** Filtering Sentinel-1 GRD imagery, calculating VV/VH polarization ratios, and generating temporal statistics[cite: 1, 5].
2. **Supervised Classification:** Training and executing a Random Forest classifier based on robust reference training samples[cite: 1, 5].
3. **Accuracy Assessment:** Evaluating map performance using an independent confusion matrix, overall accuracy, producer's/user's accuracy, and F1-scores[cite: 5].
4. **Web Publication:** Communicating results through an interactive, publicly accessible GitHub Pages webpage[cite: 5].

## Access Live Webpage
You can view the interactive map and project dashboard via GitHub Pages:  
[https://urmikamitra28-dev.github.io/Crop_mapping/] 
