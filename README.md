# Toyota Used Car Sales Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MattPollockUK/Toyota-Dataset-for-used-cars/blob/main/notebooks/toyotadataset.ipynb)

**Author:** Matt Pollock  
**Date:** September 2025  

## Project Overview
Exploratory data analysis of **used Toyota car sales in the UK**, with a focus on **hybrid vehicles**.  
The goal is to understand trends, compare hybrid vs non-hybrid cars, and provide insights to support sales and marketing decisions.

---

## Project Goals
- Clean and validate the dataset  
- Explore trends in used car sales  
- Calculate business metrics such as **Hybrid Share of Sales**  
- Compare hybrid vs non-hybrid vehicles  

---

## Dataset
- Source: `toyota.csv`  
- Key columns:
  - `model` – Toyota car model  
  - `year` – Year of manufacture  
  - `price` – Sale price (£)  
  - `mileage` – Miles on odometer  
  - `fuelType` – Petrol, Diesel, Hybrid, Other  
  - `tax` – Road tax (£)  
  - `mpg` – Miles per gallon  
  - `engineSize` – Engine displacement  

**Data Cleaning Steps:**
- Removed invalid engine sizes (`engineSize == 0`)  
- Dropped missing values  
- Standardized model names (capitalization & spacing)  
- Reset index  

---

## Key Findings
- **Hybrid vehicles** account for ~30% of used Toyota sales  
- Hybrids generally have:
  - Lower mileage  
  - Better fuel efficiency (MPG)  
  - Lower tax (£0 vs £135)  
  - Higher average price (£13,400 vs £10,800)  
- Recommendations:
  - Promote hybrids for fuel economy and tax benefits  
  - Increase stock of mid-priced hybrid models  
  - Track Hybrid Share of Sales monthly  

---

## Visualizations
- Fuel type distribution (bar chart)  
- Price distribution (histogram)  
- Hybrid vs Other comparison (median price, mileage, MPG, tax)  
- Hybrid Share of Sales (pie chart)  

---

## How to Run
```bash
# Install dependencies
pip install -r requirements.txt

# Open notebook
jupyter notebook notebooks/toyotadataset.ipynb

Toyota-Dataset-for-used-cars/
├── notebooks/
│   └── toyotadataset.ipynb
├── README.md
├── requirements.txt
└── LICENSE

Tools & libraries
Python 3.x
Pandas
Matplotlib
Jupyter/Google Colab

This project is licensed under the MIT License.
