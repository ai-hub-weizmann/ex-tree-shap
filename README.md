# Trees and SHAP Tutorial

**Author:** Saar Shoer  
**Updated by:** David Krongauz  
**Managed by:** Tamar Kashti

---

## Overview

This tutorial teaches you about machine learning for predicting COVID-19 diagnosis from symptoms. It's designed for beginners with basic Python knowledge.

**Part 1: Gradient Boosting Decision Trees** - Learn how to build a machine learning model that predicts whether someone might test positive for COVID-19 based on their symptoms. You'll learn how to train the model, test it properly, and make sure it works well on new data.

**Part 2: SHAP (Model Interpretation)** - Learn how to understand what your model learned. SHAP helps explain which symptoms are most important for predictions and how different factors interact with each other.

---

## Tutorial Files

### Jupyter Notebooks (Work through these in order)
1. **ex-trees.ipynb** - Part 1 of the tutorial
   - Build and train a Gradient Boosting model
   - Learn to split data for training and testing
   - Evaluate model performance with ROC, PR curves, and calibration
   - Tune model hyperparameters to improve accuracy
   - Complete exercises with step-by-step guidance

2. **ex-shap.ipynb** - Part 2 of the tutorial
   - Load the model you trained in Part 1
   - Calculate SHAP values to explain predictions
   - Visualize which features matter most
   - Understand feature interactions
   - Complete exercises with step-by-step guidance

### Data Files
- **data/data.csv** - The main dataset with COVID-19 symptoms and diagnoses
  - Contains 43,752 samples
  - 9 features (age, gender, symptoms like cough, fever, etc.)
  - Labels indicating COVID-19 test results

- **data/predictions.csv** - External dataset for testing your model
  - Used to validate that your model works on new data
  - Includes predictions and actual results

### Documentation
- **README.md** - This file with instructions and overview

---

## Prerequisites

### Required Software
- **Python 3.7+** installed on your computer
- **Jupyter Notebook** or **VS Code** with Jupyter extension

### Required Python Packages
You'll need these libraries (install them before starting):
```bash
pip install numpy pandas matplotlib xgboost scikit-learn shap seaborn
```

### Required Knowledge
- Basic Python programming (variables, functions, loops)
- Basic understanding of data in tables (like spreadsheets)
- No advanced math or machine learning experience required!

---

## How to Complete This Tutorial

### Step 1: Set Up Your Environment
1. Open this folder in VS Code or Jupyter
2. Install all required Python packages (see above)
3. Make sure you can see the `data/` folder with the CSV files

### Step 2: Complete Part 1 (ex-trees.ipynb)
1. Open **ex-trees.ipynb**
2. Read through each cell carefully - there are explanations mixed with code
3. Run each code cell in order from top to bottom
4. Complete the exercises when you see empty cells
5. **Important**: At the end, save your trained model - you'll need it for Part 2!

**Time estimate**: 2-4 hours

### Step 3: Complete Part 2 (ex-shap.ipynb)
1. Make sure you completed Part 1 and saved your model
2. Open **ex-shap.ipynb**
3. Load the model you saved in Part 1
4. Follow the same process: read, run, and complete exercises
5. Learn how to interpret what your model learned

**Time estimate**: 1-2 hours

---

## What You'll Learn

### Technical Skills
- How to load and clean data
- How to split data for training and testing
- How to train a Gradient Boosting model
- How to evaluate model performance
- How to tune hyperparameters
- How to interpret model predictions with SHAP

### Conceptual Understanding
- Why accuracy alone isn't enough for imbalanced datasets
- The importance of validation on external data
- How to visualize model performance (ROC, PR curves)
- Why some predictions are more confident than others
- Which features drive model predictions

---

## Tips for Success

1. **Run cells in order** - Each cell often depends on previous ones
2. **Don't skip the reading** - The markdown cells explain important concepts
3. **Try to solve exercises yourself first** - Learning happens through practice
4. **Ask questions** - If something isn't clear, look it up or ask for help

---

## Real-World Context

This tutorial recreates a model from a real research paper:
> "A Prediction Model to Prioritize Individuals for a SARS-CoV-2 Test Built from National Symptom Surveys" by Shoer et al., Cell Med (2020)  
> https://doi.org/10.1016/j.medj.2020.10.002

During the early COVID-19 pandemic, testing was limited. This model helped prioritize who should get tested first by predicting who was most likely to test positive based on their symptoms. This improved testing efficiency and helped identify cases faster.

---

## Troubleshooting

**Problem**: Package import errors  
**Solution**: Make sure all packages are installed: `pip install numpy pandas matplotlib xgboost scikit-learn shap seaborn`

**Problem**: File not found errors  
**Solution**: Make sure you're running the notebook from the correct directory and the `data/` folder exists

**Problem**: Model file not found in Part 2  
**Solution**: Go back to Part 1 and complete the "Saving the Model" section

**Problem**: Code takes too long to run  
**Solution**: Some operations (like GridSearchCV) can take several minutes - this is normal

---

## Additional Resources

- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- [SHAP Documentation](https://shap.readthedocs.io/)
- [Original Paper](https://doi.org/10.1016/j.medj.2020.10.002)
