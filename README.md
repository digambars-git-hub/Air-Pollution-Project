# Air Pollution Project

A comprehensive Streamlit web application for visualizing and predicting air quality data across different cities in India. This interactive dashboard allows users to explore historical pollution trends and make predictions about future air quality levels.

🌐 **Live Application**: [https://air-pollution-project.streamlit.app/](https://air-pollution-project.streamlit.app/)

## Features

### 📊 Data Visualization
- **City-based Analysis**: Select any city from the dataset to view pollution trends
- **Pollutant Selection**: Analyze individual pollutants (SO₂, NO₂, RSPM, SPM) or view all together
- **Date Range Filtering**: Customize the time period for analysis using an interactive slider
- **Monthly Aggregation**: Data is automatically aggregated by month for clearer trend visualization
- **Summary Statistics**: View detailed statistical summaries of pollution levels

### 🤖 Predictive Analytics
- **Future Predictions**: Use machine learning to predict future pollutant levels
- **Random Forest Model**: Powered by scikit-learn's RandomForestRegressor
- **Model Performance Metrics**: View R² score and Mean Squared Error (MSE) for model accuracy
- **Customizable Forecasts**: Select specific year and month for predictions

## Technologies Used

- **Streamlit**: Web application framework
- **Pandas**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning (Random Forest Regressor)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Air-Pollution-Project
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Make sure you have the `cleaned_data.csv` file in the project directory.

2. Run the Streamlit application:
```bash
streamlit run app.py
```

3. The application will open in your default web browser at `http://localhost:8501`

### Using the Dashboard

1. **Visualization Panel**:
   - Select a city from the sidebar dropdown
   - Choose a pollutant to analyze (or select "all" for comparison)
   - Adjust the date range slider to focus on specific time periods
   - Optionally check "Show Summary Statistics" for detailed metrics

2. **Prediction Panel**:
   - Select a city and pollutant for prediction
   - The model will automatically train on available data
   - Review the model accuracy metrics
   - Use the sliders to select a future year and month
   - View the predicted pollution level

## Project Structure

```
Air-Pollution-Project/
├── app.py                 # Main Streamlit application
├── cleaned_data.csv       # Air quality dataset
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
```

## Data

The project uses cleaned air quality data containing:
- **Pollutants**: SO₂ (Sulfur Dioxide), NO₂ (Nitrogen Dioxide), RSPM (Respirable Suspended Particulate Matter), SPM (Suspended Particulate Matter)
- **Geographic Coverage**: Multiple cities across India
- **Time Period**: Historical data from 1990 onwards
- **Data Points**: Location, sampling date, state, and pollution measurements

## Model Details

The prediction model uses:
- **Algorithm**: Random Forest Regressor
- **Features**: Year, month, and other pollutant levels
- **Training**: 80% of data for training, 20% for testing
- **Evaluation**: R² score and Mean Squared Error metrics

## Live Deployment

The application is live and accessible at:
**https://air-pollution-project.streamlit.app/**

You can use the live version without any local installation!

## License

This project is open source and available for educational and research purposes.

## Contributing

Contributions, issues, and feature requests are welcome!

