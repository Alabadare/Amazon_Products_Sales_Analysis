# Amazon Product Data Analysis
## Project Overview
This project analyzes Amazon product listings to uncover pricing trends, customer sentiment, and key drivers of product ratings across different categories.

 ## Objectives
	•	Analyze factors influencing product ratings
	•	Understand customer sentiment from reviews
	•	Identify category-level performance trends
	•	Build a predictive model for product ratings

## Data Preprocessing
	•	Converted price and rating columns to numeric (removed ₹, commas)
	•	Handled missing values using median imputation
	•	Simplified product categories
	•	Engineered features:
	•	Product description length
	•	Word count

## Exploratory Data Analysis (EDA)
	•	Dataset: 1465 products, 16 features
	•	Ratings mostly between 3.9 – 4.3
	•	Strong correlation:
	•	Actual price ↔ Discounted price
	•	Weak relationships:
	•	Discount vs Rating (~ -0.15)
	•	Description length vs Rating (~ 0.02)
## Category Insights
	•	Highest discounts: Home Improvement, Electronics
	•	Highest ratings: Musical Instruments, Home Improvement
	•	Most engagement: Computers & Accessories, Electronics

## Sentiment Analysis
	•	Tool: TextBlob
	•	Majority of reviews are positive
	•	Reviews are mostly subjective
	•	Common themes:
	•	Product quality
	•	Value for money

## Predictive Modeling
Model: Random Forest Regressor
Features used:
	•	Pricing variables
	•	Category
	•	Rating count
	•	Text features
	•	Sentiment scores
 Performance
	•	MAE: 0.1669
	•	R²: 0.2296
 Indicates moderate predictive power, suggesting other external factors influence ratings.

 ## Key Insights
	•	Discounts have minimal impact on ratings
	•	Product quality drives customer satisfaction
	•	Customer sentiment is mostly positive
	•	Category performance varies significantly
	•	Product description length has no significant effect

 ## Recommendations
	•	✔ Focus on product quality over discounts
	•	✔ Leverage positive customer reviews
	•	✔ Improve low-performing categories
	•	✔ Encourage more customer reviews for engagement

 ## Tools & Technologies
	•	Python (Pandas, NumPy, Scikit-learn)
	•	Matplotlib / Seaborn
	•	TextBlob (NLP)

 ## Project Structure

project/
│
├── data/
├── notebooks/
├── models/
├── plots/
└── README.md

## Conclusion
Customer satisfaction is driven more by product quality and experience than pricing strategies. Improving product value and leveraging customer feedback can significantly enhance performance.
