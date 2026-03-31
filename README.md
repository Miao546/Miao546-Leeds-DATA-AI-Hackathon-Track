# Miao546-Leeds-DATA-AI-Hackathon-Track

# 🌍 Global CO2 Emissions & Economic Growth Decoupling Analysis

This project analyzes the relationship between carbon dioxide (CO2) emissions, Gross Domestic Product (GDP), and population changes across different countries from 1980 to 2023. Through data cleaning and interactive visualizations, this project highlights the phenomenon of "Decoupling"—where an economy continues to grow while its carbon emissions stabilize or decline.

This repository contains three core Jupyter Notebooks responsible for data cleaning, generating a decoupling bubble chart, and creating a dynamic bar chart race.

---

## 🛠️ 1. Dependencies

To run the code in this project, you need to have Python 3.x installed along with the following data processing and visualization libraries.

---

## 📂 2. Data Setup

Before running the code, ensure your project directory is structured correctly. The scripts will automatically create the output folders, but you must prepare the raw data beforehand.

1. Ensure there is a folder named `Data/` in your root directory.
2. Place the following raw CSV files directly into the `Data/` folder:
   * `population-population-people-in-thousands.csv` (Population Data)
   * `co2-emissions-emissions-mmtco2.csv` (CO2 Emissions Data)
   * `gross-domestic-product-gdp-billion-dollars-at-purchasing-power-parities.csv` (GDP Data)

**Your initial directory structure should look like this:**

```text
.
├── Bubble_Chart_Decoupling.ipynb
├── Ultimate_Bar_Chart_Race.ipynb
├── Clean Data.ipynb
├── Output/
│   ├── Global_CO2_Decoupling_Analysis.html
│   └── Global_CO2_Ranking_Race.html
└── Data/
    ├── population-population-people-in-thousands.csv
    ├── co2-emissions-emissions-mmtco2.csv
    ├── gross-domestic-product-gdp-billion-dollars-at-purchasing-power-parities.csv
    └── Cleaned/
        ├── cleaned_gdp_data_1980_2023.csv
        ├── Master_CO2_Decoupling_Final.csv
        ├── cleaned_pop_data_1980_2023.csv
        └── cleaned_co2_data_1980_2023.csv
```

---

## 🚀 3. How to Run

Since the visualization charts depend on the cleaned master dataset, **please run the Notebooks strictly in the following order.**

You can start your environment by typing `jupyter notebook` in your terminal, then open and run the files sequentially:

### Step 1: Data Cleaning and Merging
Open and run all cells in **`Clean Data.ipynb`**.
* **Function:** Loads raw data, handles missing values, standardizes formats, and merges the three datasets by country and year.
* **Expected Output:** The script will automatically create a `Data/Cleaned/` folder, save the intermediate cleaned data, and generate the final comprehensive table `Master_CO2_Decoupling_Final.csv`.

### Step 2: Generate Decoupling Bubble Chart
Open and run all cells in **`Bubble_Chart_Decoupling.ipynb`**.
* **Function:** Reads `Master_CO2_Decoupling_Final.csv` and uses Plotly to build an interactive bubble chart illustrating the relationship between GDP and CO2 emissions per capita.
* **Expected Output:** The script will automatically create an `Output/` folder and generate the interactive HTML file `Global_CO2_Decoupling_Analysis.html`.

### Step 3: Generate Global CO2 Emissions Ranking Race
Open and run all cells in **`Ultimate_Bar_Chart_Race.ipynb`**.
* **Function:** Reads the master data table to generate a smooth, dynamic bar chart race of total emissions by country from 1980 to 2023.
* **Expected Output:** Generates the interactive HTML file `Global_CO2_Ranking_Race.html` in the `Output/` folder.

---

## 🎯 4. Viewing the Results
After running all the code above, you can directly double-click the `.html` files in the `Output/` folder to open them in your web browser. You will be able to interact with the high-quality charts (e.g., hover for exact values, play the timeline animation, etc.).
## 📂 Project Structure
The project is organized into a clean, professional directory:


