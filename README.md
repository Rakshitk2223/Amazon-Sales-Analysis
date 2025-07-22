# Amazon Sales Data Analysis Project

## 📊 Overview
This project provides a comprehensive analysis of Amazon sales data, focusing on product pricing, ratings, categories, and customer reviews. The analysis includes data cleaning, exploratory data analysis (EDA), and visualizations to extract meaningful insights from the dataset.

## 📁 Project Structure
```
Amazon Sales Analysis/
├── amazon.csv              # Raw dataset
├── SalesAnalysis.ipynb     # Main Jupyter notebook with analysis
├── Requirements.txt        # Python dependencies
└── README.md              # Project documentation
```

## 📋 Dataset Information
- **Total Products**: 1,465
- **Columns**: 16
- **Size**: 8.65 MB
- **Missing Values**: Only 2 missing values in rating_count column (0.14%)
- **No Duplicate Records**

### Dataset Columns:
- `product_id` - Unique identifier for each product
- `product_name` - Name of the product
- `category` - Product category hierarchy
- `discounted_price` - Current selling price
- `actual_price` - Original price before discount
- `discount_percentage` - Percentage discount offered
- `rating` - Product rating (1-5 scale)
- `rating_count` - Number of ratings received
- `about_product` - Product description
- `user_id` - Unique identifier for reviewers
- `user_name` - Reviewer name
- `review_id` - Unique identifier for reviews
- `review_title` - Review headline
- `review_content` - Full review text
- `img_link` - Product image URL
- `product_link` - Product page URL

## 🔧 Requirements & Setup

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab

### Installation
1. Clone or download this repository
2. Install required packages:
```bash
pip install -r Requirements.txt
```

### Required Libraries
```
pandas                 # Data manipulation and analysis
numpy                  # Numerical computing
matplotlib             # Basic plotting
seaborn               # Statistical data visualization
plotly                # Interactive visualizations
scikit-learn          # Machine learning library
scipy                 # Scientific computing
notebook              # Jupyter notebook
jupyterlab            # JupyterLab interface
openpyxl              # Excel file support
wordcloud             # Text visualization
textblob              # Text processing and sentiment analysis
nltk                  # Natural language processing
statsmodels           # Statistical modeling
requests              # HTTP library
beautifulsoup4        # Web scraping
```

## 📈 Analysis Highlights

### Key Findings:

#### 💰 Pricing Analysis
- **Average Discounted Price**: ₹3,125.31
- **Average Actual Price**: ₹5,444.99
- **Average Discount**: 47.7% (Maximum: 94%)
- **Price Range**: ₹39 - ₹77,990

#### ⭐ Rating Analysis
- **Average Rating**: 4.10/5.0
- **Rating Range**: 2.0 - 5.0
- **Total Reviews**: ~26.8 million across all products
- **Average Reviews per Product**: 18,296

#### 🏷️ Product Categories (Top 5)
1. **USB Cables** - 233 products (15.9%)
2. **Smart Watches** - 76 products (5.2%)
3. **Smartphones** - 68 products (4.6%)
4. **Smart Televisions** - 63 products (4.3%)
5. **In-Ear Headphones** - 52 products (3.6%)

## 📊 Visualizations Included

The notebook includes comprehensive visualizations:

1. **Price Distribution Histogram** - Shows distribution of discounted prices
2. **Rating Distribution Bar Chart** - Product rating frequency
3. **Discount Percentage Distribution** - Distribution of discount percentages
4. **Top Product Categories** - Most popular product categories
5. **Summary Statistics Table** - Key metrics overview

## 🚀 How to Run the Analysis

1. **Open Jupyter Notebook**:
```bash
jupyter notebook SalesAnalysis.ipynb
```

2. **Run Cells Sequentially**:
   - Cell 1-2: Import libraries and load data
   - Cell 3-4: Basic data exploration
   - Cell 5-6: Data cleaning and type conversion
   - Cell 7-8: Missing values and duplicates analysis
   - Cell 9-10: Categorical data analysis
   - Cell 11-12: Comprehensive price and rating analysis
   - Cell 13: Visualizations and summary statistics

## 📝 Analysis Workflow

### 1. Data Loading & Basic Information
- Load CSV data using pandas
- Check dataset shape, memory usage, and column information
- Display basic statistics

### 2. Data Quality Assessment
- Identify missing values and duplicates
- Analyze data types and formats
- Handle data inconsistencies

### 3. Data Cleaning & Preprocessing
- Convert price columns (remove ₹ symbol and commas)
- Clean rating data (handle special characters)
- Convert percentage and count columns to numeric
- Create clean versions of key columns

### 4. Exploratory Data Analysis (EDA)
- Statistical summary of numerical columns
- Category distribution analysis
- Price and rating correlations
- Product performance metrics

### 5. Data Visualization
- Multiple subplot charts for comprehensive overview
- Interactive plots using matplotlib and seaborn
- Summary statistics table

## 🔍 Potential Use Cases

This analysis can be extended for:

- **Price Optimization**: Analyze optimal pricing strategies
- **Sentiment Analysis**: Process review content for sentiment insights
- **Recommendation Systems**: Build product recommendation engines
- **Market Research**: Understand category performance and trends
- **Competitive Analysis**: Compare products within categories
- **Customer Segmentation**: Analyze user behavior patterns
- **Predictive Modeling**: Forecast sales or ratings

## 🤝 Contributing

Feel free to contribute to this project by:
- Adding new analysis techniques
- Improving visualizations
- Extending the dataset
- Optimizing code performance
- Adding machine learning models

## 📄 License

This project is for educational and analysis purposes. Please ensure you have appropriate rights to use the Amazon sales dataset.

## 📞 Contact

For questions or suggestions regarding this analysis, please feel free to reach out or create an issue in the repository.

---

**Note**: This analysis is based on a sample Amazon sales dataset and is intended for educational purposes. Results should not be used for commercial decisions without proper validation and additional data sources.

**Result** - 