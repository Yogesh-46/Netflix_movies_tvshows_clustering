# Netflix Movies & TV Shows Clustering

## Project Overview

This project applies **Natural Language Processing (NLP)** and **Unsupervised Machine Learning** techniques to analyze and cluster Netflix Movies and TV Shows based on their content characteristics.

The objective is to discover meaningful content groups that can support recommendation systems, audience segmentation, content acquisition, and marketing strategies.

---

## Business Problem

Streaming platforms such as Netflix contain thousands of titles across multiple genres, languages, and formats.

Manually categorizing content at scale is difficult and time-consuming.

This project aims to automatically identify natural content segments by analyzing:

* Genres
* Directors
* Content Descriptions

The resulting clusters can help stakeholders better understand the content catalog and improve user experience.

---

## Dataset Information

The dataset contains information about Netflix Movies and TV Shows including:

* Title
* Type
* Director
* Cast
* Country
* Release Year
* Rating
* Duration
* Genre
* Description

### Dataset Size

* Records: 7,787
* Features: 12

---

## Project Workflow

### 1. Data Understanding

* Dataset inspection
* Missing value analysis
* Data quality assessment

### 2. Exploratory Data Analysis

* Movies vs TV Shows distribution
* Content growth trends
* Top producing countries
* Ratings analysis
* Genre analysis
* Duration analysis
* Exceptional case analysis

### 3. Data Preprocessing

* Missing value treatment
* Feature engineering
* Text cleaning
* Stopword removal
* Lemmatization

### 4. Feature Extraction

TF-IDF Vectorization

* Max Features: 5000
* Unigrams and Bigrams

### 5. Dimensionality Reduction

TruncatedSVD

* Reduced dimensions from 5000 to 100

### 6. Clustering Algorithms

#### KMeans Clustering

* Number of Clusters: 7
* Silhouette Score: 0.0943

#### Agglomerative Clustering

* Number of Clusters: 7
* Silhouette Score: 0.0706

---

## Cluster Insights

The final KMeans model identified seven major content segments:

| Cluster | Content Category                       |
| ------- | -------------------------------------- |
| 0       | TV Comedies & Kids Entertainment       |
| 1       | Stand-Up Comedy & Comedy Specials      |
| 2       | Action & Adventure Movies              |
| 3       | Children & Family Movies               |
| 4       | Drama, Thriller & International Movies |
| 5       | Documentaries & Reality Content        |
| 6       | International TV Shows & Crime Dramas  |

---

## Model Comparison

| Algorithm                | Silhouette Score |
| ------------------------ | ---------------- |
| KMeans                   | 0.0943           |
| Agglomerative Clustering | 0.0706           |

KMeans achieved the highest Silhouette Score and was selected as the final model.

---

## Business Impact

This solution can support:

### Recommendation Systems

Recommend similar content based on cluster membership.

### Content Acquisition

Identify overrepresented and underrepresented content categories.

### Marketing Campaigns

Create cluster-specific marketing strategies.

### Audience Segmentation

Understand content consumption preferences more effectively.

---

## Future Improvements

* BERT-based embeddings
* Spectral Clustering
* DBSCAN
* User watch-history integration
* Streamlit deployment
* Azure Machine Learning integration

---

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* NLTK

---

## Author

Yogesh Dubey

Aspiring Data Scientist | BI Engineer | Machine Learning Enthusiast
