# League of Legends Match Prediction

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-success)](https://YOUR_USERNAME.github.io/YOUR_REPO)
[![Python](https://img.shields.io/badge/Python-3.8+-blue)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

**Predicting Match Outcomes from Early Game Statistics using Machine Learning**

![Project Banner](https://cdn1.epicgames.com/offer/24b9b5e323bc40eea252a10cdd3b2f10/EGS_LeagueofLegends_RiotGames_S1_2560x1440-47eb328eac5ddd63ebd096ded7d0d5ab)

## 🎮 Overview

This project applies supervised machine learning techniques to predict League of Legends match outcomes based solely on statistics captured at the 10-minute mark. Using a dataset of **9,879 Diamond-tier ranked games**, I trained and evaluated five classification models achieving approximately **72% prediction accuracy**.

## 📊 Key Findings

| Factor | Impact |
|--------|--------|
| **Gold Difference** | Strongest predictor (r = 0.51). Top quintile wins 87% |
| **First Blood** | +20 percentage point win rate advantage |
| **Dragon Control** | +22 percentage point win rate advantage |
| **Both Objectives** | 72% win rate when securing Dragon + Herald |

## 🤖 Models Implemented

- Logistic Regression (L2 regularization)
- Logistic Regression (L1/Lasso) - **Best Model**
- Decision Tree (GINI criterion)
- Random Forest (100 trees)
- SVM (RBF Kernel)

## 📁 Repository Structure

```
├── index.html                    # Project website
├── LoL_Final_Report_v2.ipynb    # Complete analysis notebook
├── high_diamond_ranked_10min.csv # Dataset
├── figure1_win_distribution_gold.png
├── figure2_feature_correlations.png
├── figure3_model_comparison.png
├── figure4_feature_importance.png
├── figure5_confusion_matrix.png
└── README.md
```

## 🚀 Quick Start

### View the Website
Visit: [https://YOUR_USERNAME.github.io/YOUR_REPO](https://YOUR_USERNAME.github.io/YOUR_REPO)

### Run the Analysis Locally

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

2. Install dependencies:
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

3. Open the notebook:
```bash
jupyter notebook LoL_Final_Report_v2.ipynb
```

## 📈 Results Summary

All models achieved approximately **72% test accuracy**, with Logistic Regression (L1) performing best in cross-validation:

| Model | Test Accuracy | CV Score |
|-------|---------------|----------|
| Logistic Regression (L2) | 72.4% | 73.4% ± 1.6% |
| **Logistic Regression (L1)** | **72.4%** | **73.5% ± 1.5%** |
| Decision Tree | 72.0% | 71.3% ± 0.8% |
| Random Forest | 72.0% | 72.9% ± 1.3% |
| SVM (RBF) | 71.8% | 72.7% ± 1.2% |

## 🎯 Strategic Recommendations

Based on the analysis:

1. **Prioritize Gold Income** - Focus on consistent CS (7-8 per minute)
2. **Secure First Blood** - +20% win rate when obtained
3. **Contest Dragon** - More impactful than Herald (+22% vs +12%)
4. **Minimize Deaths** - Strong negative correlation with winning

## 📚 Course Information

- **Course**: AOS C111/204 - Introduction to Machine Learning for Physical Sciences
- **Institution**: UCLA Department of Atmospheric and Oceanic Sciences
- **Instructor**: Dr. Alexander Lozinski
- **Date**: December 2024

## 📖 Data Source

[Kaggle - League of Legends Diamond Ranked Games (10 min)](https://www.kaggle.com/datasets/bobbyscience/league-of-legends-diamond-ranked-games-10-min)

## 📄 License

This project is for educational purposes as part of UCLA coursework.

---

**Author**: Aaron Wen  
**Contact**: [Your Email]
