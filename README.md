# 🚢 Titanic: EDA and Logistic Regression

An end-to-end beginner ML workflow on the **Titanic dataset**: explore the data, clean it, engineer features, and train a classifier to predict passenger survival.

## 🧠 Workflow
1. **Explore:** survival by sex, passenger class and age, with Seaborn count plots and histograms
2. **Missing data:** spot gaps with a heatmap
   - `Age`: filled with the **typical age for each passenger class** (37 / 29 / 24 for 1st / 2nd / 3rd class), since first-class passengers tended to be older
   - `Cabin`: dropped (mostly empty)
   - Remaining rows with missing values (two in `Embarked`): dropped
3. **Encode categories:** converted `Sex` and `Embarked` into dummy variables
4. **Model:** 70/30 train/test split, then `LogisticRegression`
5. **Evaluate:** confusion matrix on the test set

## 🛠️ Tech stack
pandas · NumPy · Seaborn · Matplotlib · scikit-learn

## 🚀 Run it
```bash
pip install pandas numpy seaborn matplotlib scikit-learn jupyter
jupyter notebook "EDA (Exploratory Data Analysis).ipynb"
```
Dataset: `Titanic-Dataset.csv` (included).

## 🔮 Next improvements
Report accuracy, precision and recall; try tree-based models; add family-size and title features.

---
👩‍💻 **Nidhi Mehta** · [GitHub](https://github.com/itsnidhimehta)
