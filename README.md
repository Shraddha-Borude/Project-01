Healthcare Appointment No-Show Prediction

Objective

This project aims to predict whether a patient will miss a scheduled medical appointment. By leveraging machine learning and data visualization, the goal is to optimize appointment scheduling and reduce no-shows.

Tools Used

 Google Colab

Power BI


Dataset

The dataset contains information about 100k+ medical appointments in Brazil and whether or not patients showed up for their appointments. Key features include:

Patient demographics (age, gender)

Appointment details (scheduled date, appointment date, day of the week)

Communication (SMS reminders)

Medical history (hypertension, diabetes, alcoholism, etc.)

Target variable: No-show (Yes/No)


Project Steps

1. Data Preprocessing (Python)

Imported dataset using Pandas

Cleaned missing or inconsistent data

Converted dates to datetime format

Engineered features like DaysUntilAppointment, IsWeekend, etc.

Encoded categorical variables


2. Predictive Modeling

Split data into training and test sets

Trained a Decision Tree Classifier using Scikit-learn

Evaluated model using accuracy, precision, recall, and confusion matrix

Identified most important features influencing no-shows


3. Power BI Dashboard

Visualized key trends:

No-show rates by age group, weekday, and neighborhood

Impact of SMS reminders and waiting time

Gender-based appointment behavior


Interactive filters for deep exploration


4. Optimization Insights

SMS Effectiveness: SMS reminders slightly reduce no-shows

Age Factor: Younger patients (0–18) and elderly patients (70+) have higher no-show rates

Lead Time: Longer wait between scheduling and appointment increases no-show likelihood

Day of Week: Appointments early in the week have lower no-show rates


Deliverables

no_show_prediction.ipynb: Jupyter notebook with data cleaning and model training

no_show_dashboard.pbix: Power BI dashboard file

README.md: Project summary and documentation

Optimization Recommendations: Included in notebook and dashboard insights


How to Run

1. Clone this repository


2. Open no_show_prediction.ipynb in Jupyter/Colab


3. Install required libraries: pandas, sklearn, matplotlib, seaborn


4. Run the notebook cells step by step


5. Open Power BI and load the .pbix file for interactive insights



Conclusion

By identifying the patterns in no-show behavior, this project provides actionable insights to healthcare providers for reducing missed appointments and improving resource utilization.


