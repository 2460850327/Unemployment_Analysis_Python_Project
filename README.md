# Unemployment Analysis with Python 📊

A Python-based exploratory data analysis (EDA) project that examines unemployment trends in India using `pandas`, `matplotlib`, and `seaborn`. The project cleans raw unemployment data, visualizes trends, and investigates the impact of COVID-19 on employment across regions, areas, and seasons.

## Project Objective

Analyze unemployment-rate data using Python to:
- Clean and prepare the dataset
- Explore unemployment patterns
- Visualize unemployment trends
- Investigate the impact of COVID-19
- Identify regional, rural/urban, and seasonal patterns
- Generate insights that can support economic and social policy discussions

## Dataset

The analysis uses the **Unemployment in India** dataset, which includes:

| Column | Description |
|---|---|
| `Region` | State/region in India |
| `Date` | Date of observation |
| `Frequency` | Reporting frequency (e.g., Monthly) |
| `Estimated Unemployment Rate (%)` | Unemployment rate |
| `Estimated Employed` | Number of people employed |
| `Estimated Labour Participation Rate (%)` | Labour force participation rate |
| `Area` | Rural or Urban |

> The dataset is not included in this repository. Download it (e.g., from [Kaggle: Unemployment in India](https://www.kaggle.com/datasets/gokulrajkmv/unemployment-in-india)) and update the `DATA_PATH` / file path in the notebook to point to your local copy.

## Tech Stack

- **Python 3**
- **pandas** – data manipulation and cleaning
- **numpy** – numerical operations
- **matplotlib** – static visualizations
- **seaborn** – statistical visualizations
- **Jupyter Notebook**

## Project Workflow

1. **Import Libraries** – Load required Python packages
2. **Load the Dataset** – Read the CSV file into a DataFrame
3. **Understand the Dataset** – Inspect shape, columns, data types, missing values, and duplicates
4. **Data Cleaning**
   - Strip whitespace from column names
   - Remove duplicate rows
   - Convert `Date` to datetime and numeric columns to proper types
   - Drop rows with missing date/unemployment values
   - Create time-based features (`Year`, `Month`, `Month_Name`)
5. **Descriptive Statistics** – Summary statistics of key metrics
6. **Overall Unemployment Trend** – Time series plot with a COVID-19 marker (March 2020)
7. **COVID-19 Impact Analysis** – Compare pre-COVID vs. COVID-period unemployment
8. **COVID-19 Impact by Region** – Regional comparison of unemployment change
9. **Rural vs. Urban Analysis** – Compare unemployment across areas
10. **Regional Unemployment Trends** – Line chart comparing trends by region
11. **Seasonal Pattern Analysis** – Identify months with higher/lower unemployment
12. **Highest & Lowest Observations** – Extreme unemployment records
13. **Employment & Labour Participation** – Trends in employment and labour force participation
14. **Correlation Analysis** – Relationship between unemployment, employment, and labour participation
15. **Key Insights** – Auto-generated summary of findings
16. **Policy-Relevant Interpretation** – Discussion of policy implications
17. **Final Conclusion** – Summary of the overall analysis

## Key Insights

- Unemployment patterns vary significantly across **regions**, **rural/urban areas**, and **seasons**.
- The COVID-19 period (March 2020 onward) shows a measurable shift in unemployment compared to the pre-COVID period.
- Correlation analysis highlights relationships between unemployment, employment levels, and labour participation.
- Findings support policy discussions around employment generation, crisis preparedness, skill development, and seasonal planning.

*Note: This analysis identifies patterns and correlations; it does not establish causation.*

## Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Place the dataset (`Unemployment in India.csv`) in the project folder.
3. Update the `DATA_PATH` variable in the notebook to point to your dataset location.
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open `Unemployment_Analysis_Python_Project.ipynb` and run all cells.

## Project Structure

```
├── Unemployment_Analysis_Python_Project.ipynb   # Main analysis notebook
├── README.md                                     # Project documentation
└── data/                                         # (Add dataset here — not tracked in repo)
```

## Future Improvements

- Add interactive visualizations (e.g., Plotly)
- Build a forecasting model for future unemployment trends
- Deploy an interactive dashboard (e.g., Streamlit)
- Incorporate additional macroeconomic indicators for deeper analysis

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Dataset source: Kaggle – Unemployment in India
- Built with Python's data science stack (pandas, matplotlib, seaborn)
