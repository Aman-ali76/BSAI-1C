# Data Analysis Project


Welcome to the **Data Analysis Project**! This project covers data loading, cleaning, preprocessing, and visualization using **Python** and **Pandas**. Below are all the details, screenshots, and the explanation of functionality of the project.



## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Setup Instructions](#setup-instructions)
4. [Code Overview](#code-overview)
5. [Results](#results)
6. [Owner](#owner)
---

## Introduction

This project analyzes and visualizes data to uncover patterns, and insights. By using **Pandas** for data manipulation and visualization, the project covers the following steps:

- Data loading and cleaning
- Handling missing values
- Data slicing and grouping
- Generating statistical summaries
- Creating visualizations like bar charts, histograms, and line graphs

---

## Features

- **Data Loading**: Read data from CSV files into Pandas DataFrames.
- **Data Cleaning**: Handle missing values and rename columns.
- **Statistical Analysis**: Generate summaries like mean, mode, and median.
- **Visualization**: Create interactive and static plots.
- **observations**: Derive meaningful results from the data.

---

## Setup Instructions

### Requirements

- Python 3.8+
- Anaconda
- Jupyter Notebook
- Libraries:
  - Pandas

### Steps

1. Clone the repository or download the project files.
2. Open the `data_analysis.ipynb` notebook in Jupyter.
3. Run the notebook cells sequentially to reproduce the analysis.

---

## Code Overview

### 1. Data Loading

```python
import pandas as pd

data = pd.read_csv('your_dataset.csv')
data.head()
```

### 2. Handling Missing Values

```python
# Checking for NULL values
data.isnull().sum()

# Filling NULL values with the mean of the column
df['Weather'] = df['Weather'].fillna(df['Weather'].mode()[0])
```

### 3. Statistical Analysis

```python
# Generating descriptive statistics
data.describe()

# Finding mean, median, and mode
mean_value = df['Temperature'].mean()
median_value = df['Distance (km)'].median()
mode_value = df['Weather'].mode()[0]
```

### 4. Data Visualization

```python

# Bar plot
df['Delivery_person_Ratings'].value_counts().plot(kind='bar',title="Bar Chart",color='blue')

# Histogram
df['Distance (km)'].plot(kind='hist',title="Histogram",color='orange')
```

---

## Results

### observations

1. **Trend Analysis**: The data reveals a clear upward/downward trend in Delivery Data Set.
2. **Missing Values**: Successfully handled NULL values, improving data quality.

### Visualizations

#### Bar Chart Example
<img src="https://images.twinkl.co.uk/tw1n/image/private/t_630/u/ux/barchart_ver_1.jpg" width="300px">

#### Histogram Example

<img src="https://businessq-software.com/wp-content/uploads/2016/04/businessq-pie-chart-controversy-2.png" width="300px">

---

## Owner

- **Muhammad Aman Ali**
  - **Roll Number**: 195
  - **Program**: BS Artificial Intelligence
  - **Section**: 1C
  - **University**: Superior University, Gold Campus, Lahore

---

## HI