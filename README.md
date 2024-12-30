# CryptoClustering

**Classifying Cryptocurrencies Based on Price Fluctuations Using K-Means and PCA**

![CryptoClustering Banner](banner.png) <!-- Optional: Add a relevant banner image -->

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Data](#data)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

**CryptoClustering** is a data analysis project that leverages the K-Means clustering algorithm and Principal Component Analysis (PCA) to classify cryptocurrencies based on their price fluctuations across various timeframes. By analyzing price changes over intervals spanning 24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year, this project aims to uncover patterns and group similar cryptocurrencies together.

## Features

- **Data Normalization**: Utilizes `StandardScaler` to normalize cryptocurrency price data.
- **Optimal Clustering**: Employs the elbow method to determine the optimal number of clusters (`k`).
- **Dimensionality Reduction**: Applies PCA to reduce feature dimensions while retaining significant variance.
- **Visualization**: Generates insightful scatter plots to visualize cryptocurrency clusters.
- **Interpretation**: Analyzes PCA loadings to understand feature influences on principal components.

## Data

The project uses a CSV dataset named `crypto_market_data.csv`, which contains price change percentages of various cryptocurrencies over different timeframes:

- **Timeframes**:
  - 24 Hours (`price_change_percentage_24h`)
  - 7 Days (`price_change_percentage_7d`)
  - 14 Days (`price_change_percentage_14d`)
  - 30 Days (`price_change_percentage_30d`)
  - 60 Days (`price_change_percentage_60d`)
  - 200 Days (`price_change_percentage_200d`)
  - 1 Year (`price_change_percentage_1y`)

- **Index**: `coin_id` (unique identifier for each cryptocurrency)

## Installation

Follow these steps to set up the project locally:

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/CryptoClustering.git
   cd CryptoClustering
