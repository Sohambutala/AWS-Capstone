<!-- # AWS-Capstone

## Introduction:

As AWS evaluates new hard drives for S3, synthetic data is key for accurately predicting future traffic patterns. Traditional testing methods often struggle to capture the complexity of future hard drive traffic patterns. Synthetic data offers a solution by approximating these patterns, a comprehensive evaluation for new hard drives' performance.

### Problem Statement:

Synthetic Data Generation based on:
Realism: mirrors the complex patterns of actual S3 traffic
Historical Data Constraints: utilizing parameters like time range, disk volume, container groupings, etc
Generative Model Application: Successfully applying generative models like GANs to produce realistic, synthetic S3 traffic data -->

# Synthetic Data Generation for AWS S3 Traffic Using Generative Models

Team Members: Neel Shah, Soham Butala, Aaditya Parthasarathy, Aditi Kharkwal, Ameya Bhamare

## Overview
This project focuses on generating synthetic data for AWS S3 traffic to evaluate new hard drives' performance accurately. By leveraging the complexity of future traffic patterns through synthetic data, we aim to provide a more comprehensive evaluation compared to traditional testing methods.

## Motivation
The motivation behind this project is the need for accurate prediction of future hard drive traffic patterns on AWS S3. Traditional testing methods often fall short in capturing the complex nature of these patterns. Synthetic data generation offers a promising solution by approximating these patterns, thus enabling a more thorough performance evaluation of new hard drives.

## Problem Statement
The challenge lies in generating synthetic data that mirrors the complexity of actual S3 traffic, adhering to historical data constraints and successfully applying generative models such as GANs (Generative Adversarial Networks) to produce realistic synthetic S3 traffic data.

## Methodology
Our approach involved exploring various data generation methods including:

TabGAN: An evolution of CTGAN for tabular datasets.
PAR: Probabilistic AutoRegressive model for learning multivariate time series data.
TimeGAN: GAN architecture for time series data.
DoppelGANger: Captures the statistical properties of time series data.
CT-GAN: Conditional Tabular Generative Adversarial Network for synthesizing realistic tabular data.

## Data Profile
Rows: 271 million S3 transactional data points.
Columns: 13 (11 categorical, 2 numerical).
Security: One-way hashing enforced.

## Results
The evaluation of different models led to identifying Gaussian Copula and CTGAN as the best performers for this use case. Notably, Gaussian Copula was found to be significantly faster and more efficient than CT-GAN, both in terms of training speed and data quality.

## References
Modeling Tabular Data using Conditional GAN. (NeurIPS 2019)
Tabular GANs for uneven distribution. (arXiv preprint arXiv:2010.00638, 2020)
Using GANs for Sharing Networked Time Series Data: Challenges, Initial Promise, and Open Questions.

## Appendix

### Poster

![AWS_Capstone_Poster_Scubed_Final pptx](https://github.com/Sohambutala/AWS-Capstone/assets/122260079/e207d7cb-f88d-430e-9289-afba26003ef3)

### Final Presentation:

[Presentation Link](./docs/AWS_Capstone_Poster_Scubed_Final.pptx.pdf)
