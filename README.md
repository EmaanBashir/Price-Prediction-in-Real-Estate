# Real Estate Price Prediction

## Project Overview

This project focuses on predicting real estate prices in Pakistan using data mining and machine learning techniques. By analyzing property characteristics and market trends, a data-driven approach is provided to assist buyers and sellers in making informed decisions.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Implementation](#project-implementation)
  - [Data Collection](#data-collection)
  - [Data Preprocessing](#data-preprocessing)
  - [Data Visualization](#data-visualization)
  - [Price Prediction](#price-prediction)
- [How to Run the Code](#how-to-run-the-code)
- [Results](#results)
- [Links](#links)

## Introduction

The real estate market in Pakistan is subject to various economic and local factors that influence property prices. This project collects and analyzes real estate data to develop a predictive model using machine learning techniques. The project involves data collection through web scraping, data preprocessing, visualization, and model training for price prediction.

## Dataset

The dataset used for this project was collected from [Zameen.com](https://www.zameen.com/) and consists of **280,046 properties** from **189 cities** in Pakistan. It includes details such as:

- Property type (House, Flat, Plot, Office, etc.)
- Location (City, Province)
- Price
- Number of bedrooms and bathrooms
- Area size
- Purpose (For Sale, For Rent)
- Date added

The dataset is available [here](https://drive.google.com/drive/folders/1X7_zt9ZvbBDPhCFCiiodzy5waXKcwqrZ?usp=share_link).

## Project Implementation

### Data Collection

Data was collected using web scraping techniques with **BeautifulSoup**. The process involved:

1. Parsing the property listings from **Zameen.com**.
2. Extracting relevant details for each property.
3. Storing the data in a structured **CSV format**.

### Data Preprocessing

The collected data was cleaned using **Pandas** and **NumPy** by:

- Extracting numerical values from price strings.
- Converting area measurements into square feet.
- Handling missing values through imputation and removal.
- Removing outliers based on price and area.
- Standardizing property type labels.

### Data Visualization

**Tableau** was used to visualize patterns in the dataset. Key insights include:

- **Price Trends Over the Years**: Line charts showing average property prices across years.
  
  ![image](https://github.com/user-attachments/assets/f3a9d14f-dc25-47b7-bf02-cfea8ef1f7a7)
- **Property Type Distribution**: Pie charts displaying the distribution of different property types.
  
  ![image](https://github.com/user-attachments/assets/9b0e8007-3051-466c-aa7a-7c82885e8626)
- **Average Property Prices by Province**: Map charts showing regional price variations.
  
  ![image](https://github.com/user-attachments/assets/1b1eb1b3-bf84-46dc-9e4b-4f16ff9926a5)
- **Price Range Distribution**: Histograms plotting the number of properties in different price ranges.
  
  ![image](https://github.com/user-attachments/assets/38635772-6b29-4694-91bc-e7ca2084b88f)
- **Property Type vs Yearly Price Trends**: Heatmaps illustrating yearly price changes for different property types.
  
  ![image](https://github.com/user-attachments/assets/a14102c7-20b5-483d-8c3e-edf744f85045)

Interactive visualizations can be explored in the [Tableau Dashboard](https://public.tableau.com/views/RealEstate_16720671945070/Dashboard1?language=en-US&display_count=n&origin=viz_share_link).

### Price Prediction

For predicting property prices, a **Decision Tree Regression model** was trained using **scikit-learn**. The model was evaluated using two different criteria:

1. **Mean Squared Error (MSE)** – Achieved **72.2% accuracy**.
2. **Friedman MSE** – Achieved **70.38% accuracy**.

## How to Run the Code

1. Clone this repository:
   ```bash
   git clone https://github.com/EmaanBashir/Price-Prediction-in-Real-Estate.git
   cd Price-Prediction-in-Real-Estate/Code
   ```
2. Run the web scraping script to collect data:
   ```bash
   jupyter notebook Web_Scraping_for_Real_Estate_Data.ipynb
   ```
3. Run the data preprocessing script:
   ```bash
   jupyter notebook Data_Preprocessing.ipynb
   ```
4. Train the price prediction model:
   ```bash
   jupyter notebook Price_Prediction.ipynb
   ```
5. View the results and visualizations in the Tableau dashboard.

## Results

Below are some key findings from the analysis:

- **Houses in major cities like Karachi, Lahore, and Islamabad tend to have higher prices.**
- **Property prices have shown an increasing trend over the past few years.**
- **Commercial properties tend to have a higher price per square foot compared to residential properties.**
- **The Decision Tree Regression model provided a reasonable accuracy of over 70%.**

## Links

- 📂 **Dataset**: [Google Drive](https://drive.google.com/drive/folders/1X7_zt9ZvbBDPhCFCiiodzy5waXKcwqrZ?usp=share_link)
- 📊 **Presentation**: [Canva](https://www.canva.com/design/DAFWDrfHGyA/sL_ZZprUQ_sg_YcBvnnbdw/edit?utm_content=DAFWDrfHGyA\&utm_campaign=designshare\&utm_medium=link2\&utm_source=sharebutton)
- 📈 **Dashboard**: [Tableau](https://public.tableau.com/views/RealEstate_16720671945070/Dashboard1?language=en-US&display_count=n&origin=viz_share_link)


