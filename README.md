*Ironhack Data Science & Machine Learning Bootcamp – Final Project**
# AI-Powered-High-Growth-Stock-Selector-Advisor
A data-driven framework to identify and rank stocks with historically high multi-year growth potential,  while quantifying risk — applied to a hypothetical $30–50k investment scenario.  
This is for educational purposes only and not investment advice.
# 🚀 AI-Powered High-Growth Stock Selector & Advisor



##  Project Overview

This project was born from a **personal goal**: exploring how data science and generative AI can help evaluate high-risk, high-reward investment opportunities. Specifically, I wanted to understand how one might approach investing a **$30,000–50,000 bank loan** into stocks with the potential to deliver **3–4x returns over 4–5 years**.

Instead of making random stock picks, I built an **end-to-end data-driven framework** that:
- Collects historical prices and fundamental data for hundreds of stocks
- Analyzes what characteristics past "moonshot" stocks had in common
- Trains machine learning models to rank stocks by growth potential and risk
- Integrates a **Generative AI chatbot** to answer natural language questions about recommendations and risks
- Provides an interactive prototype for exploring opportunities

> **⚠️ Important Disclaimer**  
> This is an **educational demonstration project only**. It is **NOT financial advice**. Past performance does **not** guarantee future results. Investing — especially with borrowed (leveraged) money — carries a **high risk of losing capital**, including total loss. Always consult a licensed financial advisor before making any investment decisions. Do not use this project to make real trading decisions.

## Business Problem & Objectives

Many retail investors dream of finding the next big winner but lack systematic, transparent tools. This project demonstrates how data science and Generative AI can support more informed decision-making while clearly highlighting risks and limitations.

**Main Objectives:**
- Build a reproducible pipeline for stock analysis and high-growth prediction
- Understand which fundamentals historically correlate with extreme multi-year returns
- Combine traditional ML with modern Generative AI (RAG)
- Create a usable interactive application

## Dataset

- **Primary Source**: `yfinance` (Yahoo Finance)
- **Number of stocks**: ~400 US-listed stocks (S&P 500 + focused high-growth tickers in tech, AI, semiconductors, and biotech)
- **Time range**: 2015 – present
- **Data types**:
  - Daily historical prices (Open, High, Low, Close, Volume)
  - Company fundamentals (revenue growth, EPS growth, PE ratios, PEG, ROE, debt/equity, market cap, sector, industry, etc.)
- **Target variable**: 5-year historical returns (used to label stocks that achieved 3x+ growth)

All collected data is stored in the `data/` folder (raw and processed versions).

## 🛠️ Project Structure

```bash
AI-High-Growth-Stock-Advisor/
├── data/
│   ├── raw/               # Raw downloads from yfinance
│   └── processed/         # Cleaned and feature-engineered data
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_genai_integration.ipynb
├── src/                   # Reusable Python functions
├── app/                   # Streamlit web application
├── models/                # Saved trained models
├── visualizations/        # Plots exported for Tableau
├── requirements.txt
├── README.md
└── presentation/          # Final presentation slides
