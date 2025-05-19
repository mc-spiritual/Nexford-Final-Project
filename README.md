# Nexford-Final-Project

# 💼 Healthcare Income & Spending Survey App

This is a data collection and analysis tool built with **Flask**, **MongoDB**, and **Python**, designed for a data analysis company in Washington, DC. The aim is to collect survey data on income and expenses in preparation for launching a new product in the healthcare industry.

## 🚀 Project Overview

This web-based survey tool allows users to:
- Enter their **Age**, **Gender**, **Total Income**, and specific **Expense categories such as Utilities, Shopping, School Fees, Health**
- Store the data in **MongoDB Atlas**
- Process and export the data to **CSV**
- Visualize key insights such as:
  - Income trends by age
  - Gender-based spending habits across categories

---

## 🛠 Tech Stack

- **Flask** — Python Web Framework
- **MongoDB Atlas** — Cloud-based NoSQL database
- **Pandas** — For data handling and export
- **Matplotlib / Seaborn** — For visualization
- **Jupyter Notebook** — For data analysis and chart generation
- **Gunicorn** — Production WSGI server for deployment
- **Render** — Deployment platform

---

## 📁 Project Structure

project/

│

├── app.py # Flask application file

├── templates/

│ └── index.html # HTML form for user data input

├── export_data # Contains a class User to import the data from Mongodb Local server 

├── requirements.txt # Python dependencies

├── Procfile # Deployment instruction for Render

├── user_data.csv # Exported survey data

└── analysis.ipynb # Jupyter notebook with data visualization

## 📊 How to Analyze the Data

Once users submit data, the app stores it in MongoDB and exports it to user_data.csv.

Open analysis.ipynb in Jupyter Notebook.

Run the notebook to generate:

Bar chart of ages with the highest income

Gender-based spending across categories

Export the charts for use in your PowerPoint client presentation.


## 🌍 Deployment (Render)

Connect your GitHub repo to Render

Add a Web Service with:

Start Command: gunicorn app:app

Environment Variable: MONGODB_URI=your_connection_string

Wait for the build and deploy. Done!

## Limitation of the project
This project uses Mongodb Local server because of the cost of using the Mongo Atlas webserver which happens to be a paid service. Hence the deployment of the web in Render would not be efficient.
