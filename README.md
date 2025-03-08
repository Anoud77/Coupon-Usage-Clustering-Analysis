# Coupon Usage Clustering Analysis

This project involves analyzing coupon usage data for different customer segments, grouping customers based on their coupon usage patterns, gender, and city of residence. The analysis leverages clustering techniques to identify distinct customer groups, allowing for targeted marketing and offer strategies. Each customer group is analyzed based on gender distribution, city distribution, and average coupon usage to provide actionable recommendations.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Model Approach](#model-approach)
3. [Cluster Analysis](#cluster-analysis)
4. [Recommendations](#recommendations)
5. [Evaluation Metrics](#evaluation-metrics)
6. [Key Findings](#key-findings)
7. [Installation](#installation)
8. [Usage](#usage)

## Project Overview

This project uses clustering techniques to segment customers based on their coupon usage. The data includes customer attributes such as gender, city, and coupon usage frequency. The goal is to identify customer clusters that share similar behavior, enabling more effective marketing strategies and targeted offers.

## Model Approach

We applied a clustering algorithm to group customers based on their coupon usage and demographics. The steps taken include:

1. **Data Preprocessing**:
   - Cleaning and preparing the data, including handling missing values and encoding categorical variables.
   - Normalizing the coupon usage data for consistent scaling across clusters.

2. **Clustering Algorithm**:
   - K-means clustering was used to group customers into different segments based on coupon usage patterns.
   - Each cluster was analyzed in terms of gender distribution and city location.

3. **Cluster Profiling**:
   - For each cluster, the average coupon usage, gender distribution, and city distribution were calculated.
   - Based on these insights, we derived actionable recommendations for each group.

## Cluster Analysis

### Cluster 0
- **Size**: 121
- **Average Coupon Usage**: 3.95
- **Gender Distribution**: 100% Female
- **City Distribution**: Predominantly from Damanhur, Sohag, Qena, and other cities.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase customer loyalty.
  - Focus on female customers and cities: Damanhur, Sohag, Qena, Fayyum, Beni Suef, Damietta, Aswan, Zagazig, Minya, Ismailia, Asyut, Tanta, El-Mahalla El-Kubra.

### Cluster 1
- **Size**: 67
- **Average Coupon Usage**: 8.49
- **Gender Distribution**: 100% Female
- **City Distribution**: Includes cities like Asyut, Aswan, Ismailia, Zagazig, Alexandria, Cairo, and others.

**Recommendations**:
  - Provide higher-value or exclusive coupons to maintain customer engagement.
  - Target offers to female customers and focus on cities: Asyut, Aswan, Ismailia, Zagazig, Alexandria, Damanhur, and more.

### Cluster 2
- **Size**: 111
- **Average Coupon Usage**: 3.76
- **Gender Distribution**: 100% Male
- **City Distribution**: Predominantly from Port Said, Giza, Shubra El-Kheima, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on male customers and cities: Port Said, Giza, Shubra El-Kheima, Suez, Cairo, Mansoura, Alexandria, and more.

### Cluster 3
- **Size**: 96
- **Average Coupon Usage**: 4.57
- **Gender Distribution**: 100% Male
- **City Distribution**: Includes cities like Aswan, Qena, Sohag, Beni Suef, Damanhur, Damietta, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on male customers and cities: Aswan, Qena, Sohag, Beni Suef, Damanhur, Damietta, and more.

### Cluster 4
- **Size**: 88
- **Average Coupon Usage**: 8.63
- **Gender Distribution**: 100% Male
- **City Distribution**: Predominantly from Fayyum, Ismailia, El-Mahalla El-Kubra, Suez, Port Said, and others.

**Recommendations**:
  - Provide higher-value or exclusive coupons to maintain engagement.
  - Focus on male customers and cities: Fayyum, Ismailia, El-Mahalla El-Kubra, Suez, Port Said, and others.

### Cluster 5
- **Size**: 87
- **Average Coupon Usage**: 4.16
- **Gender Distribution**: 100% Female
- **City Distribution**: Includes cities like Aswan, Zagazig, Damanhur, Qena, Minya, Sohag, Fayyum, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on female customers and cities: Aswan, Zagazig, Damanhur, Qena, Minya, Sohag, Fayyum, and more.

### Cluster 6
- **Size**: 108
- **Average Coupon Usage**: 4.63
- **Gender Distribution**: 100% Female
- **City Distribution**: Includes cities like Cairo, Port Said, Shubra El-Kheima, Tanta, Suez, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on female customers and cities: Cairo, Port Said, Shubra El-Kheima, Tanta, Suez, and others.

### Cluster 7
- **Size**: 108
- **Average Coupon Usage**: 4.06
- **Gender Distribution**: 100% Male
- **City Distribution**: Includes cities like Giza, Cairo, El-Mahalla El-Kubra, Suez, Mansoura, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on male customers and cities: Giza, Cairo, El-Mahalla El-Kubra, Suez, Mansoura, and others.

### Cluster 8
- **Size**: 106
- **Average Coupon Usage**: 4.84
- **Gender Distribution**: 100% Male
- **City Distribution**: Predominantly from Qena, Sohag, Minya, Damanhur, Damietta, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on male customers and cities: Qena, Sohag, Minya, Damanhur, Damietta, and others.

### Cluster 9
- **Size**: 108
- **Average Coupon Usage**: 4.85
- **Gender Distribution**: 100% Female
- **City Distribution**: Predominantly from Cairo, Alexandria, Shubra El-Kheima, Giza, Port Said, and others.

**Recommendations**:
  - Offer more frequent, smaller-value coupons to increase loyalty.
  - Focus on female customers and cities: Cairo, Alexandria, Shubra El-Kheima, Giza, Port Said, and others.

## Evaluation Metrics

The clustering model was evaluated based on:

- **Silhouette Score**: Measures the quality of the clusters by assessing how similar objects are within the same cluster and how distinct the clusters are from each other.
- **Average Coupon Usage**: Represents the mean number of coupon usages for each customer group, used as a key indicator of customer engagement.
- **City Distribution**: Assesses how well the customers are distributed across different cities, providing insights into regional preferences.

## Key Findings

- **Gender Segmentation**: Most clusters exhibit a strong gender bias (either male or female), which should be considered when targeting marketing efforts.
- **City Preferences**: Certain cities are overrepresented in particular clusters, indicating regional preferences that can be leveraged for localized offers.
- **Coupon Usage Patterns**: Some clusters show significantly higher coupon usage, suggesting that these customers may be more engaged and thus deserving of exclusive or higher-value offers.

## Installation

To get started with this project, you need Python 3.x and the following libraries:

```bash
pip install pandas numpy scikit-learn matplotlib
