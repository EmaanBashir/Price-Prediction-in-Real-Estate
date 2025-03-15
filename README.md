# Real Estate Price Prediction

## Project Overview

This project focuses on predicting real estate prices in Pakistan using data mining and machine learning techniques. By analyzing property characteristics and market trends, we aim to provide a data-driven approach to assist buyers and sellers in making informed decisions.

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
- [Contributors](#contributors)

## Introduction

The real estate market in Pakistan is subject to various economic and local factors that influence property prices. Our project collects and analyzes real estate data to develop a predictive model using machine learning techniques. The project involves data collection through web scraping, data preprocessing, visualization, and model training for price prediction.

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

We used **Tableau** to visualize patterns in the dataset. Key insights include:

- **Price Trends Over the Years**: Line charts showing average property prices across years.
- **Property Type Distribution**: Pie charts displaying the distribution of different property types.
- **Average Property Prices by Province**: Map charts showing regional price variations.
- **Price Range Distribution**: Histograms plotting the number of properties in different price ranges.
- **Property Type vs Yearly Price Trends**: Heatmaps illustrating yearly price changes for different property types.

Interactive visualizations can be explored in the [Tableau Dashboard](https://public.tableau.com/views/RealEstate_16720671945070/Dashboard1?\:language=en-US&\:display_count=n&\:origin=viz_share_link).

### Price Prediction

For predicting property prices, we trained a **Decision Tree Regression model** using **scikit-learn**. The model was evaluated using two different criteria:

1. **Mean Squared Error (MSE)** – Achieved **72.2% accuracy**.
2. **Friedman MSE** – Achieved **70.38% accuracy**.

## How to Run the Code

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/real-estate-price-prediction.git
   cd real-estate-price-prediction
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
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

Below are some key findings from our analysis:

- **Houses in major cities like Karachi, Lahore, and Islamabad tend to have higher prices.**
- **Property prices have shown an increasing trend over the past few years.**
- **Commercial properties tend to have a higher price per square foot compared to residential properties.**
- **The Decision Tree Regression model provided a reasonable accuracy of over 70%.**

## Links

- 📂 **Dataset**: [Google Drive](https://drive.google.com/drive/folders/1X7_zt9ZvbBDPhCFCiiodzy5waXKcwqrZ?usp=share_link)
- 📊 **Presentation**: [Canva](https://www.canva.com/design/DAFWDrfHGyA/sL_ZZprUQ_sg_YcBvnnbdw/edit?utm_content=DAFWDrfHGyA\&utm_campaign=designshare\&utm_medium=link2\&utm_source=sharebutton)
- 📈 **Dashboard**: [Tableau](https://public.tableau.com/views/RealEstate_16720671945070/Dashboard1?\:language=en-US&\:display_count=n&\:origin=viz_share_link)

## Contributors

This project was completed as part of the **MSc Data Science** coursework by:

- **Arooba Siddiqi**
- **Emaan Bashir**
- **Rimsha Mirza**
- **Faraz Shah**

---

For any inquiries or contributions, feel free to open an issue or contact us!

