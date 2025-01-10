# Long-term experiments in agronomy dataset & analysis: Part of the ERA data ecosystem

Welcome to the **ERA LTEs Analysis Repository**, part of the Excellence in Agronomy Initiative (EiA). This repository contains R code and a vignette for analyzing the performance of long-term agronomic experiments (LTEs). The primary focus is on integrating climate data to explore the impact of climate on experimental outcomes, such as yield and economic performance.

The dataset contains 34815 individual outcomes from 181 long-term experiments (LTEs) derived from 211 unique publications. These come from 260 sites in 28 countries. The average number of observations per study is 99 and the average duration of LTEs is 13.5 years.

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/user-attachments/assets/5f9a3750-3135-48ea-a792-82ca028d3b5b" alt="Image 1" width="45%" />
    <img src="https://github.com/user-attachments/assets/c1cadbb6-3366-4eef-9bc3-b32d807a7d9b" alt="Image 2" width="45%" />
</div>

LTES cover a range of agronomic management practices and experimental outcomes.
<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/user-attachments/assets/79dffbf6-0a26-4cc4-b531-9055adf1e394)" alt="Image 3" width="45%" />
    <img src="https://github.com/user-attachments/assets/eeb52e7b-1d1a-4027-9841-4a934576e1ca)" alt="Image 4" width="45%" />
</div>

---

## Purpose

The purpose of this repository is to:
- Provide access to a large synthesis dataset of harmonized agronomic LTEs.
- Analyze and visualize the performance of LTEs using robust statistical and geospatial methods.
- Investigate the impact of climate variables on LTE outcomes.
- Provide a systematic mapping and meta-analysis framework for agricultural research.

---

## Contents

### Repository Structure
- **`ERA_ltes.Rproj`**: The R project file for organizing and managing the repository.
- **`era_ltes.Rmd`**: The main vignette file providing an in-depth guide to analyzing LTEs.
- **`/data`**: Folder for data files, including LTE and climate datasets.
- **`/R`**: Scripts used for processing, visualization, and meta-analysis.
- **`/docs`**: Documentation and outputs generated from analyses.
  
---

## Features

1. **Vignette**:
   - The vignette (`era_ltes.Rmd`) includes:
     - Exploration of LTE data from the ERA database.
     - Visualization of geographic distribution, practices, and outcomes in LTEs.
     - Systematic mapping of LTE durations and measured outcomes.
     - Methods to integrate and analyze climate data.

2. **Integration with Climate Data**:
   - Analyzes how climatic factors such as precipitation and temperature influence LTE outcomes.
   - Provides interactive tools to visualize climate trends and anomalies alongside LTE data.

3. **Systematic Mapping and Meta-Analysis**:
   - Frameworks to study the relationships between agricultural practices and outcomes.
   - Utilizes statistical and geospatial approaches to gain insights into LTE contributions.
     
---

## How to Use

To explore the data and analyses, open the `era_ltes.Rmd` file in RStudio and knit the document. This will generate an HTML report with comprehensive visualizations and insights.
Note that the `climate data` code block line `POWER.CHIRPS <- arrow::open_dataset("s3://digital-atlas/era/geodata/POWER.CHIRPS.parquet")` is connecting to a large cloud stored parquet file,it can take several minutes for this file to load even with a fast connection, please be patient.

---

## Data Sources

This repository uses the following data sources:
- **ERA Dataset**: A compilation of LTEs focused on agricultural practices and their outcomes across various geographies.
- **Climate Data**: Integrated climate datasets from [NASA POWER](https://power.larc.nasa.gov/) and [CHIRPS](https://www.chc.ucsb.edu/data/chirps).
- The dataset is available at this cloud storage address `s3://digital-atlas/era/data/`. LTE data is  contained in a series of tables within an `.RData` object. The naming convention of the object is `industrious_elephant_2023-YYYY-MM-DD.RData` where YYYY-MM-DD indicate the production date of the most recent version of the data (e.g. `industrious_elephant_2023-2025-01-10.RData`).
---

## Links

- [Link to Excel Template](https://github.com/CIAT/ERA_dev/blob/main/data_entry/industrious_elephant_2023/excel_data_extraction_template/V2.0.28%20-%20Industrious%20Elephant.xlsm)
- [ERA GitHub](https://github.com/CIAT/ERA_dev)
  
---

## Team

This project is led and implemented by the **Climate Action Lever** of the **Alliance of Bioversity International and CIAT**.

- **Lolita Muller** – *Research Associate and Lead Developer*  
  Email: [m.lolita@cgiar.org](mailto:m.lolita@cgiar.org)  
- **Todd Rosenstock** – *Principal Scientist*  
  Email: [t.rosenstock@cgiar.org](mailto:t.rosenstock@cgiar.org)  
- **Peter Steward** – *Scientist*  
  Email: [p.steward@cgiar.org](mailto:p.steward@cgiar.org)  
- **Namita Joshi** – *Senior Research Associate*  
  Email: [n.joshi@cgiar.org](mailto:n.joshi@cgiar.org)  

---

## License

This project is licensed under the [GPL-3.0 License](https://opensource.org/licenses/GPL-3.0).

---

## Acknowlegements

This work is supported under the **Climate** area of work within the **CGIAR Excellence in Agronomy Initiative**. EiA has funded the extraction and integration of LTE data.

---

![Logos](https://github.com/user-attachments/assets/d3112c9d-6392-46a2-9fc6-8d0b72e6aec1)


