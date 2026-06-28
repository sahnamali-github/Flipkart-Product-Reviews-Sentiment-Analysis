# 📊 Flipkart Product Reviews Sentiment Analysis

A Natural Language Processing (NLP) project that analyzes customer reviews from Flipkart products to understand overall customer sentiment using **VADER Sentiment Analysis**. The project performs text preprocessing, exploratory data analysis, sentiment scoring, and visualization through interactive charts and word clouds.

---

## 📌 Overview

Customer reviews contain valuable insights about product quality and user satisfaction. This project leverages Natural Language Processing (NLP) techniques to clean and analyze review text, identify sentiment polarity, and visualize customer opinions.

The workflow includes:

* Text preprocessing and normalization
* Stopword removal and stemming
* Rating distribution analysis
* Word Cloud generation
* Sentiment analysis using VADER
* Overall sentiment aggregation

---

## 🚀 Features

* ✅ Automatic review text cleaning
* ✅ Stopword removal using NLTK
* ✅ Snowball stemming
* ✅ Rating distribution visualization
* ✅ Interactive Pie Chart with Plotly
* ✅ Word Cloud generation
* ✅ Positive, Negative and Neutral sentiment scoring
* ✅ Overall sentiment prediction

---

## 📂 Dataset

The project uses a publicly available Flipkart laptop reviews dataset containing:

| Column       | Description          |
| ------------ | -------------------- |
| Product_name | Name of the product  |
| Review       | Customer review text |
| Rating       | Product rating (1–5) |

Dataset Source:

https://raw.githubusercontent.com/amankharwal/Website-data/master/flipkart_reviews.csv

---

## 🛠️ Technologies Used

* Python
* Pandas
* NLTK
* Plotly
* Matplotlib
* Seaborn
* WordCloud
* Regular Expressions (Regex)

---

## 📖 Project Workflow

### 1. Data Loading

The dataset is imported using Pandas and checked for missing values.

```python
data = pd.read_csv(...)
```

---

### 2. Data Cleaning

Each review undergoes preprocessing including:

* Convert text to lowercase
* Remove URLs
* Remove HTML tags
* Remove punctuation
* Remove digits
* Remove stopwords
* Apply Snowball stemming

This improves text quality before sentiment analysis.

---

### 3. Exploratory Data Analysis

Customer ratings are visualized using an interactive donut chart.

Example:

* ⭐⭐⭐⭐⭐
* ⭐⭐⭐⭐
* ⭐⭐⭐
* ⭐⭐
* ⭐

This provides an overview of rating distribution.

---

### 4. Word Cloud

Frequently occurring words are displayed using a Word Cloud to highlight commonly discussed terms.

---

### 5. Sentiment Analysis

The project uses NLTK's **VADER (Valence Aware Dictionary and sEntiment Reasoner)** to compute sentiment scores for every review.

Each review receives:

* Positive Score
* Negative Score
* Neutral Score

Example:

| Review           | Positive | Negative | Neutral |
| ---------------- | -------- | -------- | ------- |
| Good performance | 0.744    | 0.000    | 0.256   |
| Best product     | 0.512    | 0.000    | 0.488   |

---

### 6. Overall Sentiment

The individual sentiment scores are aggregated across the dataset.

Example output:

```
Positive : 923.79

Negative : 96.99

Neutral : 1283.22
```

Since the Neutral score is highest, the overall dataset sentiment is classified as:

> **Neutral 🙂**

---

## 📊 Visualizations

The project generates the following visualizations:

* 📈 Rating Distribution (Interactive Plotly Pie Chart)
* ☁️ Word Cloud
* 📊 Sentiment Score Summary

---

## 📁 Project Structure

```
Flipkart-Sentiment-Analysis/
│
├── flipkart_reviews.csv
├── sentiment_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Flipkart-Sentiment-Analysis.git
```

Move into the project directory:

```bash
cd Flipkart-Sentiment-Analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Download the required NLTK resources:

```python
import nltk

nltk.download("stopwords")
nltk.download("vader_lexicon")
```

Run the notebook or Python script.

---

## 📦 Required Libraries

```text
pandas
matplotlib
seaborn
plotly
nltk
wordcloud
```

Install manually if needed:

```bash
pip install pandas matplotlib seaborn plotly nltk wordcloud
```

---

## 💡 Sample Output

```
Positive Score : 923.79

Negative Score : 96.99

Neutral Score : 1283.22

Overall Sentiment :

Neutral 🙂
```

---

## 🔮 Future Improvements

* Add sentiment distribution charts
* Perform product-wise sentiment analysis
* Build an interactive dashboard using Streamlit
* Compare sentiment with product ratings
* Train Machine Learning and Deep Learning sentiment classifiers
* Support multilingual customer reviews

---

## 🎯 Learning Outcomes

This project demonstrates practical experience with:

* Natural Language Processing (NLP)
* Text preprocessing
* Sentiment Analysis
* Data Visualization
* Exploratory Data Analysis (EDA)
* Python data science libraries
* Real-world customer review analytics

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## ⭐ If you found this project useful

Consider giving the repository a **⭐ Star** to support the project and help others discover it.
