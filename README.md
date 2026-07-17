# Solar Active Region Detection Using Aditya-L1 SUIT Data

## Astronomy & Astrophysics: Heliophysics with Aditya-L1 Data

### India Space Academy Summer Training Program 2026

---

## Overview

The Sun is a highly dynamic star where magnetic activity drives several energetic phenomena such as solar flares, coronal mass ejections (CMEs), and ultraviolet brightenings. Identifying and studying solar active regions is an important step toward understanding solar activity and space weather.

This project presents an image-processing based approach for detecting solar active regions using observations from India's first dedicated solar mission, **Aditya-L1**.

The work focuses on developing a computational pipeline to process solar images, enhance important structures, and automatically identify regions of increased solar activity.

---

## Project Motivation

Solar active regions contain strong and complex magnetic fields and are the primary locations where energetic solar events originate.

Space-based solar observations provide high-quality data without atmospheric interference, enabling detailed analysis of these structures.

The aim of this project is to explore how computational image-processing techniques can assist heliophysics research by extracting meaningful features from solar imagery.

---

# Objectives

The main objectives of this work are:

- Study the Aditya-L1 mission and its role in solar physics
- Understand the formation and importance of solar active regions
- Process solar FITS images using Python-based tools
- Develop an automated active-region detection pipeline
- Apply segmentation and image analysis techniques
- Generate scientific visualizations of detected solar structures

---

# Data Source

## Aditya-L1 Mission

**Aditya-L1** is India's first dedicated solar observatory developed by the **Indian Space Research Organisation (ISRO)**.

The spacecraft is positioned near the Sun–Earth Lagrange Point 1 (L1), providing continuous observation of the Sun.

This project uses solar observations obtained from the:

**ISRO PRADHAN Data Archive**

### Dataset Information

- **Data Format:** FITS (Flexible Image Transport System)
- **Instrument:** Solar Ultraviolet Imaging Telescope (SUIT)
- **Observation Date:** 22 February 2024
- **Associated Solar Event:** X6.3 Class Solar Flare

The selected observation was chosen because it represents a period of enhanced solar activity suitable for active-region analysis.

---

# Methodology

The complete workflow consists of multiple image-processing stages:


---

# Image Processing Pipeline

## 1. Image Preprocessing

Raw solar images contain variations in intensity and noise.

The preprocessing stage improves image quality by:

- Normalizing pixel intensity values
- Reducing unwanted noise
- Enhancing solar structures

---

## 2. Active Region Detection

Solar active regions appear as enhanced intensity structures compared to the surrounding solar surface.

The project uses:

### Otsu Thresholding

An automatic threshold selection technique that separates high-intensity solar regions from the background.

The generated binary mask identifies potential active regions.

---

## 3. Morphological Processing

Morphological operations are applied to remove small false detections and improve the quality of detected structures.

This step helps produce cleaner and more reliable active-region boundaries.

---

## 4. Connected Component Analysis

Individual solar structures are identified and labelled.

For each detected region, information such as:

- Area
- Location
- Boundary coordinates
- Shape properties

can be extracted.

---

# Results

The developed pipeline successfully identified solar active regions from Aditya-L1 observations.

### Output Generated:

✔ Normalized solar intensity maps  
✔ Binary active-region masks  
✔ Noise-reduced segmentation results  
✔ Detected active-region visualization  

### Detection Result:

**Number of detected active regions: 4**

The results demonstrate that classical image-processing methods can effectively extract solar structures from ultraviolet observations.

---

# Tools and Technologies

## Programming Language

Python

## Environment

Google Colab / Jupyter Notebook

## Scientific Libraries

- SunPy
- Astropy
- NumPy
- SciPy
- Matplotlib
- Scikit-image
- Pandas

---


---

# Future Extensions

This project establishes the foundation for advanced solar analysis.

Possible future directions include:

- Tracking active regions over time
- Studying solar evolution using multiple observations
- Comparing different segmentation algorithms
- Combining intensity observations with magnetic field measurements
- Applying machine learning techniques for solar activity prediction

---

# Acknowledgement

This project was completed as part of the:

**India Space Academy Summer Training Program 2026**

under the domain:

**Astronomy & Astrophysics: Heliophysics with Aditya-L1 Data**

I sincerely acknowledge the guidance and support provided by:

**Dr. Ashok Gopalkrishnan**  
Program Supervisor, India Space Academy

I also acknowledge ISRO's Aditya-L1 mission and publicly available scientific data resources that made this analysis possible.

---

# Author

**Shikshita Naryal**

M.Sc. Physics  
Central University of Himachal Pradesh

Research Interests:

- Astrophysics
- Solar Physics
- Space Science
- Computational Astronomy

---

# References

1. Tripathi et al., "The Aditya-L1 Mission of ISRO," arXiv:2212.13046, 2022.

2. Patel et al., "Characterizing Spectral Channels of Visible Emission Line Coronagraph of Aditya-L1," Frontiers in Astronomy and Space Sciences, 2021.

3. Goyal et al., "Aditya Solarwind Particle EXperiment (ASPEX) onboard the Aditya-L1 mission," Planetary and Space Science, 2018.

