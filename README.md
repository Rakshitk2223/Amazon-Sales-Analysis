# Amazon Sales Data Analysis Project

## 📊 Overview
This project provides a comprehensive analysis of Amazon sales data, featuring advanced data science techniques including outlier detection, correlation analysis, missing value imputation, and business intelligence dashboard preparation. The analysis goes beyond basic EDA to provide actionable insights for e-commerce decision-making.

## 📁 Project Structure
```
Amazon Sales Analysis/
├── amazon.csv                # Raw dataset (1,465 products)
├── CleanedAmazonSales.csv   # Processed dataset for Tableau/BI tools
├── README.md                # Project documentation (this file)
├── Requirements.txt         # Python dependencies (enhanced with 19 libraries)
└── SalesAnalysis.ipynb      # Main Jupyter notebook with comprehensive analysis
```

## 📋 Dataset Information
- **Total Products**: 1,465 unique products
- **Total Reviews**: ~26.8 million across all products
- **Original Columns**: 16 columns
- **Enhanced Columns**: 21 columns (including 5 cleaned numerical columns)
- **Dataset Size**: 8.65 MB
- **Data Quality**: High quality with minimal missing values (successfully handled)
- **Categories**: 1,351 unique products across multiple categories
- **Users**: 1,194 unique reviewers
- **No Duplicate Records**: Verified clean dataset

### Original Dataset Columns:
- `product_id` - Unique identifier for each product
- `product_name` - Name of the product
- `category` - Product category hierarchy (pipe-separated)
- `discounted_price` - Current selling price (₹)
- `actual_price` - Original price before discount (₹)
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

### Enhanced Cleaned Columns:
- `discounted_price_clean` - Numerical version of discounted price
- `actual_price_clean` - Numerical version of actual price
- `discount_percentage_clean` - Numerical version of discount percentage
- `rating_clean` - Cleaned rating values (handled "|" separators)
- `rating_count_clean` - Numerical version of rating count

## 🔧 Requirements & Setup

### Prerequisites
- Python 3.7+ (recommended: Python 3.9+)
- Jupyter Notebook or JupyterLab
- 4GB+ RAM (for large dataset processing)

### Installation
1. Clone or download this repository
2. Install required packages:
```bash
pip install -r Requirements.txt
```

### Enhanced Required Libraries
```
pandas>=1.5.0          # Data manipulation and analysis
numpy>=1.21.0          # Numerical computing
matplotlib>=3.5.0      # Basic plotting and visualization
seaborn>=0.11.0        # Statistical data visualization
plotly>=5.0.0          # Interactive visualizations
scikit-learn>=1.1.0    # Machine learning library
scipy>=1.7.0           # Scientific computing
notebook>=6.4.0        # Jupyter notebook
jupyterlab>=3.0.0      # JupyterLab interface
openpyxl>=3.0.0        # Excel file support
wordcloud>=1.8.0       # Text visualization
textblob>=0.17.0       # Text processing and sentiment analysis
nltk>=3.7              # Natural language processing
statsmodels>=0.13.0    # Statistical modeling
requests>=2.28.0       # HTTP library
beautifulsoup4>=4.11.0 # Web scraping
warnings               # Built-in warning handling
datetime               # Built-in date/time handling
```

## 📈 Advanced Analysis Highlights

### 💰 Comprehensive Pricing Analysis
- **Average Discounted Price**: ₹3,125.31
- **Median Discounted Price**: ₹799.00
- **Average Actual Price**: ₹5,444.99
- **Median Actual Price**: ₹1,650.00
- **Average Discount**: 47.7% (Maximum: 94%)
- **Price Range**: ₹39 - ₹77,990
- **Savings Analysis**: Average savings of ₹2,319 per product

### ⭐ Rating & Review Intelligence
- **Average Rating**: 4.10/5.0
- **Median Rating**: 4.10/5.0
- **Rating Range**: 2.0 - 5.0
- **Total Reviews**: ~26.8 million across all products
- **Average Reviews per Product**: 18,296
- **Median Reviews per Product**: 5,179
- **Review Volume**: Ranges from 2 to 426,973 reviews per product

### 🏷️ Product Category Analysis (Top 10)
1. **USB Cables** - 233 products (15.9%)
2. **Smart Watches** - 76 products (5.2%)
3. **Smartphones** - 68 products (4.6%)
4. **Smart Televisions** - 63 products (4.3%)
5. **In-Ear Headphones** - 52 products (3.6%)
6. **Remote Controls** - 49 products (3.3%)
7. **Mixer Grinders** - 27 products (1.8%)
8. **Computer Mice** - 24 products (1.6%)
9. **HDMI Cables** - 24 products (1.6%)
10. **Dry Irons** - 24 products (1.6%)

### 📊 Data Quality & Statistical Analysis
- **Outlier Detection**: Advanced IQR-based outlier identification
  - Price outliers: 14.81% (legitimate premium products)
  - Review outliers: 9.62% (viral/bestseller products)
- **Missing Value Handling**: 
  - Mean imputation for numerical columns
  - Mode imputation for categorical columns
- **Correlation Analysis**: Strong correlation (0.962) between actual and discounted prices
- **Data Validation**: Comprehensive filtering of invalid values

### 🎯 Record-Breaking Products
- **Highest Discount**: 94% on USB-C adapter (₹4,999 → ₹294)
- **Most Expensive**: Sony 65" 4K TV at ₹139,900
- **Most Reviewed**: AmazonBasics HDMI Cable with 426,973 reviews
- **Perfect Rating**: REDTECH USB-C Cable (5.0/5.0 with 18,296+ reviews)

## 📊 Advanced Visualizations Portfolio

### Dashboard 1: Initial Analysis Overview
1. **Price Distribution Histogram** - Right-skewed distribution analysis
2. **Rating Distribution Bar Chart** - Customer satisfaction patterns
3. **Discount Percentage Distribution** - Promotional strategy insights
4. **Top Product Categories** - Market segment analysis

### Dashboard 2: Maximum Values Analysis
5. **Top 10 Products by Discount %** - Clearance and promotional insights
6. **Top 10 Most Expensive Products** - Premium market analysis
7. **Top 10 Most Reviewed Products** - Viral product identification
8. **Top 10 Highest Rated Products** - Quality excellence (100+ reviews filter)

### Dashboard 3: Statistical Analysis
9. **Outlier Detection Box Plots** - IQR-based statistical analysis
10. **Correlation Heatmap** - Variable relationship mapping
11. **Pair Plot Analysis** - Multi-variable relationship visualization
12. **Distribution Analysis** - Statistical distribution with outlier bounds

## � Enhanced Analysis Workflow

### **Phase 1: Data Foundation (Cells 1-7)**
- **Import & Setup**: Load 19 specialized libraries
- **Data Loading**: Import 1,465 product records
- **Basic Exploration**: Shape, memory usage, column analysis
- **Initial Preview**: Sample data examination

### **Phase 2: Data Quality & Cleaning (Cells 8-14)**
- **Missing Value Analysis**: Comprehensive gap identification
- **Data Type Examination**: Format validation and sion
- **Categorical Analysis**: Category hierarchy exploration
- **Data Cleaning**: Currency symbol removal, numeric conversion
- **Missing Value Imputation**: Statistical mean/mode filling

### **Phase 3: Advanced Statistical Analysis (Cells 15-18)**
- **Outlier Detection**: IQR method with data filtering
- **Distribution Analysis**: Statistical validity verification
- **Correlation Analysis**: Variable relationship mapping
- **Pair Plot Generation**: Multi-dimensional visualization

### **Phase 4: Business Intelligence (Cells 19-22)**
- **Maximum Value Analysis**: Record identification
- **Performance Metrics**: Top performer analysis
- **Dashboard Creation**: Business-ready visualizations
- **Data Export**: Tableau/BI tool preparation

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

---

**Note**: This analysis is based on a sample Amazon sales dataset and is intended for educational purposes. Results should not be used for commercial decisions without proper validation and additional data sources.
