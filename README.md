# Brazilian Real Estate Market Analysis

A comprehensive analysis of the Brazilian real estate market using Python, examining regional differences and the relationship between home size and price, with a focus on southern Brazil.

## Project Overview

This project analyzes a dataset of homes for sale across Brazil to:
- Identify regional differences in the real estate market
- Examine the relationship between home size and price
- Focus specifically on the southern region of Brazil
- Visualize geographic distribution and pricing patterns

## Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Static visualizations (histograms, box plots, scatter plots)
- **Plotly Express** - Interactive charts and dashboards

## Dataset

The project uses two CSV files containing Brazilian real estate data collected in 2015-2016:
- `brasil-real-estate-1.csv`
- `brasil-real-estate-2.csv`

**Key features:**
- Property location (latitude, longitude)
- Property size (area in square meters)
- Price (in USD and Brazilian Reais)
- Region and state information

## Project Structure

```
brazilian-real-estate-analysis/
│
├── data/
│   ├── brasil-real-estate-1.csv
│   ├── brasil-real-estate-2.csv
│   └── brasil-real-estate-clean-1.csv
│
├── notebooks/
│   └── real_estate_analysis.ipynb
│
├── README.md
└── requirements.txt
```

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/brazilian-real-estate-analysis.git
cd brazilian-real-estate-analysis
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Data Cleaning Process

The following data cleaning steps were performed:

1. **Removed null values** from the dataset
2. **Split lat-lon column** into separate latitude and longitude columns
3. **Converted data types** from object to float for numerical columns
4. **Extracted state information** from the `place_with_parent_names` column
5. **Currency conversion** from Brazilian Reais to USD (exchange rate: 1 USD = 3.19 BRL)
6. **Dropped unnecessary columns** after transformation
7. **Combined datasets** from both CSV files into a single DataFrame

## Analysis Components

### 1. Exploratory Data Analysis
- Summary statistics for property area and price
- Distribution analysis of home prices
- Distribution analysis of home sizes

### 2. Regional Analysis
- Mean home price by region across Brazil
- Visualization of regional price differences

### 3. Southern Region Focus
- Property distribution by state in the South region
- Price vs. area scatter plot analysis
- Correlation analysis between area and price for each southern state

## Key Findings

The analysis examines:
- Regional price variations across Brazil
- The relationship between property size and price
- State-level differences within the southern region
- Correlation coefficients between area and price by state

## Visualizations

The project includes:
- **Histogram** - Distribution of home prices
- **Box Plot** - Distribution of home sizes
- **Bar Chart** - Mean home price by region
- **Scatter Plot** - Price vs. area relationship
- **Map Visualization** - Geographic distribution of properties

## Usage

Open and run the Jupyter notebook:
```bash
jupyter notebook notebooks/real_estate_analysis.ipynb
```

Follow the notebook cells sequentially to reproduce the analysis.

## Contributing

Feel free to fork this project and submit pull requests for any improvements.

## License

This project is open source and available under the MIT License.

## Author

Caleb Ajibola- [Your GitHub Profile](https://github.com/Caleb-Ajibola)

## Acknowledgments

- Data source: Brazilian real estate market data (2015-2016)
- Analysis conducted as part of a data science project study
