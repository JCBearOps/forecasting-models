# Forecasting Models

This repository supports both top-down and bottoms-up forecasting for SaaS consumption and revenue.

## Structure

- `top_down/`: Traditional models like SARIMAX and Prophet
- `bottoms_up/`: ML-based, account-level models with BigQuery + GCS
- `utils/`: Shared configuration and secrets loading
- `data/`: Loading/saving data to cloud or local
- `notebooks/`: Exploration and diagnostics

## Usage

1. Copy `.env.example` to `.env`
2. Install dependencies with `pipenv install`
3. Run training pipelines:
   - Top-down: `python src/top_down/sarimax_model.py`
   - Bottoms-up: `python src/bottoms_up/train_model.py`

