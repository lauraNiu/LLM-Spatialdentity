# Data Repository for "A Large Language Model–Driven Cross-Lingual Framework for Social Media–Based Cross-Boundary Spatial Identity Sensing"

This repository contains the data for the paper: **A Large Language Model–Driven Cross-Lingual Framework for Social Media–Based Cross-Boundary Spatial Identity Sensing**.

## About The Project

This repository provides the datasets used in our study on sensing cross-boundary spatial identity using large language models and social media data. Our framework is designed to analyze and quantify multidimensional spatial identities across different linguistic contexts.

For a detailed explanation of the methodology, framework, and analysis, please refer to our full paper.

- [Link to Paper] (<- Add link to your paper here when available)
- [Link to Project/Code Repository] (<- Add link to your code repository if separate)

## Data Description

The data is organized into two main categories:

1. Scored Multidimensional Spatial Identity Data (/scored_identity_data)

- Description: This dataset contains the final output of our model. Each entry represents a user or a text unit and includes scores for various dimensions of spatial identity (e.g., cognitive, affective, behavioral). This data is processed, cleaned, and ready for quantitative analysis.
- Format: CSV (.csv)
- Key Columns:
  - id: Unique identifier for post.
  - date:
  - space type: 
  - Spatial Imagery: Score for the first dimension.
  - Spatial Satisfaction: Score for the second dimension.
  - Sptial Sense of Belonging: Score for the second dimension.
  - Spatial Identity: Score for the second dimension.
  
2. Raw Data for Attribution Analysis Validation(/raw_attribution_data)

- Description: This dataset contains the raw, anonymized social media posts used for the attribution analysis part of our study. This data is intended to provide context and allow for the replication of our qualitative and attribution findings. Please note that to protect privacy, all personally identifiable information has been removed.
- Format: CSV (.csv)
- Key Fields:
  - post_id: Unique identifier for the post.
  - timestamp: Time of the post.
  - text_content: The raw text of the post.
  - language: 'zh'.

## Repository Structure
`
.
├── scored\_identity\_data/
│   └── scored\_spatial\_identity.csv
│
├── raw\_attribution\_data/
│   └── raw\_social\_media\_posts.json
│
├── README.md
└── LICENSE
`


