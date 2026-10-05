 Canteen Food Demand Predictor

📌 Project Overview

The Canteen Food Demand Predictor is a beginner-friendly Machine Learning project that predicts how many plates of a particular food item a college canteen is likely to sell.

The project uses historical/synthetic canteen sales data and factors such as:

Day of the week

Weather

Food item

Food price

Previous day's sales

Exam day

Weekend

A Random Forest Regression model is trained to learn the relationship between these factors and the number of plates sold.

The project is designed to run in Google Colab and uses an interactive prediction interface.

🎯 Problem Statement

College canteens often face difficulty estimating how much food to prepare each day.

If too much food is prepared:

Food may be wasted.

The canteen may lose money.

If too little food is prepared:

Popular food items may sell out.

Students may not get the food they want.

This project uses Machine Learning to estimate food demand and help the canteen decide approximately how many plates to prepare.

💡 Proposed Solution

The system takes information about the upcoming day and predicts the expected number of plates that may be sold.

Input

Day

Weather

Food item

Price

Previous sales

Exam day

Weekend

Output

Predicted number of plates to be sold

Example:

Predicted demand: 112 plates of Samosa

The canteen can use this prediction to plan food preparation.

🤖 Machine Learning Algorithm

Random Forest Regression

The project uses Random Forest Regressor because it works well with multiple input features and can learn non-linear relationships between the input factors and food demand.

The model creates multiple decision trees and combines their predictions to produce the final demand estimate.

📊 Dataset

The project uses a CSV dataset named:

canteen_sales_dataset.csv

The dataset contains 1,000 synthetic records.

Dataset Columns

Column

Description

day

Day of the week

weather

Sunny, Cloudy, or Rainy

food_item

Type of food sold

price

Price of the food item

previous_sales

Previous sales of the food item

exam_day

1 = Exam day, 0 = Normal day

weekend

1 = Weekend, 0 = Weekday

sales

Number of plates sold

Food Items Included

Samosa

Poha

Dosa

Vada Pav

Pav Bhaji

Biryani

Sandwich

Maggi

Important Note

The dataset used in this project is synthetically generated data for educational and demonstration purposes. It is not collected from an actual college canteen.

For a real-world implementation, the model should be trained using actual historical canteen sales data.

🛠️ Technologies Used

Python

Google Colab

Pandas – Data handling

NumPy – Numerical operations

Matplotlib – Data visualization

Scikit-learn – Machine Learning

IPyWidgets – Interactive prediction interface

🔄 Project Workflow

              Canteen Sales Dataset
                       ↓
                Data Cleaning
                       ↓
             Data Preprocessing
                       ↓
          Encode Categorical Data
                       ↓
                Feature Selection
                       ↓
              Train/Test Split
                       ↓
          Random Forest Regression
                       ↓
              Model Evaluation
                       ↓
          Interactive User Interface
                       ↓
             Demand Prediction
                       ↓
          Number of Plates Required

📈 Model Evaluation

The model is evaluated using:

1. Mean Absolute Error (MAE)

MAE represents the average difference between actual sales and predicted sales.

A lower MAE indicates better predictions.

2. Root Mean Squared Error (RMSE)

RMSE measures prediction error and gives more importance to larger errors.

A lower RMSE is generally better.

3. R² Score

R² indicates how well the model explains the variation in the sales data.

A value closer to 1 generally indicates better performance.

📊 Data Visualizations

The project generates visualizations such as:

Average Sales by Food Item

Shows which food items have higher average demand.

Average Sales by Weather

Shows how weather conditions affect food demand.

Feature Importance

Shows which input factors have the greatest influence on the model's predictions.

Actual vs Predicted Sales

Compares the model's predictions with the actual values in the test dataset.

🖥️ Interactive Prediction Interface

The project provides an interactive interface in Google Colab.

The user can select:

Day
Weather
Food Item
Price
Previous Sales
Exam Day
Weekend

and click:

🍔 PREDICT DEMAND

The model then displays the estimated number of plates that should be prepared.

▶️ How to Run the Project

Step 1: Open Google Colab

Create a new notebook in Google Colab.

Step 2: Upload the Dataset

Upload:

canteen_sales_dataset.csv

when the notebook asks for the file.

Step 3: Run the Code

Copy the complete project code into a Colab cell and run it.

Step 4: Wait for Model Training

The notebook will:

Load the dataset

Clean the data

Encode categorical variables

Split the data

Train the Random Forest model

Evaluate the model

Display graphs

Create the prediction interface

Step 5: Make a Prediction

Select the required values and click:

🍔 PREDICT DEMAND

The predicted number of plates will be displayed.

📁 Project Files

Canteen-Food-Demand-Predictor/
│
├── canteen_sales_dataset.csv
│
├── Canteen_Food_Demand_Predictor.ipynb
│
└── README.md

🌟 Advantages

Helps reduce food wastage.

Helps the canteen prepare the right quantity of food.

Easy to use.

Uses multiple demand-related factors.

Can be expanded with real-world data.

Beginner-friendly Machine Learning implementation.

Can be integrated into a web or mobile application.

⚠️ Limitations

The current dataset is synthetic.

Predictions may not represent real college demand.

Student attendance is not included.

Special college events are not included.

Holidays are not separately considered.

Sudden changes in demand may not be predicted accurately.

🚀 Future Scope

The project can be improved by adding:

1. Real Canteen Data

Replace the synthetic dataset with actual daily sales records.

2. Student Attendance

Use the expected number of students on campus to improve predictions.

3. Special Events

Consider festivals, college events, sports events, workshops, etc.

4. Holiday Detection

Automatically identify holidays and vacation periods.

5. Multiple Canteens

Predict demand separately for different college canteens.

6. Inventory Management

Connect predictions with ingredient inventory.

For example:

Predicted Samosa Demand = 120
↓
Calculate required potatoes
↓
Calculate required flour
↓
Calculate required oil
↓
Generate preparation plan

7. Web Application

The model can be deployed as a web application where canteen staff can enter the day's conditions and receive predictions.

8. Real-Time Dashboard

A dashboard could display:

Today's predicted demand

Actual sales

Food wastage

Most popular items

Weekly demand trends

Inventory requirements

🔐 Data Privacy

The current project uses synthetic data and therefore does not contain personal student information.

If real student or transaction data is used in the future, appropriate privacy and security measures should be implemented.

🎓 Academic Use

This project can be used as a:

Mini project

Machine Learning laboratory project

College assignment

Third-year engineering project

Portfolio/CV project

Demonstration of Regression and Random Forest

👩‍💻 Project Summary

Project Name: Canteen Food Demand Predictor

Domain: Machine Learning / Data Science

Problem Type: Regression

Algorithm: Random Forest Regression

Platform: Google Colab

Programming Language: Python

Dataset Size: 1,000 synthetic records

Main Output: Predicted number of food plates to prepare

📌 Conclusion

The Canteen Food Demand Predictor demonstrates how Machine Learning can be used to solve a practical college problem.

By analyzing factors such as day, weather, food price, previous sales, exam schedules, and weekends, the system estimates future food demand.

The project provides a foundation that can later be extended into a complete canteen management and inventory prediction system using real-world data.
