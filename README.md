## **CIS 731 Data Science and Analytics Term Project**

## **Project Overview**
This project focuses on building a scalable and efficient data pipeline to process Sentinel-2 satellite imagery data using Google Earth Engine (GEE). The pipeline transforms raw satellite imagery into actionable datasets suitable for training advanced machine learning models to generate realistic 3D terrain for VR and gaming applications.

---

## **Data Preparation Steps**

### 1. **Source Data**
- **Sentinel-2 Surface Reflectance Dataset**: Processed satellite data sourced vis Google Earth Engine (GEE).
 - Dataset Reference: [Sentinel-2 SR Harmonized](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR_HARMONIZED)

### 2. **Pipeline Steps**
1. **Data Retrieval**:
    - The Sentinel-2 dataset is retrieved and filtered for a specific time range and region of interest using GEE.
2. **Preprocessing**:
    - Cloud masking is applied to remove unwanted artifacts.
    - Bands corresponding to visual (RGB) and near-infrared (NIR) wavelengths are selected.
3. **Composite Generation**:
    - Image composites are created to merge high-quality imagery over the selected region.
4. **Export**:
    - The resulting composite data is exported for local processing and analysis.
5. **Visualization**:
    - 

---

## **Usage**

### 1. **Clone the repository**
```bash
 git clone https://github.com/sagewoodard/CIS731_DataScience_TermProject.git
 cd CIS731_DataScience_TermProject
```

### 2. **Set up the required Python environment**
```bash
 pip install -r requirements.txt
```

### 3. **Run the data pipeline**
```bash
 python gee_pipeline.py
```

---

## **Dependencies**
Ensure the following libraries are installed:
- Python 3.x
- Google Earth Engine API (`earthengine-api')
- Folium
- Matplotlib
- Rasterio
- NumPy
- pandas
- TensorFLow
- SciPy
- scikit-learn
- protobuf

Install all dependencies using the provided `requirements.txt` file.

---

## **Contributing**
Contributions are welcome! If you wish to contribute or improve this pipeline, please submit a pull request.

---

## **License**
This project is licensed under the MIT license.

---

## **References**
- Sentinel-2 SR Dataset: [Google Earth Engine Catalog](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR_HARMONIZED)
- Google Earth Engine: [GEE Documentation](https://developers.google.com/earth-engine)
- Folium: [Folium Documentation](https://python-visualization.github.io/folium/)
- Rasterio: [Rasterio Documentation](https://rasterio.readthedocs.io/en/latest)
