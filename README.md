# Service-Data-Analysis

## 🎯 Project Overview
Comprehensive analysis of service work orders and repair data for equipment maintenance operations. This project includes data cleaning, integration, exploratory data analysis (EDA), and root cause identification.

## 🔧 Technologies Used
- **Python 3.8+**
- **Pandas** - Data manipulation
- **Matplotlib & Seaborn** - Visualizations
- **OpenPyXL** - Excel file handling

## 📊 Project Tasks

### Task 2: Data Cleaning & Integration
1. **Primary Key Identification**
   - Analyzed: `Primary Key`, `Order No`, `Segment Number`
   - Selected: `Primary Key` (highest uniqueness, specifically designed for integration)
   - Challenge: One-to-many relationship exists (work orders can have multiple repairs)

2. **Data Cleaning**
   - Handled missing values (filled categoricals with 'Unknown')
   - Standardized date formats
   - Converted numeric columns
   - Ensured data type consistency

3. **Data Integration**
   - Join Type: **LEFT JOIN**
   - Rationale: Preserves all work orders (primary business records)
   - Maintains complete history including incomplete/pending repairs

### Task 3: Exploratory Data Analysis

#### Key Visualizations

1. **Monthly Service Order Trends**
   - Identified peak demand periods
   - Seasonal pattern analysis
   - Resource planning insights

2. **Component Failure Analysis**
   - Top 10 failure components by frequency
   - Cost vs Revenue comparison
   - Profit margin analysis

3. **Correlation Heatmap**
   - Strong correlation between Actual Hours and Cost (r > 0.8)
   - Labor hours identified as primary cost driver
   - Revenue-cost relationship analysis

#### Root Cause Investigation

- **Failure-Fix Patterns**: Most common component failures and corrections
- **Cost Analysis**: Top 5 most expensive repairs identified
- **Manufacturer Performance**: Repair frequency and cost by manufacturer

## 🚀 Installation & Usage

### Prerequisites
```bash
Python 3.8 or higher
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run Analysis
```bash
python service_analysis.py
```

### Update Configuration
Edit file paths in the script:
```python
FILE_PATH = r"path/to/your/data.xlsx"
OUTPUT_PATH = r"path/to/output.xlsx"
```

## 📤 Outputs Generated

1. **Excel File** with 3 sheets:
   - Cleaned Work Orders
   - Cleaned Repairs
   - Merged Dataset

2. **Visualizations** (PNG format):
   - Monthly trends chart
   - Failure component analysis
   - Correlation heatmap

3. **Summary Statistics** (CSV)

## 📊 Key Findings

### Data Integration Results
- Total work orders processed: [X]
- Work orders with repair data: [Y]
- Match rate: [Z]%

### Top Insights
- Most frequent failure component: [Component Name]
- Highest cost driver: Labor hours
- Peak service month: [Month]
- Average repair cost: $[Amount]

## 🔑 Key Features

✅ Comprehensive data cleaning pipeline  
✅ Justified primary key selection  
✅ LEFT JOIN with clear rationale  
✅ 3+ professional visualizations  
✅ Root cause analysis  
✅ Automated report generation  

