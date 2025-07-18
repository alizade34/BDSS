# 🌳 Trees and Random Forests for Univariate/Multivariate Time Series Prompt Classification

## 🎯 Project Overview

This project implements tree-based methods for time series classification as described in the BDSS 24/25 assignment, featuring advanced prompt tree algorithms and random forest implementations for both univariate and multivariate time series data.

## 📁 Project Structure

```
prompt_trees/
├── data/                      # Generated datasets (.npy files)
├── results/
│   ├── figures/               # Generated plots and visualizations
│   └── metrics/               # Evaluation results (.json files)
├── notebooks/
│   └── main_analysis.ipynb    # Complete implementation notebook
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
```

**Note**: All implementations are contained within the `main_analysis.ipynb` notebook, providing a complete, self-contained solution.

## ✨ Features

### 1. Prompt Tree Implementation
- Reference Slice Tests (RST) for univariate data
- Channel Reference Slice Tests (CRST) for multivariate data
- Customizable distance functions
- Post-pruning validation
- Path extraction for distance calculations

### 2. Random Forest Implementation
- Three voting mechanisms:
  - Majority voting
  - Weighted voting
  - Track-record voting
- Support for both supervised and unsupervised approaches
- Isolation forest for unsupervised learning

### 3. Distance Functions
- **Breiman Distance**: Traditional tree-based distance
- **Zhu Distance**: Enhanced distance metric
- **RatioRF Distance**: Ratio-based distance

### 4. Clustering
- Hierarchical clustering using tree distances
- Internal validation (intra/inter-cluster distances)
- External validation (purity/entropy metrics)
- Adjusted Rand Index (ARI) comparison

### 5. Evaluation
- Supervised learning evaluation with accuracy metrics
- Conformal prediction with miscalibration and efficiency
- Unsupervised clustering evaluation
- Comprehensive visualization

## 🚀 Installation

```powershell
pip install -r requirements.txt
```

## 💻 Usage

The complete implementation is contained within a single Jupyter notebook:

```powershell
jupyter notebook notebooks/main_analysis.ipynb
```

This notebook contains:
- All class implementations (PromptTree, PromptRandomForest, etc.)
- Complete evaluation pipeline
- Data generation and preprocessing
- Comprehensive visualizations
- Results analysis and export

## 📊 Dataset Requirements

### Univariate Time Series
- Binary classification datasets
- Multi-class classification datasets (3+ classes)
- Source: http://www.timeseriesclassification.com/aeon-toolkit/Archives/Univariate2018_ts.zip

### Multivariate Time Series
- Binary classification datasets
- Multi-class classification datasets (3+ classes)
- Source: http://www.timeseriesclassification.com/aeon-toolkit/Archives/Multivariate2018_ts.zip

## 🔬 Implementation Details

### Prompt Tree Algorithm
The implementation follows the PromptTreeFit algorithm with customizable components:
- **Promptness Function (fp)**: Determines intervals to consider
- **Sampling Function (fs)**: Generates candidate tests
- **Classification Function (fc)**: Determines output distribution
- **Distance Functions (∆)**: Set of distance functions
- **Optimization Function (fo)**: Selects optimal test
- **Stopping Criterion (fe)**: Determines when to create leaf nodes

### Random Forest Features
- Bootstrap sampling for tree diversity
- Feature randomness for improved generalization
- Multiple voting strategies for robust predictions
- Isolation forest mode for anomaly detection

## 📈 Results

All results, including model performance metrics, visualizations, and clustering analyses, are saved in the `results/` directory.

## 🎯 Key Achievements

- ✅ Complete implementation of prompt tree algorithms
- ✅ Advanced random forest with multiple voting mechanisms
- ✅ Comprehensive evaluation pipeline
- ✅ Support for both supervised and unsupervised learning
- ✅ Professional visualizations and analysis

## 👤 Author

**Emil Alizada**  
*Biomedical Decision Support Systems Course*  
*4th Semester, 2025*

---

**Author**: Emil Alizada  
**Course**: Biomedical Decision Support Systems  
**Status**: ✅ Complete | **Last Updated**: July 21, 2025
