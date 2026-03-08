# Titanic Survival Prediction (Logistic Regression)

This project builds a machine learning model to predict whether a passenger survived the Titanic disaster.

The model uses **logistic regression** and demonstrates a complete machine learning workflow including:

- Data cleaning
- Feature engineering
- Encoding categorical variables
- Feature scaling
- Model training
- Model evaluation
- Model interpretation

---

# Dataset

The dataset contains passenger information from the Titanic, including demographic and ticket information.

Key features include:

- Passenger Class
- Gender
- Age
- Ticket Fare
- Family relationships
- Boarding port

Target variable:

**Survived**
- 1 = Survived
- 0 = Did Not Survive

---

# Feature Engineering

Several engineered features were created to improve model performance:

### FamilySize
Combines siblings/spouses and parents/children aboard.

```
FamilySize = SibSp + Parch + 1
```

### IsAlone
Binary feature indicating whether the passenger traveled alone.

### Title
Passenger titles extracted from the Name column (Mr, Mrs, Miss, Master).

These titles capture information about gender and social roles.

---

# Model

The model used in this project is **Logistic Regression**.

Logistic regression predicts the probability of survival using a sigmoid function.

---

# Results

The final model achieved approximately:

**Accuracy: ~81%**

The most influential features included:

- Gender
- Passenger class
- Age
- Fare

These results align with historical accounts of the Titanic disaster.

---

# Project Structure

```
titanic-survival/
│
├── Titanic_LogisticRegression.ipynb
├── Titanic-Dataset.csv
└── README.md
```

---

# Key Takeaways

- Feature engineering significantly improves model performance.
- Logistic regression provides interpretable results through feature coefficients.
- Even simple machine learning models can perform well with thoughtful preprocessing.

---

# Future Improvements

Possible extensions include:

- Decision Trees
- Random Forest models
- Gradient Boosting models
- More advanced feature engineering
