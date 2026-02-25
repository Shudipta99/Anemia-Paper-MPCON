<div align="center">

<!-- Optional: add your logo file at ./assets/logo.png -->
<img src="assets/logo.png" width="120" alt="Project Logo" />

# Addressing Trust and Efficiency in Pediatric Anemia Diagnosis Using Interpretable Decision Trees

**Accepted at 15th CSNT 2026**

<!-- Badges -->
<p>
  <a href="#"><img alt="Conference" src="https://img.shields.io/badge/CSNT-2026-6a5acd?style=for-the-badge"></a>
  <a href="#"><img alt="Status" src="https://img.shields.io/badge/Status-Accepted-2ea44f?style=for-the-badge"></a>
  <a href="#"><img alt="Python" src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
  <a href="#"><img alt="Notebook" src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white"></a>
  <a href="#"><img alt="License" src="https://img.shields.io/badge/License-MIT-black?style=for-the-badge"></a>
</p>

<!-- Quick links -->
<p>
  <a href="#-highlights">Highlights</a> •
  <a href="#-pipeline-from-the-notebook">Pipeline</a> •
  <a href="#-getting-started">Getting Started</a> •
  <a href="#-results--artifacts">Results</a> •
  <a href="#-citation">Citation</a>
</p>

<!-- Animation / demo (put a gif at ./assets/demo.gif) -->
<img src="assets/demo.gif" width="820" alt="Demo animation (add assets/demo.gif)" />

</div>

---

## 🔥 Highlights

- 🧠 **Interpretable** and **trust-oriented** pediatric anemia diagnosis pipeline  
- ⚡ **Efficient** feature selection for practical deployment  
- 🧪 Built directly from the notebook workflow: `anemia_s.ipynb`  
- 📊 Feature importance and optimization for transparent decision support  

---

## 🧬 Pipeline (from the notebook)

This repository follows the exact steps implemented in **`anemia_s.ipynb`**:

1. **Data Loading** (Excel → DataFrame)  
2. **Preprocessing**
   - Gender encoding (LabelEncoder)
   - Outlier handling using **IQR + median capping**
3. **Statistical Feature Selection**
   - MinMax scaling
   - **Chi-square** test (remove insignificant features)
4. **Genetic Algorithm Feature Selection** (DEAP)
   - Fitness: 5-fold CV accuracy (RandomForest)
   - Tracks fitness evolution across generations
5. **Model-free Feature Importance**
   - **Mutual Information** ranking + visualization

---

## 📁 Repository Structure

```text
.
├── anemia_s.ipynb              # Main notebook (full pipeline)
├── Anemia Dataset.xlsx         # Dataset (if shareable)

├── figures/                  
└── README.md
