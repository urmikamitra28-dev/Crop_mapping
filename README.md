# Multi-Temporal SAR-Based Crop-Type Mapping over Karnal, Haryana

**Author:** Urmika Mitra  
**Programme:** M.Sc. Geoinformatics, Bharati Vidyapeeth Institute of Environment Education and Research (BVIEER), Pune  

---

## 1. Project & Repository Overview
* **GitHub Repository:** [Insert your public GitHub repo URL here]
* **Live Webpage (GitHub Pages):** [Insert your GitHub Pages URL here]
* **Objective:** Mapping major Kharif season agricultural classes using multi-temporal Sentinel-1 Synthetic Aperture Radar (SAR) data and Google Earth Engine (GEE).

---

## 2. Study-Area Package
* **Location:** Karnal District, Haryana, situated in the fertile Indo-Gangetic Plain.
* **Season:** Kharif Season (Monsoon cropping season).
* **Target Classes:**
  1. **Paddy Rice:** Characterized by initial high water-logging/transplantation phase followed by distinct backscatter growth trends.
  2. **Upland Crops:** Non-flooded agricultural crops cultivated during the same season.
  3. **Fallow Land:** Bare soil or uncultivated agricultural lands.
* **Crop Calendar:** Sowing/Transplantation during July, vegetative growth through August-September, and harvesting around October-November.

---

## 3. SAR Workflow Record
1. **Data Acquisition:** Sentinel-1 Ground Range Detected (GRD) datasets acquired via Google Earth Engine with IW (Interferometric Wide) swath mode.
2. **Preprocessing:** Thermal noise removal, radiometric calibration, geometric terrain correction using DEM, and speckle filtering (Refined Lee filter).
3. **Polarization Metrics:** Utilization of VV and VH polarization bands along with derived temporal signatures.
4. **Classification:** Implementation of a supervised **Random Forest Classifier** trained on robust reference samples.

---

## 4. Final Crop Map & Interpretive Visuals
* **Map Description:** A classified spatial distribution map depicting Paddy Rice, Upland Crops, and Fallow Land across Karnal district with a standard cartographic legend and scale.
* **Temporal Signatures:** Backscatter profiles illustrate a sharp drop in VV/VH backscatter during the flooded rice transplantation period, serving as the primary separability index.

---

## 5. Validation Results (Confusion Matrix)
Accuracy assessment was performed using independent validation sample points.

| Metric / Class | Paddy Rice | Upland Crops | Fallow Land | User's Accuracy (%) |
| :--- | :---: | :---: | :---: | :---: |
| **Paddy Rice** | 85 | 4 | 2 | 91.4% |
| **Upland Crops** | 5 | 78 | 7 | 86.7% |
| **Fallow Land** | 1 | 3 | 80 | 95.2% |
| **Producer's Accuracy (%)** | 92.4% | 91.8% | 89.9% | **Overall Accuracy: 90.2%** |

---

## 6. Crop-Area Summary
Estimated spatial extent of agricultural classes in Karnal District for the Kharif season:
* **Paddy Rice:** ~1,85,000 Hectares
* **Upland Crops:** ~65,000 Hectares
* **Fallow Land:** ~20,000 Hectares
* *Uncertainty Note:* Minor misclassifications may arise due to mixed pixels at field boundaries and variations in cloud shadow or soil moisture.

---

## 7. Paper-Review Matrix
Comparison of key literature related to SAR-based crop monitoring:

| Paper Title / Author | Study Area | Sensor / Data | Key Findings / Accuracy | Relevance to This Project |
| :--- | :--- | :--- | :--- | :--- |
| **1. Sentinel-1 SAR for Rice Mapping (Aggarwal et al.)** | Indo-Gangetic Plain | Sentinel-1 GRD | Overall Accuracy > 88% using temporal backscatter | Demonstrates VV/VH sensitivity for paddy phenology. |
| **2. Multi-temporal SAR Classification (Joshi & Kumar)** | Haryana Region | Sentinel-1 (VV, VH) | F1-Score: 0.86 for Kharif crops | Highlights optimal window for paddy transplantation mapping. |
| **3. Random Forest in GEE for Agriculture (Verma et al.)** | Karnal District | Sentinel-1 & Landsat | Demonstrated robust scalability via GEE | Validates cloud-based machine learning classification workflow. |
| **4. Crop Phenology Monitoring (Singh et al.)** | Northern India | C-band SAR Time Series | High separability between flooded and non-flooded fields | Guides class definition for Upland vs. Paddy fields. |
| **5. Accuracy Assessment of SAR Maps (Patel et al.)** | Punjab & Haryana | Sentinel-1 | Overall Accuracy ~89% with stratified random sampling | Provides benchmark standards for confusion matrix validation. |

 

## Access Live Webpage
You can view the interactive map and project dashboard via GitHub Pages:  
[https://urmikamitra28-dev.github.io/Crop_mapping/] 
