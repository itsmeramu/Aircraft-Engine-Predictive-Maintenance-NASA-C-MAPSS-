# Aircraft-Engine-Predictive-Maintenance-NASA-C-MAPSS-
# Introduction
An aerospace data analytics project using NASA C-MAPSS turbofan engine data to study engine health, sensor behavior, and degradation through Excel, Python/Pandas, SQL, and Power BI, with machine learning planned as the final phase.

## Project Overview

This project is an end-to-end aircraft engine predictive maintenance project using the NASA C-MAPSS FD001 turbofan engine degradation dataset.

The project focuses on understanding, cleaning, analyzing, and visualizing aircraft engine sensor data before developing machine learning models.

The complete workflow is:

Raw Data → Excel → Python/Pandas → SQL → Power BI → Machine Learning

Machine learning is intentionally being kept as the final stage. The current priority is to build a strong foundation in data cleaning, exploratory analysis, SQL, and dashboard development.

## Why This Project?

Aircraft engines operate under demanding conditions, and their performance changes as they accumulate operating cycles. Monitoring parameters such as temperature, pressure, rotational speed, fuel-related measurements, and other engine variables can provide valuable information about engine operating condition and degradation.

This project uses NASA's C-MAPSS dataset because it provides a structured aerospace-engine dataset suitable for studying engine health and predictive maintenance.

Rather than immediately training machine learning models, the project follows the complete data analytics workflow.

The approach is:

Understand the data
→ Clean the data
→ Analyze the data
→ Query the data
→ Visualize the data
→ Extract engineering insights
→ Develop machine learning models

## Dataset

The project uses the NASA Commercial Modular Aero-Propulsion System Simulation (C-MAPSS) Turbofan Engine Degradation Simulation dataset.

The initial focus is FD001.

FD001 contains:

- 100 simulated engine units
- 20,631 training observations
- 26 columns
- 3 operational settings
- 21 sensor measurements
- 1 operating condition
- 1 simulated fault mode: High-Pressure Compressor (HPC) degradation

The training trajectories continue until simulated failure.

The Unit_Number identifies an individual simulated engine within the dataset. These are not real aircraft registrations or real-world engine serial numbers.

## Phase 1 — Excel

The first stage focuses on understanding and structuring the raw dataset.

The NASA dataset is provided as a space-delimited text file without descriptive column headers.

The raw data was imported into Excel and separated into individual columns using Text to Columns.

The dataset was then verified to contain:

- 20,631 rows
- 26 columns
- 100 unique simulated engine units

The 26 NASA-defined column names were added to the dataset.

### Completed Excel Work

- Imported raw FD001 training data
- Separated space-delimited values
- Added column headers
- Verified dataset dimensions
- Checked for blank values
- Found zero blank cells

Further data-quality checks will be performed before moving to Python.

## Phase 2 — Python / Pandas

After completing the Excel stage, the dataset will be analyzed using Python and Pandas.

The purpose of this stage is to create a reproducible data-cleaning and analysis workflow.

Planned work includes:

- Dataset inspection
- Data-type validation
- Missing-value analysis
- Duplicate analysis
- Engine-level analysis
- Cycle analysis
- Sensor statistics
- Sensor variability
- Descriptive statistics
- Outlier investigation
- Exploratory data analysis
- Sensor trend analysis
- Exporting the cleaned dataset

## Phase 3 — SQL

The cleaned dataset will be loaded into PostgreSQL.

SQL will be used to analyze the engine fleet and sensor data.

Planned analysis includes:

- Operating cycles per engine
- Engine operating-life comparisons
- Sensor averages
- Minimum and maximum sensor values
- Engine-level comparisons
- Cycle-level analysis
- Grouping and aggregation
- Sensor relationships
- Identification of unusual patterns

## Phase 4 — Power BI

The cleaned and analyzed dataset will be used to create a Power BI dashboard.

The dashboard will focus on aircraft engine health and operating behavior.

Planned dashboard analysis includes:

- Total number of engines
- Total operating cycles
- Engine operating-life analysis
- Individual engine filtering
- Sensor trends
- Temperature analysis
- Pressure analysis
- Engine-speed analysis
- Sensor variability
- Engine-to-engine comparisons
- Operating-cycle analysis

The purpose of the dashboard is to convert the sensor data into meaningful engineering insights.

## Phase 5 — Machine Learning

Machine learning will be introduced only after the Excel, Python/Pandas, SQL, and Power BI stages are completed.

The final phase will investigate predictive-maintenance applications such as:

- Remaining Useful Life prediction
- Engine degradation prediction
- Anomaly detection
- Engine health assessment
- Sensor-based predictive analysis

Multiple machine learning models will be trained and evaluated rather than assuming that one algorithm is automatically the best.

The model selection will be based on the problem, data characteristics, and evaluation results.

## Final Objective

The final objective is to develop a complete aircraft engine predictive maintenance workflow:

Raw NASA Data
→ Excel
→ Data Cleaning
→ Python/Pandas
→ Exploratory Data Analysis
→ PostgreSQL/SQL
→ Power BI
→ Machine Learning
→ Predictive Maintenance

The project will demonstrate the ability to work with aerospace data from its raw form through data preparation, analysis, visualization, and eventually predictive modeling.

## Current Status

### Completed

- [x] NASA C-MAPSS dataset selected
- [x] FD001 selected
- [x] Raw training data imported
- [x] Text-to-Columns completed
- [x] 26-column structure verified
- [x] NASA column names added
- [x] Dataset size verified: 20,631 × 26
- [x] Blank-value check completed
- [x] Zero blank cells identified

### Current Stage

- [ ] Remaining Excel data-quality checks
- [ ] Export structured CSV
- [ ] Begin Python/Pandas analysis

### Upcoming

- [ ] Python/Pandas cleaning
- [ ] Exploratory Data Analysis
- [ ] PostgreSQL implementation
- [ ] SQL analysis
- [ ] Power BI dashboard
- [ ] Portfolio documentation
- [ ] Machine learning experiments
- [ ] Model comparison
- [ ] Predictive-maintenance analysis

## Sources

NASA Prognostics Center of Excellence Data Set Repository:

https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/

Technical Reference:

Saxena, A. & Goebel, K. — Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation, PHM08.

NASA C-MAPSS FD001 dataset documentation and README supplied with the dataset.

## Dataset Disclaimer

The C-MAPSS FD001 dataset is simulated data generated using NASA's Commercial Modular Aero-Propulsion System Simulation.

The Unit_Number values represent simulated engine units, not real aircraft registrations, aircraft names, or real-world engine serial numbers.

This project should therefore be interpreted as an aircraft engine predictive maintenance study using simulated aerospace data.
