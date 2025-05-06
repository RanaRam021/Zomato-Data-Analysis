# 🍽️ Zomato Data Analysis Project

This project performs an in-depth exploratory data analysis (EDA) on the Zomato restaurant dataset. The aim is to uncover trends, understand customer behavior, and derive actionable insights regarding restaurants, their services, and performance based on rating, cost, and type.

---

## 📁 Project Structure

- zomato-data-analysis 
  - ├── Zomato Dataset.zip # Compressed dataset
  - ├── Zomato_Data_Analysis.ipynb # Full code with data cleaning, preprocessing, EDA, and visualizations
  - └── README.md # Project documentation


---

## 🎯 Objectives

- Clean and preprocess the Zomato dataset
- Perform exploratory data analysis (EDA)
- Visualize important insights about restaurants in terms of:
  - Online ordering and reservation
  - Cost distribution
  - Rating analysis
  - Restaurant types and locations

---

## 🧰 Technologies Used

- **Language**: Python
- **Libraries**:
  - `pandas` – data manipulation
  - `matplotlib` – visualizations
  - `seaborn` – enhanced statistical plots

---

## 📊 Data Preprocessing Steps

- Removed unnecessary columns (`url`, `phone`, `menu_item`, etc.)
- Renamed columns for clarity (e.g., `rate` → `rating`, `approx_cost(for two people)` → `cost_for_two`)
- Cleaned `rating` by:
  - Removing `'NEW'` and `'-'` entries
  - Converting ratings to float
  - Filling missing values with mean
- Cleaned `cost_for_two` by:
  - Removing commas
  - Converting to numeric
  - Filling missing values with mean
- Handled missing values in `rest_type` by replacing them with `'Other'`
- Added a new column `rating_categories` with bins:
  - Poor: 1–2
  - Unsatisfactory: 2–3
  - Satisfactory: 3–4
  - Outstanding: 4–5

---

## 📈 Visualizations

- **Pie Charts**:
  - Online order availability
  - Table reservation options
  - Rating categories
  - Types of services

- **Bar Charts**:
  - Top 10 restaurant names by number of outlets
  - Average cost for top 10 restaurants
  - Average rating of top restaurants
  - Top 10 locations by restaurant count, rating, and cost

- **Box Plot**:
  - Rating distribution across restaurant types

- **Scatter Plot**:
  - Restaurant rating distribution by location

---

## 🔍 Key Insights

- A large number of restaurants provide **online delivery**, while fewer offer **table reservations**.
- **Quick Bites** and **Casual Dining** are the most common service types.
- Popular restaurants are not always the highest-rated or most expensive.
- Certain locations like **BTM**, **Indiranagar**, and **Koramangala** dominate in terms of restaurant availability and variety.
- Locations like **Church Street** have restaurants with relatively higher average ratings and costs.

---

## 📦 Dataset

- Source: Zomato Bangalore Restaurant Dataset
- Cleaned and compressed version: `Zomato Dataset.zip`
- The full project, including preprocessing and visualizations, is included in the notebook/script.

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/RanaRam021/Zomato-Data-Analysis.git
   cd zomato-data-analysis

2. Unzip the compressed files if needed::
   ```bash
   unzip Zomato Dataset.zip

3. Open the Jupyter Notebook or run the Python script::
   ```bash
   jupyter notebook Zomato_Data_Analysis.ipynb


## ⭐ Acknowledgment

This project is part of a data science learning initiative, inspired by the need to explore real-world data and uncover insights using Python and visualization tools.

