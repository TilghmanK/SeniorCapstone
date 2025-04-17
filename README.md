# SeniorCapstone

# Replicating X-ray data analysis of Tycho SNR

# 🌠 Tycho's Supernova Remnant

> *"Decoding stellar explosions through machine learning and X-ray vision."*

![Tycho Banner](./assets/tycho_banner.png) <!-- Optional: custom image goes here -->

---

## 🧭 Mission Control

This project explores the **Tycho Supernova Remnant (SN 1572)** using **Principal Component Analysis (PCA)** on X-ray flux maps. We aim to uncover the internal structure, asymmetries, and shock morphologies embedded in the stellar debris of this Type Ia supernova.

---

## 🛰 Data Payload

- 🧊 **FITS images** from Chandra across multiple energy bands  
- 🚀 Preprocessed, aligned, and stacked using `astropy` & `scipy`  
- 🌐 PCA applied using `scikit-learn`

---

## 🔬 Scientific Objectives

- 📌 Extract **principal components** from flux data (focus on PC1)
- 📈 Generate **radial profiles** to map structure as a function of radius
- 🔁 Identify **asymmetries and shell contours** across the remnant
- 🧩 Compare with literature (e.g., Warren et al. 2005)

---

## 🌌 Visuals from the Void

| 🖼️ Visualization | Description |
|------------------|-------------|
| ![PC1 Image](./assets/pc1_overlay.png) | *First Principal Component with overlaid contours* |
| ![Radial Profile](./assets/radial_profile.png) | *Radial intensity profile of PC1* |

---

## 🛠 Reproducibility

```bash
git clone https://github.com/yourusername/tycho-pca.git
cd tycho-pca
pip install -r requirements.txt
python tycho_pca_analysis.py
