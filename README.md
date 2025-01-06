# S&P 500 Companies Analysis

## Project Overview
This project demonstrates how Python can be used to gain insights from publicly available data. The dataset used for this analysis contains information about S&P 500 companies, including their market capitalization, revenue, and sector classification. Through data cleaning, manipulation, visualization, and statistical analysis, we explore trends and patterns to answer the following questions:

1. Which sectors dominate the S&P 500?
2. What is the relationship between market cap and revenue?
3. How are market caps distributed across the dataset?

The project includes all relevant Python scripts, visualizations, and a summary of findings.

---

## Dataset Information
- **Source**: [Kaggle - S&P 500 Companies Dataset](https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks)
- **Format**: CSV
- **Content**:
  - `Company Name`: The name of the company.
  - `Sector`: The sector to which the company belongs.
  - `Market Cap`: Market capitalization of the company (in billions).
  - `Revenue`: Annual revenue of the company (in billions).

---

## Steps in the Analysis

### 1. Data Cleaning
- Removed duplicate rows to ensure unique entries for each company.
- Handled missing values in critical columns (`Market Cap`, `Revenue`, and `Sector`) by removing rows with missing or invalid data.
- Converted the `Market Cap` and `Revenue` columns to numeric types for proper analysis.

### 2. Data Manipulation
- Sorted the dataset by `Market Cap` to identify the largest companies.
- Grouped data by `Sector` to calculate average market cap and revenue for each sector.

### 3. Data Visualization
Three key visualizations were created:
- **Bar Chart**: Average market cap by sector.
- **Pie Chart**: Sector distribution of companies.
- **Scatter Plot**: Relationship between market cap and revenue.

### 4. Statistical Analysis
- Descriptive statistics for numerical columns (e.g., mean, median, standard deviation).
- Correlation analysis between market cap and revenue.

---

## Key Insights

### Sector Analysis
- The **Technology** sector has the highest average market capitalization, making it the dominant sector in the S&P 500.
- **Healthcare** and **Financials** sectors also have significant representation and market value.

### Market Cap Distribution
- The market cap distribution is highly right-skewed, with a small number of companies having exceptionally high market caps.
- Most companies fall into the small to mid-cap range.

### Revenue vs Market Cap
- A strong positive correlation (≈ 0.85) exists between market cap and revenue, suggesting that companies with higher revenues tend to have larger market caps.

---

## Visualizations
### 1. Average Market Cap by Sector
![Bar Chart](visualizations/average_market_cap_by_sector.png)
- Highlights the dominance of the Technology sector.

### 2. Sector Distribution
![Pie Chart](visualizations/sector_distribution.png)
- Shows the proportional representation of sectors in the S&P 500.

### 3. Market Cap vs Revenue
![Scatter Plot](visualizations/market_cap_vs_revenue.png)
- Displays the positive correlation between market cap and revenue.

---

## How to Run the Code
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/sp500-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd sp500-analysis
   ```
3. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the analysis script:
   ```bash
   python analysis.py
   ```
5. The visualizations will be saved in the `visualizations` folder.

---

## Conclusion
This analysis provides insights into the composition and financial characteristics of S&P 500 companies. By leveraging Python, we explored the dataset to uncover trends across sectors and key financial metrics. These insights can inform investment decisions, sector analysis, and economic studies.

For more details, refer to the Python scripts and visualizations included in this repository.

---

## Repository Structure
```
sp500-analysis/
|
|-- data/
|   |-- sp500_companies.csv
|
|-- scripts/
|   |-- analysis.py
|
|-- visualizations/
|   |-- average_market_cap_by_sector.png
|   |-- sector_distribution.png
|   |-- market_cap_vs_revenue.png
|
|-- README.md
|-- requirements.txt
```

---

## Acknowledgments
- Dataset provided by [Kaggle](https://www.kaggle.com/).
- Visualizations created with Matplotlib and Seaborn.

---

## Author
Kayden Rumsey - [GitHub Profile](https://github.com/KaydenRumsey/)

