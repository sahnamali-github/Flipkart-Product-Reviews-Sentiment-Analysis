# 📊 Flipkart Product Reviews Sentiment Analysis

A Natural Language Processing (NLP) project that analyzes customer reviews from Flipkart products to understand overall customer sentiment using **VADER Sentiment Analysis**. The project performs text preprocessing, sentiment scoring, and data visualization to extract meaningful insights from customer feedback.

---

## 📌 Overview

Customer reviews provide valuable insights into product quality, customer satisfaction, and user experience. This project explores how **Natural Language Processing (NLP)** techniques can be used to analyze product reviews, classify sentiment, and summarize overall customer opinion.

The workflow includes cleaning raw review text, performing sentiment analysis using **VADER**, and visualizing review patterns through interactive charts and word clouds.

---

## 🚀 Features

* 📝 Text preprocessing and cleaning
* 🧹 Stopword removal and stemming using NLTK
* 😊 Sentiment analysis using VADER
* 📊 Product rating distribution visualization
* ☁️ Word Cloud generation
* 📈 Overall sentiment summary
* 🔍 Exploratory Data Analysis (EDA)

---

## 📂 Dataset

The project uses a publicly available Flipkart product reviews dataset containing customer reviews and ratings.

| Column       | Description          |
| ------------ | -------------------- |
| Product_name | Name of the product  |
| Review       | Customer review text |
| Rating       | Product rating (1–5) |

The dataset is loaded directly from a public GitHub repository using Pandas.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NLTK
* Matplotlib
* Seaborn
* Plotly
* WordCloud
* Regular Expressions (Regex)

---

## 🔄 Project Workflow

### 1. Load the Dataset

The dataset is imported into a Pandas DataFrame and checked for missing values to ensure data quality before analysis.

---

### 2. Text Preprocessing

Each customer review undergoes several preprocessing steps to improve text quality:

* Convert text to lowercase
* Remove URLs
* Remove HTML tags
* Remove punctuation
* Remove special characters and numbers
* Remove English stopwords
* Apply Snowball stemming

These steps help standardize the text and improve sentiment analysis accuracy.

---

### 3. Exploratory Data Analysis

The distribution of product ratings is visualized using an interactive Plotly donut chart, providing an overview of customer rating patterns.

---

### 4. Word Cloud Generation

A Word Cloud is generated to highlight the most frequently occurring words across customer reviews, making it easier to identify common topics and themes.

---

### 5. Sentiment Analysis

The cleaned reviews are analyzed using **VADER (Valence Aware Dictionary and sEntiment Reasoner)** from the NLTK library.

For each review, VADER calculates:

* Positive score
* Negative score
* Neutral score

These scores provide a sentiment profile for every customer review.

---

### 6. Overall Sentiment Evaluation

The individual sentiment scores are aggregated across all reviews to determine the overall sentiment of the dataset.

Example output:

```text id="g8s0t2"
Positive Score : 923.80

Negative Score : 96.99

Neutral Score : 1283.22

Overall Sentiment : Neutral 🙂
```

---

## 📊 Output

The project generates:

* 📈 Rating Distribution (Interactive Plotly Chart)
* ☁️ Word Cloud of Customer Reviews
* 😊 Positive, Negative, and Neutral Sentiment Scores
* 📊 Overall Dataset Sentiment

---

## 📁 Project Structure

```text id="8huzzw"
Flipkart-Product-Reviews-Sentiment-Analysis/
│
├── sentiment_analysis.ipynb
├── flipkart_reviews.csv
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash id="y6eszh"
git clone https://github.com/yourusername/Flipkart-Product-Reviews-Sentiment-Analysis.git
```

Navigate to the project directory:

```bash id="3fjlwm"
cd Flipkart-Product-Reviews-Sentiment-Analysis
```

Install the required dependencies:

```bash id="v0vqgb"
pip install -r requirements.txt
```

Download the required NLTK resources:

```python id="17c6p9"
import nltk

nltk.download("stopwords")
nltk.download("vader_lexicon")
```

Run the notebook or Python script.

---

## 📦 Required Libraries

```text id="u5i6ck"
pandas
matplotlib
seaborn
plotly
nltk
wordcloud
```

Or install them manually:

```bash id="5w25l8"
pip install pandas matplotlib seaborn plotly nltk wordcloud
```

---

## 💻 Sample Output

```text id="zwpdzg"
Positive Score : 923.80

Negative Score : 96.99

Neutral Score : 1283.22

Overall Sentiment : Neutral 🙂
```

---

## 📚 Learning Outcomes

Through this project, I explored:

* Natural Language Processing (NLP)
* Text preprocessing techniques
* Stopword removal and stemming
* Sentiment Analysis using VADER
* Exploratory Data Analysis (EDA)
* Data Visualization using Plotly and Matplotlib
* Word Cloud generation
* Python for data analysis

---

## 🔮 Future Improvements

* Train machine learning models for sentiment classification
* Compare VADER with transformer-based sentiment models
* Perform product-wise sentiment analysis
* Build an interactive dashboard using Streamlit
* Analyze sentiment trends across different rating levels
* Deploy the application as a web-based sentiment analysis tool

---

## 🎓 About This Project

This project was developed as part of my learning journey to explore **Natural Language Processing (NLP)** and **sentiment analysis** using Python. It demonstrates practical implementation of text preprocessing, sentiment scoring with VADER, and data visualization techniques to analyze customer reviews and extract meaningful insights.
