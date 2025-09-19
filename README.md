📊 Customer Feedback Sentiment Analysis

This project analyzes customer product reviews using a lexicon-based sentiment analysis approach.
It helps businesses understand what their customers are saying about their products, identify areas of improvement, and track customer satisfaction.

📁 Project Overview

Input:

A CSV file containing customer reviews (product ID, product name, rating, review text, review date).

Two lexicon files containing lists of positive and negative words/phrases.

Process:

Clean and normalize review text.

Match positive/negative words and phrases.

Handle negations (e.g., “not good” → negative).

Calculate sentiment scores and assign sentiment labels.

Output:

A processed CSV with sentiment results for each review.

A summary CSV with aggregated product-level insights.

An Excel dashboard with processed data and summaries.

Charts (PNG) showing sentiment distribution and average ratings.

⚙️ Technologies Used

Python 3

Pandas – data cleaning & aggregation

Matplotlib – data visualization

OpenPyXL – export to Excel

Regex – text preprocessing

📂 Project Structure
.
├── customer_reviews.csv                # Input reviews dataset
├── positive-words.txt                  # Positive words/phrases lexicon
├── negative-words.txt                  # Negative words/phrases lexicon
├── customer_feedback_sentiment.py      # Main Python script
├── customer_reviews_processed_by_you.csv   # Processed reviews with sentiment
├── summary_by_product_by_you.csv       # Aggregated summary by product
├── customer_feedback_dashboard_by_you.xlsx # Excel dashboard
├── sentiment_distribution_by_you.png   # Sentiment distribution chart
├── avg_rating_by_product_by_you.png    # Avg rating by product chart
└── README.md                           # Project documentation

📝 How It Works

Load Data
The script reads customer_reviews.csv and the lexicon files.

Preprocessing

Convert to lowercase

Remove punctuation/special characters

Normalize spaces

Sentiment Matching

Detect positive/negative words & phrases

Apply negation rules within a small word window

Scoring

Sentiment score = (positive_count - negative_count) / total_tokens

Sentiment label = positive / negative / neutral

Outputs

Review-level results in CSV

Product-level summary in CSV/Excel

Visual insights (PNG charts)

📊 Example Outputs

1. Sentiment Distribution Chart
Bar chart showing counts of positive, neutral, and negative reviews.

2. Average Rating by Product
Bar chart comparing average customer ratings across products.

🚀 How to Run

Clone this repo:

git clone https://github.com/yourusername/customer-feedback-sentiment.git
cd customer-feedback-sentiment


Install dependencies:

pip install pandas matplotlib openpyxl


Place your input files:

customer_reviews.csv → project folder

positive-words.txt and negative-words.txt → project folder

Run the script:

python customer_feedback_sentiment.py


Check the outputs:

CSVs, Excel, and PNG charts will be generated in the same folder.

🧭 Use Cases

Small & Medium Businesses (SMBs):
Track customer satisfaction without expensive software.

Data Analysts:
Practice sentiment analysis with lexicon-based methods.

Students / Learners:
Learn text preprocessing, lexicon usage, and data visualization.

🔮 Next Steps

Add VADER sentiment analysis for comparison.

Build an interactive Streamlit dashboard.

Extend lexicon with domain-specific words (e.g., for e-commerce or services).

👤 Author

Victor Ebere
📧 Email: vecharisma@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/victor-ebere-40a56014a