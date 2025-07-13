---
layout: default
title: Data Prep and EDA
---

<ul class="nav">
  <li><a href="index.html">Home</a></li>
  <li><a href="introduction.html">Introduction</a></li>
  <li><a href="conclusion.html">Conclusions</a></li>
  <li class="dropdown">
    <a href="dataprep_eda.html" class="dropbtn">DataPrep_EDA</a>
    <div class="dropdown-content">
      <a href="clustering.html">Clustering</a>
      <a href="arm.html">ARM</a>
      <a href="naivebayes.html">NaiveBayes</a>
      <a href="dectrees.html">DecTrees</a>
      <a href="svms.html">SVMs</a>
      <a href="regression.html">Regression</a>
      <a href="nn.html">NN</a>
    </div>
  </li>
</ul>

<style>
.nav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

.nav li {
  float: left;
  position: relative;
}

.nav li a, .dropbtn {
  display: inline-block;
  padding: 14px 16px;
  text-decoration: none;
  background-color: #f9f9f9;
}

.nav li .dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
}

.nav li:hover .dropdown-content {
  display: block;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  display: block;
  text-decoration: none;
}

.dropdown-content a:hover {
  background-color: #ddd;
}
</style>

# Data Prep and EDA

# Data Preparation & Exploratory Data Analysis (EDA)

## Data Sources and Collection Methods

For this project, two primary datasets were gathered to support the goal of forecasting mental health service demand based on projected population growth in Colorado:

1. **Colorado Population Projections Dataset**
   - Source: [Colorado Information Marketplace](https://data.colorado.gov/Demographics/Population-Projections-in-Colorado/q5vp-adf3/about_data)
   - Download Format: CSV
   - [Download Raw Dataset](assets/Population_Projections_in_Colorado_20250713.csv)

2. **U.S. Census Bureau API – ACS 5-Year Estimates**
   - API Source: [https://www.census.gov/data/developers/data-sets.html](https://www.census.gov/data/developers/data-sets.html)
   - API GET Example:
     ```
     https://api.census.gov/data/2022/acs/acs5?get=NAME,B01003_001E&for=county:*&in=state:08&key=YOUR_API_KEY
     ```
   - [View Python Notebook for API Collection](assets/colorado_population_api_project.ipynb)

## Why These Datasets Were Chosen

Population projections provide a foundational view of where service demand is likely to grow, especially among specific age groups and geographic regions. Combining this with U.S. Census estimates allows for a more complete picture of baseline population and demographic trends across Colorado counties.

---

## Raw Data Snapshots

### Example from Colorado Population Projections CSV:

![Raw Population Data](assets/raw_population_data.png)

### Example from Census API Dataset:

![Raw Census API Data](assets/raw_census_api_data.png)

---

## Data Cleaning and Preparation Steps
