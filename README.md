# Brain Stroke Prediction Project

Brain strokes are one of the leading causes of disability and death globally. Early detection and preventive measures can significantly reduce the impact of strokes. This project focuses on building a machine learning model that predicts the likelihood of an individual experiencing a stroke based on various health and lifestyle factors. 

The dataset used in this project includes demographic, medical, and lifestyle attributes such as age, gender, hypertension, heart disease, marital status, smoking habits, and more. By analyzing these factors and applying machine learning techniques, we aim to build a robust model that can assist healthcare professionals in identifying high-risk individuals for timely intervention.

Using popular machine learning algorithms like Logistic Regression, Decision Trees, Naive Bayes, and Random Forest, this project compares their performance and chooses the best model to predict stroke occurrences.

The primary goal of this project is to predict whether an individual will experience a stroke based on a range of health and demographic factors. By analyzing features such as age, gender, hypertension, heart disease, and smoking habits, the machine learning models aim to identify individuals at high risk for stroke, helping in early intervention.

### Key Highlights:
- **Dataset**: The dataset consists of multiple health and demographic variables that can influence stroke occurrences.
- **Target Variable**: The target variable is `stroke` (1 if the individual had a stroke, 0 if not).
- **Models Used**: Various machine learning models, including Logistic Regression, Decision Trees, Naive Bayes, and Random Forest, were trained and tested to predict stroke occurrences.
- **Evaluation Metrics**: The models were evaluated based on accuracy, precision, recall, and F1-score. Hyperparameter tuning was also conducted for Random Forest to enhance performance.

## Dataset Information

- **Source**: The dataset is sourced from Kaggle.
- **File Name**: `full_data.csv`
- **Features**:
  - `gender`: Gender of the person
  - `age`: Age of the person
  - `hypertension`: Whether the person has hypertension (1: Yes, 0: No)
  - `heart_disease`: Whether the person has heart disease (1: Yes, 0: No)
  - `ever_married`: Marital status
  - `work_type`: Type of work the person does
  - `Residence_type`: Urban or rural residence
  - `avg_glucose_level`: Average glucose level of the person
  - `bmi`: Body Mass Index
  - `smoking_status`: Smoking status (never smoked, formerly smoked, smokes)
  - `stroke`: Target column (1: Stroke occurred, 0: No stroke)

## Data Preprocessing

- Missing values in the dataset were handled, and categorical variables were encoded using `LabelEncoder` for machine learning compatibility.
- Features like `work_type`, `gender`, `smoking_status`, `ever_married`, and `Residence_type` were converted into numerical format for modeling.
  
## Exploratory Data Analysis

- **Gender Distribution**: Visualized using a pie chart to show the ratio of males to females in the dataset.
- **Stroke Analysis**: Analyzed how stroke occurrences vary based on gender, smoking status, and marital status.
- **Correlation Heatmap**: Visualized relationships between various features to identify significant predictors of stroke.

## Modeling

Multiple classifiers were used to predict strokes, and their performances were compared:
- **Naive Bayes**
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**: Hyperparameter tuning was done using a parameter grid to optimize the Random Forest classifier for improved prediction accuracy.
  
## Results

- **Naive Bayes**: Achieved an accuracy of 86.35%
- **Logistic Regression**: Achieved the highest accuracy of 95.65%
- **Decision Tree**: Achieved 90.50% accuracy
- **Random Forest**: After hyperparameter tuning, the Random Forest model also achieved strong performance, comparable to Logistic Regression.
