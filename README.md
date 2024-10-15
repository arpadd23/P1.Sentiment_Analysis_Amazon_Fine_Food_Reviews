# Sentiment Analysis of Amazon Fine Food Reviews (2024 Update) 📊

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methods](#methods)
- [Results](#results)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Conclusions](#conclusions)
- [Contact](#contact)

## Project Overview
This project performs sentiment analysis on the Amazon Fine Food Reviews dataset using the VADER (Valence Aware Dictionary and Sentiment Reasoner) sentiment analyzer from NLTK. The goal is to extract sentiment scores from customer reviews and analyze how they correlate with the provided star ratings.

## Dataset
**Name:** Amazon Fine Food Reviews  
**Size:** 568,454 reviews  
**Features:**
- Id
- ProductId
- UserId
- ProfileName
- HelpfulnessNumerator
- HelpfulnessDenominator
- Score (1 to 5 stars)
- Time
- Summary
- Text (Review text)  
You can find the dataset on [Kaggle](https://www.kaggle.com).

## Methods
### Data Loading and Exploration
- Loaded a subset of 10,000 reviews for efficiency.
- Performed exploratory data analysis to understand the distribution of ratings.

### Data Preprocessing
- Checked for and handled missing values.
- No significant preprocessing was needed as VADER works well with raw text.

### Sentiment Analysis with VADER
- Utilized NLTK's VADER sentiment analyzer.
- Calculated negative, neutral, positive, and compound sentiment scores for each review.

### Results Visualization
- Plotted distributions of sentiment scores.
- Analyzed correlations between sentiment scores and star ratings.
- Created heatmaps and boxplots for better insights.

### Results

#### Distribution of Ratings
![Distribution of Ratings](https://github.com/arpadd23/P1.Sentiment_Analysis_Amazon_Fine_Food_Reviews/blob/main/Distribution%20of%20Ratings.png?raw=true)

#### Compound Sentiment Scores by Rating
![Compound Sentiment Scores by Rating](https://github.com/arpadd23/P1.Sentiment_Analysis_Amazon_Fine_Food_Reviews/blob/main/Compound%20Sentiment%20Scores%20by%20Rating.png?raw=true)

#### Correlation Between Sentiment Scores and Ratings
![Correlation Between Sentiment Scores and Ratings](https://github.com/arpadd23/P1.Sentiment_Analysis_Amazon_Fine_Food_Reviews/blob/main/Correlation%20Between%20Sentiment%20Scores%20and%20Ratings.png?raw=true)

#### Correlation Heatmap
![Correlation Heatmap](https://github.com/arpadd23/P1.Sentiment_Analysis_Amazon_Fine_Food_Reviews/blob/main/Correlation%20Heatmap.png?raw=true)


**Key Findings:**
- Positive correlation between compound sentiment scores and review ratings.
- Higher-rated reviews have higher positive sentiment scores.
- Lower-rated reviews have higher negative sentiment scores.
- VADER effectively captures the sentiment expressed in customer reviews.

## Usage

To run the analysis:

### Clone the Repository
```bash
git clone https://github.com/yourusername/your-repo-name.git
```

### Navigate to the Project Directory
```bash
cd your-repo-name
```

### Install Dependencies
Ensure you have Python 3.7 or higher. Install the required packages:
```bash
pip install -r requirements.txt
```

### Download the Dataset
Download the Amazon Fine Food Reviews dataset from Kaggle. Place the `Reviews.csv` file into the `data/` directory.

### Run the Notebook
Open and run the Jupyter notebook:
```bash
jupyter notebook sentiment-analysis-python-2024-09.ipynb
```

## Dependencies
- Python 3.7+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK

Install them using:
```bash
pip install pandas numpy matplotlib seaborn nltk
```
## Conclusions
The VADER sentiment analyzer is a powerful tool for quick and effective sentiment analysis on text data.

There's a significant correlation between the sentiment scores calculated by VADER and the actual star ratings given by customers.

This project demonstrates the ability to preprocess data, apply sentiment analysis techniques, and visualize results to extract meaningful insights.

## Contact
For any further questions or project collaborations, feel free to reach out via GitHub.
