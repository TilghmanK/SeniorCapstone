# 🌌 Tycho Supernova Remnant: Exploration of Fluid Discontinuities through Chandra X-Ray Images

![Banner](./assets/tycho_modern_banner.png)

> *"We applied PCA to multi-band X-ray flux maps of Tycho’s supernova remnant—not to extract textbook components, but to visualize structure and uncover the elusive reverse shock."*

---

## 🧭 Project Summary

In this project, we perform **Principal Component Analysis (PCA)** on Chandra X-ray images of **Tycho's Supernova Remnant (SN 1572)**. While PCA did not yield clean physical decompositions as initially expected, it revealed morphological features that align with theoretical expectations for a **reverse shock** structure.

---

## 🔍 Scientific Context

- **Tycho SNR** is a classic Type Ia supernova remnant exhibiting shell-like morphology.
- **Reverse shocks** are inward-moving shocks that heat the stellar ejecta.
- Traditional spectral analysis is limited by resolution—so we explored **unsupervised PCA** as a tool for structural insight.

---

## 📈 What We Found

| Visualization | Description |
|---------------|-------------|
| ![PC1](./assets/pc1_overlay.png) | **PC1 Map**: Morphology suggests presence of a reverse shock |
| ![Radial Profile](./assets/radial_profile.png) | **Radial Intensity**: Non-monotonic behavior consistent with a second shock front |
| ![Contours](./assets/contours.png) | **Contours**: Shell structure and asymmetry visualized |

---

## 🧪 Methodology

1. **Data Preparation**
   - Chandra X-ray flux maps (multi-band)
   - FITS preprocessing, image alignment, interpolation

2. **PCA Application**
   - Flattened flux image stack → PCA via `scikit-learn`
   - Focus on PC1 for dominant variance and structure

3. **Post-PCA Analysis**
   - Radial profile computation from explosion center
   - Visual comparison to theoretical shock structures

---

## 🚀 Usage

```bash
git clone https://github.com/yourusername/tycho-pca.git
cd tycho-pca
pip install -r requirements.txt
python tycho_pca_analysis.py
