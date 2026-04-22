# PYTHON-PROJECT
Student Analytics Dashboard (Python + Pandas)
 Project Overview

This project is an interactive data analytics dashboard built using Python, Pandas, and Matplotlib.
It analyzes a tutoring institute database containing students, enrollments, payments, courses, and attendance data.

The goal is to generate business insights such as revenue trends, top-performing courses, and student activity.

 Tools & Technologies
Python 
Pandas
Matplotlib
Jupyter Notebook / Google Colab
ipywidgets (for interactivity)
 Dataset Structure

The dataset contains multiple Excel sheets:

Students
Teachers
Courses
Batches
Enrollments
Payments
Attendance
 Data Processing Workflow

The analysis is built using relational joins:

df = payments.merge(enrollments, on='enroll_id') \
             .merge(batches, on='batch_id') \
             .merge(courses, on='course_id')
 Key Features
 Revenue Analysis
Total revenue calculation
Revenue by course
Monthly revenue trends
 Student Analytics
Top paying students
Student enrollment patterns
 Course Performance
Best performing courses by revenue
Course-wise student distribution

 Interactive Dashboard
<img width="1220" height="753" alt="Screenshot 2026-04-22 183937" src="https://github.com/user-attachments/assets/4f37dd26-0cca-40f8-a325-14b58181d1f0" />

 
Filter by course
Dynamic KPI updates
Real-time charts
 Dashboard Preview


 How to Run
pip install pandas matplotlib ipywidgets openpyxl

Then open:

notebooks/analysis_dashboard.ipynb

Run all cells.

 Key Insights
Identified top revenue-generating courses
Found high-value students based on payments
Analyzed attendance patterns
Built interactive filtering dashboard
Future Improvements
Add Streamlit web app version
Add predictive analytics (student dropout prediction)
Connect to SQL database instead of Excel


Your Name
Data Analyst Portfolio Project
