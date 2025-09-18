# Cryptocurrency Adoption Analysis

[![Python](https://img.shields.io/badge/Python-3.12-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

This project performs an **Exploratory Data Analysis (EDA)** on cryptocurrency adoption trends in **Nigeria**, **Ukraine**, and **India** over the period **2024-2025**. The analysis focuses on key **economic**, **social**, and **technological indicators** to uncover factors driving crypto usage, such as inflation, currency volatility, internet penetration, and regulatory environments.

Key components include:
- Data cleaning and preparation.
- Visualizations (e.g., scatter plots, correlation heatmaps).
- Statistical analysis (e.g., linear regression between peace index and crypto ownership).
- Insights into correlations between violence/volatility and adoption rates.

The notebook reveals patterns like higher adoption in regions with economic instability (e.g., Nigeria's 10.3% crypto ownership amid 20.12% inflation) and explores potential drivers like mobile money usage and smartphone penetration.

## Features

- **Data Visualization**: Seaborn and Matplotlib plots for trends and regressions.
- **Statistical Tools**: Linear regression, PCA, and hierarchical clustering via SciPy and scikit-learn.
- **Country-Specific Data**: Hardcoded datasets for Nigeria, Ukraine, and India with 28+ indicators.
- **Reproducible Analysis**: Self-contained Jupyter notebook with all code and outputs.

## Installation

1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/crypto-adoption-analysis.git
   cd crypto-adoption-analysis
   ```

2. **Set Up Environment** (Recommended: Use a virtual environment):
   ```
   python -m venv myenv
   source myenv/bin/activate  # On Windows: myenv\Scripts\activate
   ```

3. **Install Dependencies**:
   Install the required Python packages:
   ```
   pip install pandas matplotlib seaborn numpy scipy scikit-learn jupyter
   ```

   Or use the provided `requirements.txt` (if added):
   ```
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**:
   ```
   jupyter notebook Crypto_adoption.ipynb
   ```

## Usage

1. Open `Crypto_adoption.ipynb` in Jupyter Notebook or JupyterLab.
2. Run cells sequentially to load data, perform EDA, and generate visualizations.
3. Key sections:
   - **Setup & Imports**: Installs libraries and sets styles.
   - **Data Loading**: Loads country-specific DataFrames (Nigeria, Ukraine, India).
   - **Data Cleaning**: Converts metrics to numeric values and handles non-numeric entries.
   - **Exploratory Analysis**: Computes correlations, scales data, and runs PCA/clustering.
   - **Visualizations**: Plots like GPI-Crypto regression.
   - **Insights**: Summary of findings (e.g., positive correlation between economic volatility and adoption).

Example output: A scatter plot showing the relationship between Global Peace Index scores and crypto ownership percentage, with an r-value for regression strength.

To extend:
- Add more countries by appending DataFrames.
- Update data for new years via external sources (e.g., World Bank API).

## Data Sources

Data is sourced from reliable public datasets and aggregated for 2024-2025 estimates:
- **Economic Indicators**: World Bank, IMF (GDP, inflation, unemployment).
- **Social Indicators**: UN Population Division (median age, fertility), Global Peace Index.
- **Technological Indicators**: GSMA (smartphone ownership), ITU (internet penetration).
- **Crypto-Specific**: Chainalysis reports, Triple-A surveys (% owning crypto), CoinMetrics (trading volumes).
- **Regulatory**: Local government announcements (e.g., Nigeria's licensed status).

Full sources are referenced in the notebook's "Sources for data" table (under Data Loading section). Data is hardcoded for reproducibility but can be externalized.

| Category          | Example Indicators                  | Sources                          |
|-------------------|-------------------------------------|----------------------------------|
| Economic         | GDP/capita, Inflation %            | World Bank, IMF                 |
| Social           | Poverty rate, Gini coefficient     | UN, World Bank                  |
| Technological    | Internet penetration, Mobile money | GSMA, ITU                       |
| Crypto           | % owning crypto, Trading volume    | Chainalysis, Triple-A           |

## Dependencies

- **Python**: 3.12+
- **Libraries**:
  - `pandas`: Data manipulation.
  - `matplotlib` & `seaborn`: Visualization.
  - `numpy`: Numerical computing.
  - `scipy`: Statistics (linregress, clustering).
  - `scikit-learn`: PCA and preprocessing.
  - `jupyter`: Notebook execution.

See `requirements.txt` for pinned versions.

## Contributing

Contributions are welcome! Please:
1. Fork the repo and create a feature branch (`git checkout -b feature/amazing-feature`).
2. Commit changes (`git commit -m 'Add amazing feature'`).
3. Push to the branch (`git push origin feature/amazing-feature`).
4. Open a Pull Request.

For major changes, open an issue first to discuss.

---

*Last updated: September 18, 2025*
