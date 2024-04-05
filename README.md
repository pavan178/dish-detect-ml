# DishDetect Machine Learning Pipeline


## 🧠 Machine Learning Pipeline

The DishDetect project leverages a machine learning pipeline to classify images of various dishes based on attributes such as Taste, Healthiness, Ingredients, and Likeness. The pipeline involves several stages of data processing and model building.

## 📊 Input Data

The pipeline begins with data from a CSV file provided by the ML library. The following features are utilized as input:

- Ingredients
- Diet
- Home or Restaurant
- Healthiness Rating (integer)
- Likeness
  
Categorical features are encoded into numerical values. Ingredient data is cleaned, and lemmatization is applied for preprocessing. The TF-IDF method is employed to extract important ingredients and vectorize the feature set. After preprocessing, the input data expands to 1635 columns.

## 🔄 Transformation Stage

A Random Forest classifier is utilized to reduce the dimensionality of the feature set. Features with importance scores above the threshold of 0.01 are retained, resulting in the identification of 22 significant columns.

## 🤖 Modeling

Ensembling techniques along with grid search are employed to discover the best parameters and models. The following classification algorithms are considered:

- Random Forest
- Support Vector Classifier (SVC)
- Logistic Regression

These models are renowned for their effectiveness in classification tasks.

## 📝 Methodology

The dataset is split into training and testing sets using an 80:20 ratio. The models are trained on the training dataset and evaluated based on various metrics including accuracy score, confusion matrix, precision, and recall. This thorough assessment helps in selecting the most suitable model for dish classification.

## 🚀 Let's Get Cooking!

DishDetect streamlines the process of identifying and categorizing dishes, making it easier to analyze culinary data and enhance decision-making in various contexts. 
