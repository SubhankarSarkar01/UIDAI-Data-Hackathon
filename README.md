# UIDAI Aadhar Data Analysis

A comprehensive data analysis project for UIDAI (Unique Identification Authority of India) Aadhar enrollment, demographic, and biometric data. This project processes large-scale datasets and provides insights through data cleaning, transformation, and visualization.

## 📁 Project Structure
```
Hackathon/
├── api_data_aadhar_enrolment/
│ ├── api_data_aadhar_enrolment_*.csv # Enrollment data files (segmented)
│ ├── enrolment.py # Enrollment data processing script
│ ├── Enrollment.ipynb # Enrollment analysis notebook
│ ├── west_bengal_*.csv # Processed West Bengal enrollment data
│ └── wb_month_enroll_trend.csv # Monthly enrollment trends
│
├── api_data_aadhar_demographic/
│ ├── api_data_aadhar_demographic_*.csv # Demographic data files (segmented)
│ ├── Demography.ipynb # Demographic analysis notebook
│ ├── df_wb_*.csv # Aggregated demographic datasets
│ ├── pin_district_demo_map.csv # PIN code to district mapping
│ └── west_bengal_*.csv # West Bengal demographic datasets
│
├── api_data_aadhar_biometric/
│   └── api_data_aadhar_biometric_*.csv      # Biometric data files (segmented)
│
└── README.md                                  # Project documentation
```


## 📊 Datasets

The project contains data segmented into manageable CSV files:

### Enrollment Data
- **api_data_aadhar_enrolment_0_500000.csv** - Records 0 to 500,000
- **api_data_aadhar_enrolment_500000_1000000.csv** - Records 500,000 to 1,000,000
- **api_data_aadhar_enrolment_1000000_1006029.csv** - Records 1,000,000 to 1,006,029

### Demographic Data
- **api_data_aadhar_demographic_0_500000.csv** - Records 0 to 500,000
- **api_data_aadhar_demographic_500000_1000000.csv** - Records 500,000 to 1,000,000
- **api_data_aadhar_demographic_1000000_1500000.csv** - Records 1,000,000 to 1,500,000
- **api_data_aadhar_demographic_1500000_2000000.csv** - Records 1,500,000 to 2,000,000
- **api_data_aadhar_demographic_2000000_2071700.csv** - Records 2,000,000 to 2,071,700

### Biometric Data
- **api_data_aadhar_biometric_0_500000.csv** - Records 0 to 500,000
- **api_data_aadhar_biometric_500000_1000000.csv** - Records 500,000 to 1,000,000
- **api_data_aadhar_biometric_1000000_1500000.csv** - Records 1,000,000 to 1,500,000
- **api_data_aadhar_biometric_1500000_1861108.csv** - Records 1,500,000 to 1,861,108

## 🔧 Technologies & Libraries

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive analysis

## 📝 Scripts & Notebooks

### Enrollment Analysis
- **enrolment.py** - Main script for processing enrollment data
  - Concatenates multiple enrollment CSV files
  - Date format standardization (DD-MM-YYYY → YYYY-MM-DD)
  - Data quality checks and validation

- **Enrollment.ipynb** - Interactive notebook for enrollment insights
  - Exploratory data analysis
  - District-level aggregations
  - Temporal trend analysis

### Demographic Analysis
- **Demography.ipynb** - Interactive notebook for demographic insights
  - Multi-file data consolidation
  - State and PIN code level analysis
  - Conflict detection and resolution

## 🚀 Getting Started

```bash
pip install pandas numpy matplotlib seaborn jupyter

# Run enrollment processing
python enrolment.py

# Open Jupyter notebooks
jupyter notebook
```

### 📈 KeyFeatures

- Large-scale Data Processing: Handles millions of records efficiently
- Data Cleaning: Standardizes date formats and validates data quality
- Geographical Analysis: District and PIN code level insights
- Temporal Analysis: Monthly enrollment trends and patterns
- Data Aggregation: Consolidates segmented data into unified datasets


### 📊 Output Files
West Bengal Analysis
- west_bengal_cleaned_data.csv - Cleaned and processed enrollment data
- west_bengal_district_level.csv - District-wise aggregation
- west_bengal_district_level_all.csv - Enhanced district analysis
- west_bengal_pincode_level.csv - PIN code level insights
- wb_month_enroll_trend.csv - Monthly enrollment trends

Demographic Aggregations
- df_wb_dist_demo_level.csv - District-level demographic data
- df_wb_month_demo_level.csv - Monthly demographic trends
- df_wb_pincode_demo_level.csv - PIN code level demographics
- pin_district_demo_map.csv - PIN code to district mappings

### 📌 Data Processing Pipeline
1. Load - Read segmented CSV files
2. Transform - Standardize dates and formats
3. Validate - Check for missing values and 4. data quality
4. Aggregate - Consolidate by geography and time periods
5. Analyze - Generate insights and statistics
6. Visualize - Create charts and visualizations

### 🔍 Data Quality Checks
- Null value detection and reporting
- Date format validation
- State-wise data verification
- PIN code conflict resolution

### 📚 Documentation
For detailed UIDAI Hackathon requirements and specifications, see:

- UIDAI Hackathon.docx
- UIDAI Hackathon_PDF.pdf

### 🤝 Contributing
This project is part of the UIDAI Hackathon initiative. Contributions and improvements are welcome.


### 📄 License
This project uses data from the Unique Identification Authority of India (UIDAI).

### 📞 Contact
For questions or support, please refer to the UIDAI Hackathon documentation included in the repository.