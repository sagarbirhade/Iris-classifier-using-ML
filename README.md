# Iris-classifier-using-ML

Iris Species Classifier Project

This project implements a machine learning model using a Decision Tree Classifier to predict the species of an Iris flower based on its sepal and petal measurements. Here's an overview:

Dependencies:
pandas (data manipulation)
numpy (numerical operations)
matplotlib.pyplot (data visualization)
seaborn (advanced data visualization)
sklearn (machine learning library)
streamlit (web framework for deployment)
pickle (model serialization)

Instructions:
1. Setup Environment:
Install the required dependencies using pip install pandas numpy matplotlib seaborn scikit-learn streamlit pickle.
Make sure you have Python and the mentioned libraries installed.

2. Data Exploration and Preprocessing
The code reads the Iris dataset from a CSV file (iris.csv). You'll need to place this file in the same directory as your Python script.
It performs basic data exploration tasks, including checking for missing values, species distribution, and visualizing relationships between features.
It encodes the categorical Species feature into numerical values for training the model.
The Id column (if present) is dropped, assuming it's not relevant for prediction.

3. Model Training and Evaluation
The code splits the data into training and testing sets using train_test_split from sklearn.model_selection.
A Decision Tree Classifier is created from sklearn.tree.
The model is trained on the training data.
Predictions are made on both training and testing data, and accuracy is calculated using accuracy_score from sklearn.metrics.
The decision tree is visualized using plot_tree from sklearn.tree.
Feature importances are calculated and displayed.

4. Model Deployment
The trained model is saved using pickle for later use.
A Streamlit app is created to take user input for the four Iris flower features (Sepal Length, Sepal Width, Petal Length, Petal Width).
Based on the user's input, the model predicts the flower species and displays the result.

5. Running the Project
Open a terminal in the project directory and run python your_script_name.py.
The Streamlit app will launch in your web browser, typically at http://localhost:8501.

Example Usage:
1. Enter values for Sepal Length, Sepal Width, Petal Length, and Petal Width in the Streamlit app.
2. Click the "Predict" button.
3. The app will display the predicted species of the Iris flower (Iris-setosa, Iris-versicolor, or Iris-virginica).
