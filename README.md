# 🚀 Exploring Space Missions and Discoveries: A Data-driven Story from NASA's Archives

## 🛰️ Project Overview

This project explores NASA’s rich archive of space missions, exoplanet discoveries, and celestial observations through a data-driven lens. With a focus on storytelling and analysis, the project showcases how historical and recent mission data can reveal patterns in launch frequency, technology trends, and astronomical findings.

By integrating tools from Python, Excel, SQL, and Tableau, we aim to bring insights to life and inspire curiosity about our universe.

---

## 🎯 Goal

To demonstrate proficiency in data collection, wrangling, querying, analysis, and visualization across the Python, GENDATA, and PYDATA modules by working on a real-world dataset related to outer space and NASA.

---

## 🔍 Problem Statement
“Despite decades of space exploration, we still struggle to answer questions like: Which missions yield the most discoveries for the cost? How have political shifts and private companies changed mission outcomes? What trends can we predict for the future of space exploration?”



---

## 🧰 Tools & Technologies Used

| Tool          | Purpose |
|---------------|---------|
| **Python**    | Used NASA APIs to collect mission and discovery data |
| **Excel**     | Performed initial data cleaning and formatting |
| **SQL**       | Stored cleaned dataset and performed analytical queries |
| **Tableau**   | Built an interactive dashboard to visualize mission trends |
| **Pandas** | Data wrangling and numeric analysis |
| **Matplotlib** | Created 3+ static EDA charts |
| **Plotly**    | Built an interactive visualization |
| **Jupyter Notebook** | Used for all code and analysis steps |

---

## 📂 Project Structure
📁 Exploring-Space-Missions-NASA
├── data_collection/           
│   └── nasa_data_collector.ipynb   # Pulls exoplanet data from NASA API
├── excel_cleaning/             
│   ├── raw_exoplanets.csv          # Raw data fetched from API
│   └── cleaned_nasa_data.xlsx      # Cleaned dataset
├── sql/                        
│   ├── nasa_database.sql
│   └── sql_queries_results.md
├── eda_visuals/                
│   └── space_missions_eda.ipynb
├── tableau/                    
│   ├── tableau_dashboard_screenshot.png
│   └── tableau_dashboard_link.txt
├── presentation/               
│   └── final_presentation.pdf
├── data_dictionary.md          
├── requirements.txt            
└── README.md
# 🧹 Excel Cleaning Report (Step 2)

This folder contains the **Excel-cleaned datasets** for the project *Exploring Space Missions and Discoveries: A Data-driven Story from NASA's Archives*.

---

## 🔍 Purpose
While the Python scripts in **Step 1** already fetched and structured the datasets from NASA APIs, this step demonstrates **manual inspection and cleaning in Microsoft Excel**, as required by the project guidelines.

The goal was to:
- Check for missing values
- Standardize formats (dates, numbers, categories)
- Remove duplicates
- Validate column names
- Save a final "Excel-verified" dataset for use in SQL and Tableau

---

## 📑 Files in this Folder
- `raw_missions.csv` → Direct output from Launch Library API (before Excel cleaning)  
- `raw_exoplanets.csv` → Direct output from NASA Exoplanet Archive (before Excel cleaning)  
- `cleaned_nasa_data.xlsx` → Cleaned automatically by Python (Step 1 result)  
- `cleaned_nasa_data_v2.xlsx` → Final manually verified dataset after Excel inspection (Step 2 result)  

---

## 📝 Cleaning Steps in Excel

### 1. Missions Sheet
- Standardized column names:  
  - `vehicle` → `launch_vehicle`  
  - `agency` → `launch_agency`
- Converted `launch_date` to proper **Date** format.  
- Checked for **missing values** in `latitude` / `longitude`.  
- Removed duplicates on `mission_name + launch_date`.  

### 2. Discoveries Sheet
- Ensured `discovery_year` is numeric.  
- Checked for blanks in `planet_radius_earth`, `planet_mass_earth`, `orbital_period_days`.  
- Converted columns to **numeric types** where needed.  
- Cleaned categorical values in `discovery_method` (removed trailing spaces).  
- Validated RA/Dec as `longitude` and `latitude` for mapping.  

---

## ✅ Outcome
The final file `cleaned_nasa_data_v2.xlsx` is now:
- Structured
- Free of duplicates
- With standardized formats
- Ready for **Step 3: SQL Storage and Querying**

## Website link
-https://sites.google.com/view/exploringspacemissionsanddisco/discoveries-and-mission-success?read_current=1


