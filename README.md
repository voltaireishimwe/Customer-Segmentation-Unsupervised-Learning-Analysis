# CUSTOMER SEGMENTATION & UNSUPERVISED LEARNING ANALYSIS

## Overview
This repository contains a comprehensive analysis of customer data using unsupervised learning techniques, specifically focusing on customer segmentation through clustering algorithms. The project demonstrates a complete data science workflow from data loading and exploration to feature engineering and clustering implementation.

## Project Structure
The notebook is organized into two main parts:

### Part 1: Unsupervised Learning Analysis
**Task 1.1: Customer Segmentation with Clustering**

#### Key Components:

1. **Data Loading & Initial Exploration**
   - Loads customer dataset from `./customer/customer_dataset.csv`
   - Dataset contains 500 entries with 11 features
   - Initial exploration shows no missing values
   - Data types include numerical (6), categorical (4), and identifier features

2. **Data Preparation & Feature Engineering**
   - **Missing Value Handling**: Uses median imputation for numerical features and mode imputation for categorical features
   - **Feature Engineering**:
     - `Category_Count`: Count of product categories per customer
     - `Brand_Count`: Count of brands purchased per customer
     - `RFM_Score`: Combined metric using Recency, Frequency, and Monetary value
     - `Engagement_Score`: Combined metric from Website Visits and Email Opens
   - Final dataset shape: 500 rows × 15 columns

3. **Exploratory Data Analysis (EDA)**
   - Analysis of feature distributions
   - Correlation analysis between numerical features
   - Outlier detection and handling
   - Visualization of relationships between key variables

4. **Clustering Implementation**
   - Uses 10 engineered features for segmentation:
     - Demographic: Age
     - Transactional: Frequency, Monetary Value, Recency
     - Behavioral: Website Visits, Email Opens
     - Derived: Category_Count, Brand_Count, RFM_Score, Engagement_Score
   - Multiple clustering algorithms available:
     - KMeans
     - Agglomerative Clustering
     - DBSCAN

## Technical Stack

### Core Libraries
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn, plotly (optional for interactive plots)
- **Machine Learning**: scikit-learn
- **Deep Learning**: TensorFlow/Keras
- **Statistical Analysis**: scipy

### Machine Learning Components
- **Clustering Algorithms**: KMeans, AgglomerativeClustering, DBSCAN
- **Dimensionality Reduction**: PCA, t-SNE
- **Preprocessing**: StandardScaler, LabelEncoder
- **Evaluation Metrics**: silhouette_score, adjusted_rand_score
- **NLP Processing**: Tokenizer, pad_sequences (for text data if needed)

## Dataset Features

### Original Features (11)
- **Identifiers**: Customer_ID
- **Demographic**: Age, Gender, Location
- **Transactional**: Frequency, Monetary Value, Recency
- **Behavioral**: Categories, Brands, Website Visits, Email Opens

### Engineered Features (4)
- Category_Count
- Brand_Count
- RFM_Score
- Engagement_Score

## Methodology

### Data Preprocessing Strategy
- Numerical features standardized using StandardScaler
- Categorical variables one-hot encoded
- Feature engineering to create meaningful composite metrics
- Comprehensive EDA to understand data distributions and relationships

### Clustering Approach
- Multiple algorithms for comparative analysis
- Dimensionality reduction techniques for visualization
- Evaluation using internal (silhouette) and external (adjusted rand) metrics
- Feature selection focused on customer behavior and value metrics

## Business Applications

### Customer Segmentation Use Cases
1. **Targeted Marketing**: Identify high-value customer groups
2. **Personalized Recommendations**: Tailor product suggestions based on segment behavior
3. **Customer Retention**: Focus on at-risk segments
4. **Resource Allocation**: Optimize marketing spend across different segments
5. **Product Development**: Understand different customer preferences

### RFM Analysis Integration
The RFM scoring system enables:
- Identification of most valuable customers
- Detection of customers at risk of churn
- Opportunities for customer reactivation
- Strategic customer lifetime value analysis

## Expected Outcomes
- Clear customer segments with distinct behavioral patterns
- Visualizations showing cluster separation and characteristics
- Actionable insights for marketing strategy
- Framework for ongoing customer segmentation analysis

## Next Steps
The notebook structure suggests potential extensions including:
- Deep learning approaches for customer segmentation
- Time-series analysis of customer behavior
- Integration with recommendation systems
- Deployment of clustering models for real-time segmentation

## Requirements
All required libraries are imported at the beginning, with warnings suppressed for cleaner output. The code is structured for reproducibility and can be easily adapted for similar customer segmentation tasks.

**⭐ Star us on GitHub — /Voltaie Ishimwe**
