# 🛳 Titanic - Machine Learning from Disaster

This is my solution to the Titanic Kaggle competition: [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic). The goal is to predict whether a passenger survived the Titanic shipwreck based on features like age, gender, ticket class, and other attributes.

---

## 📂 Project Structure


---

## ✅ Features Used

- Passenger Class (`Pclass`)
- Sex
- Age (with missing values handled)
- Fare
- Embarked
- Title (extracted from Name)
- FamilySize (`SibSp + Parch + 1`)
- IsAlone (engineered from FamilySize)
- Ticket Price (scaled)
- More categorical variables encoded using Label Encoding

---

## 🧠 Machine Learning Models Tested

| Model                  | Accuracy |
|------------------------|----------|
| Logistic Regression    | 80.45%   |
| Support Vector Machine | 80.45%   |
| K-Nearest Neighbors    | 79.33%   |
| Naive Bayes            | 77.65%   |
| Decision Tree          | 61.45%   |
| Random Forest          | ~77%     |
| XGBoost                | ~78%     |

✅ **Best Model Selected:** Logistic Regression

---

## ⚙️ Preprocessing Steps

- Handled missing values (`Age`, `Embarked`)
- Extracted `Title` from names
- Encoded categorical variables using `LabelEncoder`
- Scaled numerical features using `StandardScaler`
- Feature engineering:
  - `FamilySize` = `SibSp + Parch + 1`
  - `IsAlone` = 1 if FamilySize == 1, else 0
  - `HouseAge` and `RemodAge` for house-related data (if used)

---

## 🧪 Evaluation

- **Train Accuracy:** ~80%
- **Kaggle Public Submission Score:** `0.67460`


---

## 📦 Dependencies

```bash
scikit-learn
xgboost
pandas
numpy
matplotlib
seaborn
ml models
🙋‍♂️ Author
Abid Ali Atif
Aspiring Data Scientist | 4th Semester CS Student
