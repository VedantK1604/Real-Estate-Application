# The Real Estate Application Using Machine Learning

This project is an advanced end-to-end real estate application designed to assist users in making informed decisions about property prices and recommendations. The application includes features for real estate data analysis, price prediction, and property recommendations. It was built using modern machine learning techniques, web scraping, and an intuitive web interface using **Streamlit**.

## Project Overview
This Real Estate Application provides users with the following functionalities:
- **Analytics**: Detailed insights on real estate data (flats, houses, sectors).
- **Price Prediction**: Predict the prices of properties based on various features like location, size, amenities, etc.
- **Recommendations**: Suggest similar properties based on content-based filtering using price, location advantages, and nearby areas.

The application is designed to offer a smooth and interactive experience through a web-based interface built using **Streamlit**.

## Modules

### 1. Analytics Module
In this module, users can explore comprehensive analytics about properties, including trends in different locations, sector-based property insights, average prices, and more. This allows users to make data-driven decisions while browsing real estate properties.

### 2. Price Prediction Module
This module uses a **Random Forest** regression model with an **R² score of 0.90** to predict property prices. Users can input property details such as location, size, and other features, and the system provides an estimated price based on the model's predictions. The features used for price prediction are carefully selected using feature engineering techniques.

### 3. Recommendation Module
The recommendation engine is based on **content-based filtering** and suggests apartments or properties based on key features like price, location advantages, and proximity to important landmarks. Users receive property recommendations that match their interests based on the input features they provide.

## Data Collection
The data for this project is collected through web scraping using **BeautifulSoup** from **99acres.com**. The data contains details about various apartments, their features, and the surrounding location advantages. The scraping process fetched data points such as property prices, area, number of bedrooms, and amenities.

## Data Preprocessing
The raw data was preprocessed to ensure the model's efficiency and accuracy. Preprocessing steps included:
- **Cleaning**: Removing any irrelevant or duplicated data.
- **Fixing Outliers**: Detecting and handling outliers in the dataset to avoid skewing model predictions.
- **Missing Value Imputation**: Filling in missing values using appropriate strategies.
- **Feature Selection**: Applying feature selection techniques to choose the most relevant features for price prediction and recommendations.

## Modeling

### Price Prediction
The **Random Forest** algorithm was selected for the price prediction task after rigorous testing and model evaluation. The model was trained on features such as:
- Location
- Property size (square feet)
- Number of bedrooms
- Property type (flat, house, etc.)
- Amenities

The model achieved an **R² score of 0.90**, ensuring accurate predictions of property prices based on the input data.

### Recommendation System
For the recommendation module, a **content-based filtering** approach was implemented. The system filters and recommends properties based on key features:
- Price range
- Location advantages (proximity to schools, markets, etc.)
- Nearby locations and amenities

This helps users discover similar properties that match their preferences and interests.

## Technologies Used
- **Python**: Main programming language used for the entire project.
- **Pandas**, **NumPy**: For data manipulation and processing.
- **BeautifulSoup**: For web scraping to gather real estate data from 99acres.com.
- **Streamlit**: To create the user-friendly web interface for interacting with the application.
- **Scikit-learn**: Machine learning library used for building the Random Forest model.
- **Plotly**: For data visualization in the analytics module.
- **Matplotlib**, **Seaborn**: For additional data visualizations.
- **Pickle**: For saving and loading the machine learning model.

## Setup and Installation

To run the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/real-estate-application.git
   cd real-estate-application
   ```

2. **Install Dependencies**:
   Install the required libraries listed in the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   Use the following command to run the Streamlit web application:
   ```bash
   streamlit run Home.py
   ```

4. **Data Scraping**:
   If you'd like to scrape fresh data from 99acres.com, ensure you have the correct scraping scripts and permissions, then run the scraping script.

## Usage

- Navigate to the **Analytics Module** to explore various insights and trends in the real estate market.
- Use the **Price Prediction Module** to get an estimate for a property based on its features.
- Discover similar properties using the **Recommendation Module**.

### Try out the project: https://real-estate-application-fn3q.onrender.com/
