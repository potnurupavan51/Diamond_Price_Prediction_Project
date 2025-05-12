# **Diamond Price Prediction Project**

## **Overview**
 
This project aims to predict the price of diamonds using a regression analysis approach. A dataset containing various attributes of diamonds (carat, cut, color, clarity, etc.) is used to train several regression models. The best-performing model can then be used to estimate the price of a diamond given its characteristics.

## **Technologies Used**

* Python  
* Pandas  
* Scikit-learn  
* Flask  
* Matplotlib  
* Seaborn

## **Project Description**

The project involves building a predictive model for diamond prices. The following steps are performed:

1. **Data Ingestion:** The gemstone dataset is read using Pandas.  
2. **Exploratory Data Analysis (EDA):** The dataset is analyzed to understand its characteristics, including data types, missing values, duplicate values, and statistical distributions.  
3. **Data Preprocessing:**  
   * Irrelevant features are dropped.  
   * Categorical features are encoded using ordinal encoding based on domain expertise.  
   * Numerical features are scaled using standard scaling.  
   * The data is split into training and testing sets.  
4. **Model Training:** Several regression models are trained, including:  
   * Linear Regression  
   * Lasso Regression  
   * Ridge Regression  
   * Elastic Net Regression  
5. **Model Evaluation:** The performance of each model is evaluated using metrics such as:  
   * R-squared  
   * Mean Absolute Error (MAE)  
   * Root Mean Squared Error (RMSE)  
6. **Web Application (Optional):** A Flask application is created to provide a web interface for making price predictions.

## **Dataset Description**

The dataset contains information about various attributes of diamonds, with the goal of predicting their price.

### **Independent Variables**

* carat: Carat weight of the diamond.  
* cut: Quality of the diamond cut (Fair, Good, Very Good, Premium, Ideal).  
* color: Color of the diamond (D, E, F, G, H, I, J).  
* clarity: Diamond clarity (I1, SI2, SI1, VS2, VS1, VVS2, VVS1, IF).  
* depth: The height of the diamond, from culet to table.  
* table: The width of the diamond's table.  
* x: Length of the diamond.  
* y: Width of the diamond.  
* z: Depth of the diamond.

### **Target Variable**

* price: Price of the diamond.

### **Dataset Source**

The dataset is obtained from Kaggle: [https://www.kaggle.com/datasets/soumyakushwaha/gemstone?resource=download](https://www.kaggle.com/datasets/soumyakushwaha/gemstone?resource=download)

## **Installation**

1. Clone the repository.  
2. Install the required Python packages:  
   pip install pandas scikit-learn Flask

   You might also need to install matplotlib and seaborn if you want to run the EDA part of the code.  
   pip install matplotlib seaborn

## **Usage**

1. **Run the Flask application (Optional):**  
   * Navigate to the directory containing the code.  
   * Run the following command:  
     python app.py

   * Open a web browser and go to http://0.0.0.0:5000 to use the prediction form.  
2. Run the prediction code directly:  
   The provided notebook contains the code to read the data, train the model and make the predictions. You can directly run the jupyter notebook.

## **File Structure**

* README.md: This file.  
* app.py: (Optional) Flask application code.  
* notebook: Jupyter Notebook with the data processing, model training, and evaluation code.  
* data/gemstone.csv: The dataset.  
* src: Source code.
