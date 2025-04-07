# UK Road Accident and Safety Data Analysis

## Project Overview
This project analyzes UK road accident data to uncover patterns, identify risk factors, and develop predictive models for accident severity. The analysis aims to provide insights that could help inform road safety policies and targeted interventions to reduce both the frequency and severity of road accidents.

## Dataset Description
The analysis is based on two primary datasets:

1. **Accident Information Dataset**:
   - Contains information about accidents including location, date, time, severity, road conditions, weather conditions, etc.
   - 2,047,256 observations with 34 features

2. **Vehicle Information Dataset**:
   - Contains information about vehicles involved in accidents including vehicle type, age, driver information, etc.
   - 2,177,205 observations with 24 features

## Analysis Methods
The project follows a comprehensive data science workflow:

1. **Data Exploration and Cleaning**:
   - Analysis of dataset structure and features
   - Handling missing values
   - Data quality assessment

2. **Exploratory Data Analysis**:
   - Distribution of accident severity
   - Impact of road and weather conditions
   - Temporal patterns (time of day, day of week, seasonality)
   - Relationship between vehicle characteristics and accident outcomes

3. **Machine Learning Models**:
   - Prediction of accident severity
   - Techniques for handling class imbalance:
     - Class weights
     - Undersampling
     - Custom thresholds
     - Ensemble methods
   - Model evaluation using balanced metrics

## Key Findings
- Distribution of accident severity shows imbalanced classes with most accidents classified as "Slight"
- Road surface conditions impact accident severity, with specific conditions associated with more serious accidents
- Weather conditions show correlation with accident frequency and severity
- Specific vehicle types and driver demographics exhibit different risk profiles
- The machine learning models can predict accident severity with reasonable performance, especially after addressing class imbalance

## Setup and Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook

### Required Libraries
```
numpy
pandas
matplotlib
seaborn
scikit-learn
```

### Running the Analysis
1. Clone this repository:
   ```
   git clone https://github.com/yourusername/uk-accident-and-safety.git
   cd uk-accident-and-safety
   ```

2. Install required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Download the datasets and place them in the `dataset` directory:
   - Accident_Information.csv
   - Vehicle_Information.csv

4. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

5. Open and run `ammar_data_analysis.ipynb`

## Notebook Structure
The Jupyter notebook `ammar_data_analysis.ipynb` is organized into the following sections:

1. **Libraries and Setup**: Importing necessary libraries
2. **Exploratory Data Analysis**: Loading and examining datasets
3. **Data Visualization**: Visual analysis of accident patterns
4. **Data Preprocessing**: Handling missing values and preparing features
5. **Machine Learning Models**: Building and evaluating predictive models
6. **Advanced Techniques**: Addressing class imbalance in accident severity
7. **Results and Evaluation**: Model performance and feature importance

## Future Work
- Incorporate additional datasets such as road infrastructure and traffic volume
- Explore spatial analysis using geographic data
- Develop interactive dashboards for exploring accident patterns
- Implement more advanced modeling techniques such as deep learning

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- UK Department for Transport for providing the accident data
- Contributors to the pandas, scikit-learn, and visualization libraries that made this analysis possible