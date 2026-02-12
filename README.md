# Hybrid-Recommender-System
A hybrid recommendation system combining collaborative filtering, content-based filtering, and popularity models. User interaction data feeds into the collaborative model (ALS Alternative Least Square), product metadata is used for content-based similarity, and popularity acts as a fall back. 

## Overview
This project implements a production-grade Hybrid Recommendation System combining:
- Collaborative Filtering (ALS)
- Content-Based Filtering (TF-IDF)
- Popularity-Based Ranking

## Features
- Cold-start handling
- Scalable architecture
- REST API deployment
- Offline & online evaluation

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn, Implicit
- FastAPI
- Docker
- Redis
- Airflow

## Run Locally
```bash
pip install -r requirements.txt
python pipelines/train_pipeline.py
uvicorn src.api.app:app --reload
