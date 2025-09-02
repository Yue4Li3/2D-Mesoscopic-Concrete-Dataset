# 2D-Mesoscopic-Concrete-Dataset
150 mesoscopic 2D concrete models with varying specimen sizes and aggregate fractions; includes images (.jpg) and pixel data (.csv).

# 🏗️ 2D Mesoscopic Concrete Dataset

This repository provides a dataset of **150 mesoscopic 2D concrete models** generated for research in **concrete mesostructure, durability, and machine learning applications**.  
The dataset follows open science principles but is restricted for **non-commercial use only**.

---

## 📦 Dataset Description
- **Sizes:** 100 × 100 mm, 150 × 150 mm, 200 × 200 mm  
- **Aggregate fractions:** 20%, 30%, 40%, 50%, 60%  
- **Per model:**  
  - `.jpg` → mesoscopic cross-section image  
  - `.csv` → pixel-level binary data (aggregate vs mortar)  
- **Total models:** 150  

---

## 📂 File Naming Convention
Each file is named:
AGin_<size><agg%><id>.jpg
AGin_<size><agg%><id>.csv


- `<size>` → specimen size in mm (100, 150, 200)  
- `<agg%>` → aggregate volume fraction (20, 30, 40, 50, 60)  
- `<id>` → model index  

**Example:**  
- `AGin_200_30_2.jpg` → 2nd model, size = 200 × 200 mm, aggregate fraction = 30%  
- `AGin_200_30_2.csv` → corresponding pixel-level data  

---

## 🔧 Example Usage

### Load and Visualize CSV in Python
```python
import pandas as pd
import matplotlib.pyplot as plt

# Load CSV data (no header)
data = pd.read_csv("AGin_200_30_2.csv", header=None)

# Visualize
plt.imshow(data, cmap="gray")
plt.title("Concrete Mesostructure (200mm, 30% agg)")
plt.show()
