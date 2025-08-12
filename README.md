#Automated EDA in Python

This project provides a **Python script** that performs **Exploratory Data Analysis (EDA)** on any CSV dataset automatically.  
It loads the dataset, inspects its structure, analyzes missing values, detects outliers, and generates visualizations — all in one go.

---

##Features
- **Flexible Dataset Loading**
  - Load CSV directly from a specified file path.
  - Or choose a file through a selection dialog if no path is provided.
- **Automatic Data Inspection**
  - First 5 rows preview.
  - Dataset info (rows, columns, data types).
  - List of numerical and categorical features.
- **Data Quality Checks**
  - Missing values summary.
  - Outlier detection using the **IQR method**.
- **Categorical Feature Analysis**
  - Value counts for each categorical column.
- **Visualizations**
  - Histograms of numerical features.
  - Boxplots for outlier visualization.
  - Correlation heatmap for numerical columns.

---

##Project Structure
```
├── eda_script.py     # Main Python script
├── README.md         # Documentation
└── Cuisine_rating.csv # Example dataset (optional)
```

---

## Installation

1. **Clone this repository** (or download the script):
```bash
git clone https://github.com/yourusername/eda-python.git
cd eda-python
```

2. **Install dependencies**:
```bash
pip install pandas matplotlib seaborn
```
Optional (for file selection dialog):
```bash
pip install tk
```

---

##Usage

### **Option 1 — Run with predefined dataset path**
Edit in the script:
```python
dataset_path = "/path/to/your/dataset.csv"
```
Run:
```bash
python eda_script.py
```

### **Option 2 — Run and choose file**
Set:
```python
dataset_path = None
```
When run, a file selection dialog will open.

---

## Output
- Dataset preview & info
- Missing value summary
- Outlier detection results
- Value counts for categorical columns
- Visualizations:
  - Histograms
  - Boxplots
  - Correlation heatmap

---

## Notes
- Only supports CSV files.
- For large datasets, plotting may take more time.
- Works with both **Jupyter Notebook** and normal Python execution.

---

## License
This project is licensed under the MIT License — you are free to use and modify it.
