# Titanic Preprocessing Assignment

## 1. Data Cleaning
- Age ki missing values ko Pclass ke median se bhara
- Cabin se Deck nikala (pehla letter) aur missing ko Unknown kiya
- Embarked ki 2 missing values ko Mode (S) se bhara

## 2. Age Categories Banayi
- Child (0-15), Young Adult (16-30), Adult (31-45), Middle Aged (46-60), Senior (60+)

## 3. Feature Engineering
- FamilySize = SibSp + Parch + 1
- Title = Name se Mr, Mrs, Miss, Master nikala
- Fare ko 4 hisso me baanta: Low, Medium, High, Very High
- Deck = Cabin ka pehla harf

## 4. Final Step
- Sex (male=0, female=1) aur Embarked ko number me badla
- Extra columns delete kiye

## Conclusion
Dataset ab bilkul clean hai aur ML model ke liye ready hai.
