# Wine Quality Data Ethics Check

## Overview
This project demonstrates a quick **data ethics analysis** on the Wine Quality dataset.  
The goal is to evaluate balance, fairness, and potential biases before applying predictive models.  
By combining Python, pandas, and seaborn, the script produces both a console report and a visualization.

---

## Dataset
- **Source:** Wine Quality dataset (UCI / Kaggle)  
- **File:** `WineQT.csv`  
- **Rows:** 1143  
- **Columns:** 13 (including physicochemical properties and quality ratings)

---

## Analysis Performed
1. **Missing Values Check**  
   - Verified dataset completeness.  
   - No missing values detected.

2. **Quality Ratings Distribution**  
   - Majority concentrated around scores 5 and 6.  
   - Very few extreme ratings (3, 4, 8).  
   - Imbalance ratio flagged at ~80:1 between majority and minority classes.

3. **Alcohol Content Statistics**  
   - Values ranged between 8.4 and 14.9.  
   - No unrealistic outliers detected.  
   - Mean alcohol content ~10.4.

4. **Visualization**  
   - Bar chart of quality distribution saved as `wine_quality_distribution.png`.

---

## Ethics Report
- **Balance:** Dataset is moderately imbalanced in quality ratings.  
- **Fairness:** Models trained on this dataset may overfit to majority classes.  
- **Transparency:** Clear reporting of imbalance ensures responsible use.  
- **Suitability:** Dataset is usable for modeling, but fairness adjustments (e.g., resampling, weighting) are recommended.

---

## Conclusion
After thorough analysis, the Wine Quality dataset shows no missing values, a moderate imbalance in quality ratings, and alcohol values within expected ranges.  
This makes it suitable for modeling tasks, but ethical considerations around class imbalance should be addressed to ensure fair evaluation.  
The dataset provides a strong foundation for exploring predictive models while keeping **responsible data practices** in mind.

---

## How to Run
1. Clone this repository.  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
