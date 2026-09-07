# Wine Dataset PCA + Logistic Regression

A classic machine learning project demonstrating **Principal Component Analysis (PCA)** for dimensionality reduction and **Logistic Regression** for multi-class classification on the UCI Wine dataset.

## 📊 Dataset

- **Source**: `sklearn.datasets.load_wine()`  
- **Samples**: 178  
- **Features**: 13 (chemical composition of wines)  
- **Classes**: 3 (different cultivars)  

## 🚀 Project Workflow

1. Load the Wine dataset and create a DataFrame  
2. Split data into training and test sets (80/20, stratified)  
3. Standardize features using `StandardScaler`  
4. Perform PCA to analyze explained variance and select 6 principal components (~85% variance retained)  
5. Train Logistic Regression on:
   - Original 13 features  
   - Reduced 6 PCA components  
6. Evaluate and compare performance using 5-fold cross-validation  

## 📈 Results

| Method | Accuracy (CV mean) |
|--------|-------------------|
| Original (13 features) | 98.60% |
| PCA (6 components) | 99.31% |

**Conclusion**: PCA reduces feature dimensions from 13 to 6 while maintaining (and even slightly improving) predictive performance — an excellent demonstration of dimensionality reduction in practice.

## 📦 Installation

Clone this repository and install the required packages:

```bash
git clone https://github.com/Myscrayon/Wine-PCA-Classification.git
cd Wine-PCA-Classification
pip install -r requirements.txt
```

## 🖼️ Visualizations Included

- Scree plot: explained variance ratio (bar + cumulative line)
- 2D scatter plot: first two principal components, colored by wine class
- Accuracy comparison bar chart: original vs PCA-reduced data

## 📁 File Structure

```
.
├── Wine_PCA_Classification.ipynb   # Main Jupyter Notebook
├── README.md                       # Project overview
└── requirements.txt                # Python dependencies
```

## 👨‍💻 Author :  Myscrayon
