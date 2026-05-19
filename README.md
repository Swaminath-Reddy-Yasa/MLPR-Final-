# MLPR-Final-
Pre- release Movie Success Prediction
# Movie Success Prediction (Hollywood and Indian Cinema)

## Overview

This project focuses on predicting the success of movies using machine learning techniques. It analyzes both Hollywood and Indian film datasets and builds predictive models based on financial, temporal, and popularity-related features.

---

## Datasets

* Hollywood dataset (inflation-adjusted)
* Indian movies dataset

### Data Cleaning

* Handled missing values (minimal after manual correction)
* Removed duplicate entries (same title and release year)
* Encoded categorical variables such as genre and language

---

## Feature Engineering

The following features were engineered to improve model performance:

* Director success (based on past performance using ROI)
* Actor star power
* Producer/production company success
* Music director popularity (for Indian dataset)
* Release month extracted from release date

---

## Data Enrichment

Wikipedia links were added for each movie using an API-based pipeline:

TMDB ID → Wikidata → Wikipedia

* Extracted `wikidata_id` using TMDB API
* Retrieved Wikipedia page title from Wikidata
* Constructed the corresponding Wikipedia URL

---

## Models Used

* Logistic Regression
* Random Forest (best performing model)
* Additional baseline models

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

---

## Results

* Random Forest achieved the best overall performance
* Feature engineering significantly improved prediction accuracy

---

## Project Structure

```id="3s2n7u"
project/
│── data/
│   ├── raw/
│   ├── processed/
│
│── notebooks/
│── src/
│── results/
│── README.md
│── requirements.txt
```

---

## How to Run

1. Install dependencies:

```id="6q12qg"
pip install -r requirements.txt
```

2. Run the notebooks or scripts for:

* Data preprocessing
* Feature engineering
* Model training

---

## Notes

* API keys have been removed for security reasons
* Large datasets may not be included due to GitHub size limitations

---

## Conclusion

This project demonstrates that combining feature engineering with machine learning techniques can effectively predict movie success across different film industries.
