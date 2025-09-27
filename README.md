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

### Analysis and Prediction
The `data_analysis.ipynb` notebook performs:
1. **Historical Analysis**: Examines championship-winning patterns and team performance trends
2. **Feature Engineering**: Creates predictive features from early season data
3. **Model Training**: Trains Random Forest Classifier on historical data
4. **Prediction**: Generates predictions for 2024/25 season based on first 10 games
5. **Validation**: Compares predictions with actual results using comprehensive metrics

### Key Insights
- **Championship Winners**: Manchester City dominated with 6 titles in 10 years
- **Average Points per Match**: Championship winners average 2.41 points per match
- **Prediction Accuracy**: Model provides detailed accuracy metrics and error analysis
- **Visual Comparisons**: Interactive charts show prediction vs actual performance


## Methodology

1. **Data Collection**: Automated scraping of 10 years of Premier League data
2. **Feature Selection**: Key metrics including points per match, goal difference, wins/losses
3. **Model Training**: Random Forest Classifier with 200 estimators
4. **Cross-Validation**: Model validation using historical data
5. **Prediction**: Early season performance scaled to predict full season results
6. **Validation**: Comparison with actual 2024/25 season results

## Results

The project successfully demonstrates:
- Machine learning application to sports prediction
- Data-driven analysis of football performance patterns
- Comprehensive visualization of prediction accuracy
- Statistical validation of model performance

## Future Enhancements

- Real-time data integration for live predictions
- Additional features (player transfers, injuries, form)
- Ensemble methods combining multiple algorithms
- Web application for interactive predictions
- API integration for automated updates


## Acknowledgments

- Data source: [FBRef.com](https://fbref.com) for Premier League statistics
- Scikit-learn documentation for machine learning guidance
- Matplotlib community for visualization inspiration
