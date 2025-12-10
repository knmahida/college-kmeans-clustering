# college-kmeans-clustering

## Overview
This project performs K-Means clustering analysis on a college dataset to segment higher education institutions based on financial and enrollment characteristics. The analysis explores relationships between tuition, enrollment, and graduation rates using unsupervised learning, then evaluates clustering performance against known private/public institution labels.

## Dataset
The analysis uses the `College_Data` dataset containing information about various U.S. colleges and universities with features including:
- **Out-of-State Tuition** (Outstate)
- **Room and Board Costs** (Room.Board)
- **Number of Full-time Undergraduates** (F.Undergrad)
- **Graduation Rate** (Grad.Rate)
- **Institution Type** (Private: Yes/No)
- Additional demographic and financial metrics

## Analysis Steps

### 1. Data Exploration & Visualization
- Load and inspect dataset structure
- Generate summary statistics and data type information
- Create scatter plots showing:
  - Room and Board costs vs. Graduation Rate (by Private status)
  - Out-of-State Tuition vs. Number of Full-time Undergraduates
- Generate histograms of distribution for:
  - Out-of-State Tuition (by Private status)
  - Graduation Rate (by Private status)

### 2. Data Cleaning
- Identify data anomalies (e.g., Graduation Rates > 100%)
- Fix invalid values to ensure data quality

### 3. K-Means Clustering
- Apply K-Means algorithm with 2 clusters to segment institutions
- Extract and analyze cluster centers
- Compare predicted clusters with actual Private/Public labels

### 4. Model Evaluation
- Generate confusion matrix comparing KMeans predictions to institution types
- Produce classification report with precision, recall, and F1-score metrics

## Key Findings
- K-Means successfully segments colleges into two clusters that correlate with private vs. public institution status
- Clear separation exists between institutions based on financial and enrollment characteristics
- The clustering aligns well with the known private/public classification

## Technologies Used
- **Python 3**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - K-Means clustering and metrics
