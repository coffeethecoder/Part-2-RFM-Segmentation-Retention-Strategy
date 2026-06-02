# Part 2: RFM Segmentation & Retention Strategy

This repo builds RFM from pre-snapshot orders only and enriches it with support, web, abandoned cart, campaign cost, and manual priority signals.

## Segments
Champions, Loyal but at risk, Discount hunters, Support-stressed, Dormant, and Maintain.

## Run
```bash
pip install -r requirements.txt
jupyter notebook rfm_segmentation.ipynb
```

Set `DATA_DIR` in the notebook to your dataset package folder.
