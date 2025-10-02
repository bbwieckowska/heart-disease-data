# Heart Disease Dataset with Generated Variables

A processed clinical dataset with synthetically generated variables for evaluating binary classification methods.

## 📁 Available Datasets

- `heart_disease.rda` - Complete dataset (661 cases, 56 variables)
- `heart_disease_train.rda` - Balanced training set (331 cases)
- `heart_disease_test.rda` - Balanced test set (330 cases)  
- `heart_disease_train_imbalanced_30.rda` - 30% disease cases
- `heart_disease_train_imbalanced_10.rda` - 10% disease cases
- ... and other variants

## 🚀 Quick Start

```r
# Load any dataset
load("data/heart_disease.rda")

# Check structure
str(heart_disease)
summary(heart_disease)

# Basic analysis
table(heart_disease$disease)
boxplot(age ~ disease, data = heart_disease)
```
## 🔧 Regenerate Data
```r
source("R/generate_data.R")
# This will recreate all dataset files
```
## 📊 Dataset Description
Contains 661 complete cases with:

Real clinical variables (age, sex, cholesterol, etc.)

Generated random variables for method testing

Multiple train/test splits with different class imbalances

Detailed description of dataset: [heart_disease_description_0.1.0.pdf](heart_disease_description_0.1.0.pdf)

📝 Citation
Wieckowska, B. (2025). Heart Disease Dataset with Generated Variables for Method Validation (Version v0.1.0) [Data set]. GitHub. https://github.com/bbwieckowska/heart-disease-data

Janosi, A., Steinbrunn, W., Pfisterer, M., & Detrano, R. (1989). Heart Disease [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C52P4X.
