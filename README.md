# 🎧 Spotify Top 2000 Song Popularity

This project explores the relationship between song characteristics and popularity using Spotify’s **All-Time Top 2000 Tracks** dataset. The goal is to classify songs as either **popular** or **not popular** based on a range of audio features and genre.

## 📊 Dataset

- **Source**: Spotify All-Time Top 2000 Tracks
- **Observations**: 1994 songs
- **Features**:
  - **Numerical**: BPM, Energy, Danceability, Loudness, Valence, Duration, Acousticness, Speechiness, Liveness
  - **Categorical**: Genre (cleaned and grouped into 6 categories)

## 🎯 Problem Statement

We transform the continuous `popularity` variable into a binary classification target:
- **1**: Song is **popular** (popularity ≥ median)
- **0**: Song is **not popular** (popularity < median)

The objective is to predict this binary outcome using various classification algorithms.

## 🧪 Methods

Implemented and compared the following classification models:

- **Logistic Regression**
- **Linear Discriminant Analysis (LDA)**
- **Quadratic Discriminant Analysis (QDA)**
- **k-Nearest Neighbors (KNN)** — with k = 3, 5, 7, 10

### Evaluation Metrics:
- **Accuracy**
- **Sensitivity**
- **Specificity**
- **Runtime**

### Validation Approaches:
- Full dataset
- 50/50 train-test split
- 5-fold Cross-Validation

## 🛠 Tools Used

- **Language**: R
- **Libraries**: `tidyverse`, `MASS`, `class`, `ggplot2`
