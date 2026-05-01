# Road-Network-Efficiency-Index
Scoring NH stretches on Cost Efficiency Ratio using NHAI/MoRTH data — MATLAB
# Road Network Efficiency Index

Scoring 20 National Highway stretches on Cost Efficiency Ratio (CER)  
using NHAI Annual Report and MoRTH Road Transport Yearbook 2022-23.

## Problem Statement
India's highway investment decisions often lack a standardised 
efficiency metric. This project builds a Cost Efficiency Ratio (CER) 
to identify underperforming stretches and recommend audit targets.

## Methodology

Cost Efficiency Ratio (CER)
CER = Construction + Maintenance Cost (₹Cr/km) ÷ Traffic (thousand PCU/day)

Higher CER = more spend per unit of traffic = poor ROI

Efficiency Index
Normalises both cost and traffic to 0–100 and computes:
Efficiency Index = Traffic Score − Cost Score + 100

Outlier Detection
Z-score on CER with threshold > 1.2 flags audit candidates.

## Key Findings

- Analysed 20 NH stretches across 6 zones (North, South, East, 
  West, Central, NE)
- NH-54 (Aizawl–Jiribam) and NH-52 (Imphal–Moreh) flagged 
  as audit candidates with CER 5.4× above network average
- NH-44 (Delhi–Agra) and NH-48 (Delhi–Jaipur) ranked as 
  most efficient stretches in the network

## Visualisations

### Cost vs Traffic Scatter Plot
[Scatter Plot](road_efficiency_scatter.png)

### Efficiency Index Ranking
[Ranking Chart](road_efficiency_ranking.png)

## Policy Recommendation

1. Commission independent cost audit for NE corridor (NH-52, NH-54)
2. Defer capacity upgrades until traffic exceeds 20,000 PCU/day
3. Benchmark future projects against NH-44/NH-48 corridor 
   (lowest CER in the network)

## Data Sources

| Data | Source |

| NH construction cost per km | NHAI Annual Report 2022-23 |
| Traffic volume (PCU/day) | MoRTH Road Transport Yearbook 2022 |
| Highway length & state | data.gov.in |

> Note: Dataset uses synthetic values calibrated to NHAI/MoRTH 
> published ranges for portfolio demonstration purposes.

## Tech Stack
- MATLAB — analysis, visualisation, CSV export
- Statistical method — Z-score outlier detection
- Data source — NHAI / MoRTH public reports

## Author
Ashish Patel | B.Tech Civil Engineering | NIT Raipur
