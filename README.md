# Premier League Table Prediction 2024/25

A machine learning project that predicts the final Premier League table for the 2024/25 season using historical data from the past 10 years. The project analyzes team performance patterns, applies Random Forest classification, and provides comprehensive visualizations comparing predictions with actual results.

## Features

- **Historical Data Analysis**: Analyzes 10 years of Premier League data (2014-2024) to identify winning patterns and team performance trends
- **Machine Learning Prediction**: Uses Random Forest Classifier to predict final league positions based on early season performance
- **Championship Probability**: Calculates realistic probabilities for each team to win the Premier League based on historical data
- **Relegation Prediction**: Identifies teams most likely to be relegated based on past performance patterns
- **European Qualification Spots**: Predicts Champions League (top 4), Europa League (5th-6th), and Conference League (7th) qualification
- **Interactive Visualizations**: 
  - Bar charts comparing predicted vs actual league positions
  - Trend analysis of championship-winning teams over time
- **Comprehensive Accuracy Analysis**: 
  - Mean Absolute Error calculations
  - Position prediction accuracy metrics
  - Detailed comparison tables
- **Data Scraping**: Automated data collection from FBRef.com for historical Premier League statistics

## Technologies Used

- **Python 3.x**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning algorithms (Random Forest Classifier)
- **Matplotlib**: Data visualization and plotting
- **Jupyter Notebooks**: Interactive development environment
- **Web Scraping**: pandas.read_html() for data collection from FBRef.com

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Predicting-premier-league-table-for-2024-2025.git
   cd Predicting-premier-league-table-for-2024-2025
   ```

2. Install required dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib jupyter
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the notebooks in the following order:
   - `data_scrapping.ipynb` - Data collection and preprocessing
   - `data_analysis.ipynb` - Analysis, modeling, and visualization

## Project Structure

```
├── data_scrapping.ipynb          # Data collection from FBRef.com
├── data_analysis.ipynb           # Main analysis and prediction notebook
├── prem_2014_2025.csv           # Historical Premier League dataset
└── README.md                     # Project documentation
```

## Usage

### Data Collection
The `data_scrapping.ipynb` notebook automatically scrapes Premier League data from FBRef.com for seasons 2014-2025, including:
- Team statistics (wins, draws, losses, goals for/against)
- League positions and points
- Attendance figures
- Top scorers and goalkeepers

## Results

### Prediction Accuracy Metrics

The model was validated against the actual 2024/25 Premier League season results:

- **Mean Absolute Error (Position)**: 4.80 positions
- **Mean Absolute Error (Points)**: 10.65 points
- **Exact Position Predictions**: 5/20 teams (25.0%)
- **Within 1 Position**: 6/20 teams (30.0%)
- **Within 3 Positions**: 9/20 teams (45.0%)

### Perfect Predictions

The model accurately predicted the final position for:
- **Liverpool** (1st place - Champions)
- **Tottenham** (17th place)
- **Leicester City** (18th place - Relegated)
- **Ipswich Town** (19th place - Relegated)
- **Southampton** (20th place - Relegated)

### Biggest Prediction Errors

| Team | Actual Position | Predicted Position | Error |
|------|----------------|-------------------|-------|
| Wolves | 16th | 3rd | 13 positions |
| Manchester City | 3rd | 15th | 12 positions |
| Chelsea | 4th | 14th | 10 positions |
| West Ham | 14th | 4th | 10 positions |
| Newcastle United | 5th | 13th | 8 positions |

### Key Findings

1. **Relegation Zone**: The model perfectly predicted all three relegated teams (Leicester City, Ipswich Town, Southampton)
2. **Championship Winner**: Correctly predicted Liverpool would win the title
3. **Mid-table Volatility**: Greatest prediction errors occurred in mid-table positions (5th-15th)
4. **Top Teams**: Early season form proved less reliable for established top teams like Manchester City and Chelsea
5. **Consistent Teams**: Teams with stable performance (top and bottom of table) were easier to predict

The project successfully demonstrates:
- Machine learning application to sports prediction
- Data-driven analysis of football performance patterns
- Comprehensive visualization of prediction accuracy
- Statistical validation of model performance
- Real-world applicability with 25% exact prediction accuracyachine learning guidance
- Matplotlib community for visualization inspiration
