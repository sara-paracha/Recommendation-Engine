# Airbnb Website Recommendation Engine

## Project Overview

This project focuses on extracting rental listing data from Airbnb PDF files using regular expressions and building a recommendation engine. The main objectives are:

- Parse Airbnb rental listings to extract key features
- Clean and preprocess the extracted data
- Perform exploratory data analysis
- Create a recommendation system that filters listings based on user preferences

## Project Structure

The project is implemented in a Jupyter Notebook (AirBnb_website_Recommendation_Engine.ipynb) with the following main components:

### 1\. Data Extraction

- PDF files are processed using pdfminer.six to extract text content
- Regular expressions are applied to extract specific features from each listing:
  - Host information
  - Property ratings and reviews
  - Property details (bedrooms, bathrooms, guest capacity)
  - Amenities and facilities
  - Pricing information
  - House rules (smoking, pets policies)
  - Host status (superhost verification)
  - Cancellation policies

### 2\. Data Processing

- Created a structured DataFrame from extracted features
- Saved the extracted data to a CSV file (features-retrieved-by-SaraParacha.csv)
- Performed data cleaning operations:
  - Removed unnecessary text from columns
  - Handled missing values
  - Converted string data to appropriate data types (integers, floats)
  - Standardized categorical values

### 3\. Exploratory Data Analysis

- Generated heatmaps to visualize missing values and correlations
- Created bar plots to analyze property type distribution
- Developed scatter plots to examine relationships between variables
- Identified that most properties are residential homes
- Discovered strong correlation between bedroom count and rental price

### 4\. Recommendation Engine

- Implemented a user-input based filtering system
- Allows users to specify preferences for:
  - Price range
  - Number of bedrooms and bathrooms
  - Guest capacity
  - Property ratings
  - Specific amenities
- Returns filtered listings that match user criteria

## Technologies Used

- Python
- pandas, numpy for data manipulation
- pdfminer.six for PDF text extraction
- Regular expressions for pattern matching
- seaborn, matplotlib for data visualization
- scikit-learn for data preprocessing

## Key Features Extracted

- Host name and verification status
- Property ratings and number of reviews
- Pricing information
- Property type and size (bedrooms, bathrooms)
- Amenities (WiFi, kitchen, parking, etc.)
- House rules (smoking, pets policies)
- Guest capacity
- Host response rate
- Cancellation policies

## Usage

1. The notebook processes Airbnb PDF files to extract listing features
2. After data cleaning and transformation, exploratory analysis is performed
3. The recommendation engine takes user preferences as input
4. The system returns filtered listings that match the specified criteria

## Insights

- Most Airbnb listings in the dataset are residential homes
- Number of bedrooms shows strong correlation with rental price
- Property ratings have weaker correlation with pricing
- The recommendation system effectively filters properties based on multiple criteria

This project demonstrates comprehensive data extraction, cleaning, analysis, and practical application through a recommendation system that helps users find suitable Airbnb rentals based on their preferences.
