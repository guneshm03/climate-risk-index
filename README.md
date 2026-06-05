# U.S. Climate Risk & Energy Vulnerability Index

## What is this project?
This project builds a state-level climate risk index for all 50 US states using real government data. The goal is to measure how vulnerable each state is to climate-driven energy disruptions - rising prices, increasing disasters, and temperature stress on the grid.

## Why I built this
This came out of my IST 625 Enterprise Risk Management coursework where I studied climate change as a business risk. I wanted to go beyond the classroom and actually build something with real data that shows the risk quantitatively.

## Data Sources
- EIA - State level electricity prices and consumption (2001-2023)
- FEMA - Climate disaster declarations by state (2001-2023)
- NOAA - Average annual temperature by state (2001-2023)

## Methodology
I built a composite risk score for each state using four variables:
- Disaster count (40%) - most direct evidence of climate risk
- Average temperature (30%) - root cause of climate stress
- Electricity price (20%) - indicator of grid stress
- Energy consumption (10%) - measures state exposure

All variables were normalized to 0-1 scale before scoring.

## Top 5 Highest Risk States
1. Florida - 0.51
2. Texas - 0.50
3. California - 0.47
4. Alaska - 0.46
5. Oklahoma - 0.42

## Tools Used
- Python, pandas, scikit-learn, matplotlib
- Tableau Public
- Git/GitHub

## Project Structure
- notebooks/ - data collection, cleaning, EDA, and risk modeling
- data/raw/ - original downloaded datasets
- data/processed/ - cleaned and merged files
- tableau/ - dashboard workbook