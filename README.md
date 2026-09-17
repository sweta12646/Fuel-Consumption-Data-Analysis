🚗 Fuel Consumption Data Analysis Using Python

📌 Project Overview

This project analyzes vehicle fuel consumption and CO₂ emissions using Python. The analysis explores vehicle characteristics, fuel types, engine size, cylinders, city and highway fuel consumption, combined fuel consumption, and their relationships with CO₂ emissions.

The project uses Pandas, NumPy, Matplotlib, and Seaborn for data manipulation, analysis, and visualization.

---

🎯 Project Objective

The main objectives of this project are to:

- Understand vehicle characteristics.
- Analyze different fuel types.
- Analyze engine size and number of cylinders.
- Study city fuel consumption.
- Study highway fuel consumption.
- Analyze combined fuel consumption.
- Analyze CO₂ emissions.
- Identify relationships between vehicle specifications, fuel consumption, and emissions.

---

🛠️ Technologies & Libraries Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization

---

📂 Dataset

The dataset contains 1,067 vehicle records and 13 columns.

Dataset Columns

Column| Description
"MODELYEAR"| Vehicle model year
"MAKE"| Vehicle manufacturer
"MODEL"| Vehicle model
"VEHICLECLASS"| Vehicle category/class
"ENGINESIZE"| Engine size
"CYLINDERS"| Number of cylinders
"TRANSMISSION"| Transmission type
"FUELTYPE"| Fuel type
"FUELCONSUMPTION_CITY"| City fuel consumption
"FUELCONSUMPTION_HWY"| Highway fuel consumption
"FUELCONSUMPTION_COMB"| Combined fuel consumption
"FUELCONSUMPTION_COMB_MPG"| Combined fuel consumption in MPG
"CO2EMISSIONS"| CO₂ emissions

---

🔍 Data Quality Checks

The project performs several data-quality checks:

Dataset Dimensions

df.shape

Output:

(1067, 13)

Missing Values

df.isnull().sum()

The analysis shows 0 missing values across all 13 columns.

Duplicate Records

df.duplicated().sum()

Output:

0

No duplicate records were found in the dataset.

---

📊 Analysis Performed

1. Vehicle Manufacturer Analysis

The dataset contains 39 unique vehicle manufacturers.

The manufacturers with the highest number of vehicle records include:

- Ford
- Chevrolet
- BMW
- Mercedes-Benz
- GMC
- Audi
- Toyota
- Porsche
- Volkswagen
- Dodge

This represents the composition of this particular dataset and should not be interpreted as overall automobile market share.

---

2. Fuel Type Analysis

The dataset contains four fuel types:

Fuel Type| Records
X| 514
Z| 434
E| 92
D| 27

---

3. Vehicle Class Analysis

The project analyzes the distribution of different vehicle classes, including:

- Mid-size
- Compact
- SUV
- Full-size
- Two-seater
- Subcompact
- Pickup truck
- Station wagon
- Van
- Minivan
- Special purpose vehicle

The dataset is not evenly distributed across all vehicle categories.

---

4. Engine Size Analysis

A histogram is used to understand the distribution of engine sizes.

sns.histplot(
    data=df,
    x="ENGINESIZE",
    bins=20,
    kde=True
)

The analysis shows that most vehicles are concentrated within a particular range of engine sizes, while very small or very large engine sizes occur less frequently.

---

5. Cylinder Analysis

The number of cylinders represented in the dataset includes:

Cylinders| Vehicles
3| 4
4| 420
5| 9
6| 356
8| 252
10| 9
12| 17

---

⛽ Fuel Consumption Analysis

City Fuel Consumption

The city fuel consumption ranges from 4.6 to 30.2 L/100 km, with an average of approximately 13.30 L/100 km.

Highway Fuel Consumption

Highway fuel consumption ranges from 4.9 to 20.5 L/100 km, with an average of approximately 9.47 L/100 km.

Combined Fuel Consumption

Combined fuel consumption ranges from 4.7 to 25.8 L/100 km, with an average of approximately 11.58 L/100 km.

---

📈 Relationship Analysis

City vs Highway Fuel Consumption

A scatter plot is used to compare city and highway fuel consumption.

The analysis shows a positive relationship: vehicles with higher city fuel consumption generally also have higher highway fuel consumption.

Engine Size vs Fuel Consumption

The analysis generally indicates a positive relationship between engine size and combined fuel consumption. Vehicles with larger engines tend to have higher fuel consumption in this dataset.

Engine Size vs CO₂ Emissions

The analysis generally shows a positive relationship between engine size and CO₂ emissions.

Fuel Consumption vs CO₂ Emissions

A strong positive relationship is observed between combined fuel consumption and CO₂ emissions. Vehicles with higher fuel consumption generally produce higher CO₂ emissions.

---

🔥 Correlation Analysis

The project uses correlation analysis to measure linear relationships between numerical variables.

Some important correlations include:

Variables| Correlation
Engine Size & CO₂ Emissions| 0.874
Cylinders & CO₂ Emissions| 0.850
City Consumption & CO₂ Emissions| 0.898
Highway Consumption & CO₂ Emissions| 0.862
Combined Consumption & CO₂ Emissions| 0.892
Combined MPG & CO₂ Emissions| -0.906

Important: Correlation indicates association, not causation.

---

🚙 Average CO₂ Emissions by Vehicle Class

The project calculates average CO₂ emissions for each vehicle class.

Some values from the analysis are:

Vehicle Class| Average CO₂ Emissions
Compact| 216.72
Mid-size| 226.48
SUV - Small| 242.69
Full-size| 267.65
SUV - Standard| 307.67
Pickup Truck - Standard| 309.10
Van - Cargo| 361.50
Van - Passenger| 401.00

---

📊 Visualizations

The project includes the following visualizations:

1. Top 10 Vehicle Manufacturers
2. Distribution of Fuel Types
3. Vehicle Class Distribution
4. Distribution of Engine Size
5. Distribution of Number of Cylinders
6. City Fuel Consumption Distribution
7. Highway Fuel Consumption Distribution
8. City vs Highway Fuel Consumption
9. Combined Fuel Consumption Distribution
10. Engine Size vs Combined Fuel Consumption
11. Engine Size vs CO₂ Emissions
12. Combined Fuel Consumption vs CO₂ Emissions
13. Correlation Heatmap
14. Average CO₂ Emissions by Vehicle Class

---

📁 Project Structure

Fuel-Consumption-Data-Analysis/
│
├── FuelConsumption.csv
├── FuelConsumption_Analysis.ipynb
├── README.md
└── visualizations/

«Update the filenames above if your actual GitHub files use different names.»

---

▶️ How to Run the Project

1. Clone the Repository

git clone <your-github-repository-url>

2. Navigate to the Project Folder

cd Fuel-Consumption-Data-Analysis

3. Install Required Libraries

pip install pandas numpy matplotlib seaborn jupyter

4. Run the Jupyter Notebook

jupyter notebook

Open the project notebook and run the cells.

---

💡 Key Insights

- The dataset contains 1,067 vehicle records and 13 variables.
- There are 39 unique manufacturers.
- The dataset contains four fuel types: X, Z, E, and D.
- City fuel consumption is generally higher than highway fuel consumption.
- Engine size is positively associated with combined fuel consumption.
- Engine size and cylinder count are associated with CO₂ emissions.
- Combined fuel consumption has a strong positive relationship with CO₂ emissions.
- Combined MPG has a strong negative relationship with CO₂ emissions.
- CO₂ emissions vary across different vehicle classes.
- Correlation represents association and does not establish causation.

---

🏁 Conclusion

The Fuel Consumption dataset was analyzed using Python, Pandas, NumPy, Matplotlib, and Seaborn.

The analysis demonstrates relationships between engine size, cylinders, vehicle class, fuel consumption, and CO₂ emissions. Vehicles with higher fuel consumption generally produce higher CO₂ emissions, while different vehicle classes show differences in their average CO₂ emissions.

Overall, the project provides an understanding of vehicle fuel consumption patterns and their relationship with environmental impact.

---

👤 Author

Swetalina Stitapragyan Sahoo

📌 Skills Demonstrated

- Python
- Pandas
- NumPy
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Analysis
- Correlation Analysis
- Seaborn
- Matplotlib

---

⭐ If you find this project useful, consider giving the repository a star!
