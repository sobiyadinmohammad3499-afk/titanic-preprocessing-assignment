# Titanic Dataset - Data Cleaning & Preprocessing Assignment

## Overview
This project focuses on cleaning and preprocessing the Titanic dataset to make it ready for Machine Learning.

Dataset: https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv

## 1. Handling Missing Values
- **Age (177 missing):** Filled using median age grouped by Pclass.
    - Pclass 1 median = 37, Pclass 2 = 29, Pclass 3 = 24
- **Cabin (687 missing):** Extracted Deck (first letter of Cabin) and filled missing with 'Unknown'.
- **Embarked (2 missing):** Filled with Mode value 'S' (Southampton).

## 2. Age Categories
Divided Age into 5 categories:
- Child (0-15), Young Adult (16-30), Adult (31-45), Middle Aged (46-60), Senior (60+)

## 3. Feature Engineering
- **FamilySize:** FamilySize = SibSp + Parch + 1
- **Title:** Extracted Title (Mr, Mrs, Miss, Master, Dr) from Name column
- **Fare:** Divided Fare into 4 bins - Low, Medium, High, Very High
- **FarePerPerson:** Fare / FamilySize
- **Deck:** Extracted first letter from Cabin column

## 4. Final Preprocessing
- Encoded Sex: male=0, female=1
- Encoded Embarked: S=0, C=1, Q=2
- Dropped unnecessary columns: PassengerId, Name, Ticket, Cabin

## Conclusion
The dataset is now fully clean with no missing values and is ready for model training (Logistic Regression / Random Forest).
