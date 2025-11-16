# energy-efficiency-dataset
Source: UCI Machine Learning Repository, “Energy Efficiency” dataset (https://archive.ics.uci.edu/dataset/242/energy+efficiency)
Number of Observations (Instances): 768 different building configurations.
Input Features: 8 variables (X1–X8).
Target Variables: Heating Load (Y1) and Cooling Load (Y2).
Task: Regression (continuous value estimation). It can also be used as a classification (multiclass) problem if Y1 and Y2 are rounded to integers.

Variable Meaning / Description Unit of Measurement / Note
X1 – Relative Compactness / The building's compactness ratio (volume / surface relationship) / (non-unit, ratio)
X2 – Surface Area / The building's exterior surface area / m²
X3 – Wall Area / Exterior wall area / m²
X4 – Roof Area / Roof area / m²
X5 – Overall Height / Building height / meters
X6 – Orientation / Building direction (geometric configuration) / Integer (2 = North, 3 = East, 4 = South, 5 = West)
X7 – Glazing Area: Glazed (glass) area ratio. Ratio/proportional value (e.g., 0.00, 0.10, 0.25, 0.40).
X8 – Glazing Area Distribution / Glazing area distribution / Categorical integer (e.g., 0 = Uniform, other values ​​are directional).
Y1 – Heating Load / Energy load required for heating / kWh/m² (simulation result).
Y2 – Cooling Load / Energy load required for cooling / kWh/m² (simulation result).

Data Generation & Simulation Information:
The data was generated using Ecotect simulation software, based on 12 different building geometries.
These 12 shapes were simulated with various parameters such as glazing area, glazing distribution, and orientation, resulting in a total of 768 different building versions.
Heating and cooling loads were calculated for each building.

Usage Notes & Data Analysis:
There are no missing values: complete data are provided for all 768 observations.
The Orientation and Glazing Area Distribution variables can be defined categorically:
Values ​​for Orientation: 2 = North, 3 = East, 4 = South, 5 = West.
For Glazing Area Distribution, simulation studies include different distribution types.
This dataset is suitable for both multivariate regression models and categorical classification.


Data Processing Steps on Project
The raw Excel file (ENB2012_data.xlsx) was loaded without modification.
Column names were automatically detected to ensure compatibility with different dataset versions.
The 8 input features were normalized to floating-point format; no rows were removed or altered.
