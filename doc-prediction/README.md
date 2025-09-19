# Machine Learning and Satellite Remote Sensing for Predicting Dissolved Organic Carbon (DOC) in Lakes

**Authors:**  
Aisha Malik¹, Marzi Azarderakhsh², Leonid Metlitsky³, Reginald Blake², and Hamid Norouzi²  

¹ Hunter College, CUNY, New York, NY, USA  
² New York City College of Technology, CUNY, Brooklyn, NY, USA  
³ Cornell University, Ithaca, NY, USA  

---

## Abstract

> Understanding long-term changes in dissolved organic carbon (DOC) in lakes is critical for assessing ecological responses to environmental stressors. However, routine, large-scale monitoring of DOC is challenging due to the limited spatial and temporal coverage of in-situ sampling. Remote sensing offers a promising solution, as satellite sensors can detect chromophoric dissolved organic matter (CDOM)—the optically active component of dissolved organic matter—which serves as a widely used proxy for DOC in many freshwater systems. While CDOM provides valuable insight into water quality, traditional remote sensing methods that rely on raw visible-band data and empirical algorithms have shown limited reliability in capturing its spatiotemporal dynamics. This study explores the use of machine learning to enhance DOC prediction within individual lakes using multi-sensor satellite data combined with in-situ measurements from the Adirondack Long-Term Monitoring (ALTM) program, spanning 44 lakes sampled from 1992 to 2021. Surface reflectance data from Landsat 5, 7, 8, and Sentinel-2 are combined with engineered spectral and environmental features to train a range of machine learning models, including decision tree–based algorithms, neural networks, and ensemble approaches. The results show that stacking regressors trained on Landsat data achieved R² values as high as 0.90 within the sampled lakes, yet performance declined substantially on unseen lakes, revealing that the models capture within-lake patterns but struggle to generalize across sites. Despite this limitation, the model outputs effectively capture long-term DOC trends across the Adirondacks region, indicating an increase over time. These findings highlight the potential of machine learning combined with satellite observations as an emerging tool for tracking temporal trends in freshwater carbon dynamics, with applications to monitoring climate change and land-use impacts on lake ecosystems.  

---

## Results

Below is a heatmap showing the performance of different machine learning models trained on the satellite and in-situ data based on current model inputs that result in limited accuracy with new/unseen lakes:

![Model Performance Heatmap](https://github.com/aisha1021/lake-research-nsf/blob/560a5fafe8abcbf76b3e4f0b6cd4cb60abd147cb/doc-prediction/original_model_heatmap.png)

---

## Repository Structure

This repository contains the code, data, and results for experiments on predicting Dissolved Organic Carbon (DOC) in lakes using machine learning and satellite remote sensing.  

```

📂 v1_original_model
├── Jupyter notebooks for each satellite sensor (Landsat 5/7/8, Sentinel-2)
├── Tested machine learning models with visualized results
├── **data/** – includes site information, in-situ measurements, and derived satellite band data
└── ⚠️ Models perform well on **known lakes** but poorly on **new/unseen lakes**

📂 v2_new_features
├── Jupyter notebooks for each sensor trained with engineered features
├── Ongoing work to improve performance on new/unseen lakes
└── Still **work in progress (WIP)**

```

---

## Acknowledgments

This research project was supported by NY Department of Environmental Conservation Grant #DEC01-C01714GG-3350000 (NYS-DEC) and NSF Grant AGS-2150432 (REU). Special appreciation to the New York State SCALE (Survey of Climate Change and Adirondack Lake Ecosystems) project for sharing the in-situ data.




