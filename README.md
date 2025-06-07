# Impact of Central Bank Communications on Inflation

## Overview
This repository contains the research project titled **"Impact of Central Bank Communications on Inflation"**, which investigates the role of central bank forward guidance and tone in influencing inflation dynamics in India. Leveraging Natural Language Processing (NLP) and econometric modeling, the study offers a novel empirical approach to quantifying the impact of the Reserve Bank of India's (RBI) communications on inflation expectations and outcomes.

## Project Structure
- **Data**: A corpus of over 19,000 RBI communications including monetary policy statements, speeches, and press releases for Masked Language Modelling. Over 9K annotated speeches were               used for Supervised finetuning task.
- **NLP Modeling**: Custom sentiment indices were derived using finetuned FinBERT (MLM + SFT)
- **Empirical Framework**: An Extended Hybrid New Keynesian Phillips Curve was used to integrate the sentiment indices.
- **Estimation Technique**: Generalized Method of Moments (GMM) was employed for parameter estimation.

## Key Contributions
- Developed a sentiment-based tone index for RBI communications over two decades.
- Integrated communication sentiment into a Phillips Curve framework to explain inflation behavior.
- Provided evidence that central bank tone has statistically significant effects on inflation.
- Compared the impact of positive vs. negative sentiment across different time horizons.

## Methodology
### 1. Data Collection
- RBI communications from official sources were parsed and cleaned.
- Text preprocessing included sentence segmentation, stop-word removal, and stemming.

### 2. Sentiment Analysis
- **FinBERT**: A transformer-based model pre-trained on financial texts was used to score positive, negative, and neutral sentiment.
- **Loughran-McDonald Dictionary**: Used as a lexicon-based benchmark to validate FinBERT outputs.

### 3. Empirical Modeling
- An extended NKPC was estimated:
  - Output gap, lagged inflation, and forward-looking inflation expectations were included.
  - The tone index served as an exogenous explanatory variable.
- GMM estimation ensured robustness against potential endogeneity.

## Skills & Technologies Used
- Natural Language Processing (NLP)
- FinBERT & Lexicon-based Sentiment Analysis
- Time Series Econometrics
- GMM Estimation
- Python (NLTK, Transformers, Pandas)
- STATA / R for econometric modeling

## Results
- RBI's tone significantly correlates with future inflation.
- Negative sentiment had a stronger short-run effect on inflation expectations.
- Findings support the role of central bank communications as a non-trivial monetary policy tool.

## Applications
- Enhances forecasting models by including communication-based variables.
- Supports central banks in crafting clearer forward guidance.
- Useful for analysts, investors, and policymakers tracking monetary signals.

## How to Cite
```bibtex
@unpublished{centralbank2025,
  title={Impact of Central Bank Communications on Inflation},
  author={Abhirup Guhathakurta},
  year={2025},
  note={Master's Thesis, Indian Institute of Foreign Trade}
}
```

---
For queries or collaborations, please contact: **abhirupguhathakura5@gmail.com**

