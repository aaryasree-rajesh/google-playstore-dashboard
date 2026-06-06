# Google Play Store Analytics Dashboard

## Live Dashboard
🔗 [Click here to view live dashboard](https://mybinder.org/v2/gh/aaryasree-rajesh/google-playstore-dashboard/HEAD?urlpath=voila/render/Untitled2.ipynb)

## Overview
Interactive analytics dashboard built on the Google Play Store dataset
with 6 charts, IST time gates, and global filters.

## Dataset
- **Source**: Google Play Store Apps (Kaggle)
- **Link**: https://www.kaggle.com/datasets/lava18/google-play-store-apps
- **Size**: 10,841 apps across 33 categories

## Charts
| Chart | Type | Time Window |
|-------|------|-------------|
| Chart 1 | Grouped Bar — Top 10 categories by installs | 3–5 PM IST |
| Chart 2 | Choropleth Map — Global installs by category | 6–8 PM IST |
| Chart 3 | Dual-Axis — Free vs Paid installs and revenue | 1–2 PM IST |
| Chart 4 | Time Series — Install trends over time | 6–9 PM IST |
| Chart 5 | Bubble Chart — App size vs rating | 5–7 PM IST |
| Chart 6 | Stacked Area — Cumulative installs over time | 4–6 PM IST |

## Transformations Applied
- Cleaned Installs: removed + and , characters
- Parsed Size: converted M and k suffixes to MB
- Cleaned Price: removed $ symbol
- Calculated Revenue: Price x Installs
- Extracted Android Version: regex extraction
- Parsed Last Updated: converted to datetime
- Removed duplicate apps

## KPIs Measured
- Average Rating per category
- Total and Average Installs
- Total Reviews
- Revenue (Free vs Paid)
- Month-over-Month install growth
- Cumulative installs over time

## Tech Stack
- Python 3
- Pandas, NumPy
- Plotly (interactive charts)
- ipywidgets (filters)
- Voila (dashboard deployment)
- Binder (live hosting)

## How to Run Locally
pip install -r requirements.txt
voila dashboard.ipynb

## Screenshots
![Chart 1](screenshots/chart1.png)
![Chart 2](screenshots/chart2.png)
![Chart 3](screenshots/chart3.png)
![Chart 4](screenshots/chart4.png)
![Chart 5](screenshots/chart5.png)
![Chart 6](screenshots/chart6.png)
