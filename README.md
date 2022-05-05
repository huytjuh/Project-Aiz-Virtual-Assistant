# **Projec Aiz - Virtual Assistant**
![](https://www.cxtoday.com/wp-content/uploads/2019/09/How-Do-Bots-Chatbots-Work.jpg)
![](https://img.shields.io/github/license/huytjuh/Recommender-System-Basket-Analysis) ![](https://img.shields.io/maintenance/no/2021)

Subsequence Time Series (STS) Clustering model for discovering hidden patterns and complex seasonality within univariate time-series datasets by clustering similar groups of time windows based on their structural characteristics with advanced statistics.

Python implementation from scratch inspired by paper [Wang et al. (2006)](https://link.springer.com/content/pdf/10.1007/s10618-005-0039-x.pdf).

***Version: 2.1 (2021)*** 

---

## Introduction
Time-series analysis allows us to predict future values based on historical observed values, but they can only do so to the point where the model is able to differentiate between seasonal fluctuations within the univariate time-series dataset. So far, many papers consider relatively simple seasonal patterns such as weekly and monthly effects. However, higher frequency time-series often exhibit more complicated seasonal patterns. An alternative to using dummy variables, especially for multiple complex seasonal patterns, is to use Fourier terms. Using linear combinations of sine and cosine functions, successive Fourier terms represents the harmonics of the multiple seasonality components, and thus can be added as explanatory regressors to the forecasting models.

While traditional Fourier term analysis is able to capture the pattern of an univariate time-series relatively well, it tends to overestimate for day-of-the-week, monthly, and other known events that are self-evident without requiring extensive analysis. Hence, we suggest residual modified Fourier terms obtained from the residuals of ARIMA, allowing us to redirect our focus on capturing the more complex hidden patterns. On top of that, we propose a Subsequence Time series Clustering framework to enforce the forecasting models to adjust their parameters according to the clustered seasonal time windows, bringing the complex seasonality model to another level. That is, by incorporating advanced statistical operations and defining more complex characteristics of the univariate time-series such as non-linearity, self-similarity, and chaos on top of the decomposed time-series (trend, seasonality, noise), allows us to further refine and improve the forecasting accuracy using a fully data-driven framework.

## Colab Notebook

STS Clustering based on Hierarchical Clustering:<br/>
[Google Colab]() | [Code]()

STS Clustering based on Self-Organizing Maps (SOM):<br/>
[Google Colab]() | [Code]()

## Prerequisites
* Linux or macOS
* python 3.8
* nolds 0.5.2
* pmarima 1.8.4
* bayesian-optimization 1.2.0
* CPU or NVIDIA GPU + CUDA CuDNN

## Getting Started



