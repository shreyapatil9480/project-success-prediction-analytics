# Project Success Prediction Analytics

Which marketing channels deliver positive ROI?

**Stakeholder:** Marketing Director

## Key Insights

- Paid social campaigns with low impression volume rarely break even on ROI.
- Email retains the highest conversion efficiency despite smaller reach.
- Display spend above $8k without A/B testing correlates with negative ROI.

## Dataset

Primary file: `data/campaign_performance.csv`  
Target variable: `roi_positive`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/exploratory_analysis.ipynb
```

## CLI Usage

```bash
python src/train.py
python src/predict.py --input data/sample_input.csv
```

## Next Steps

**Done.** Docker training image and scheduled retraining workflow are implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-10*

<!-- build 7 -->

### Implemented

```bash
pip install -r requirements.txt
docker build -t train . && docker compose run train
```
