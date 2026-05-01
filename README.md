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
  as audit candidates with above network average
- NH-44 (Delhi–Agra) and NH-48 (Delhi–Jaipur) ranked as 
  most efficient stretches in the network

## Visualisations

### Cost vs Traffic Scatter Plot
[Scatter Plot]<img width="1250" height="812" alt="road_efficiency_scatter" src="https://github.com/user-attachments/assets/4cf2438f-b44f-419e-acd5-5685d5108885" />


### Efficiency Index Ranking
[Ranking Chart]<img width="1250" height="875" alt="road_efficiency_ranking" src="https://github.com/user-attachments/assets/141fee58-8da0-4e2c-8389-800c20c806c6" />


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

## Tech Stack
- MATLAB — analysis, visualisation, CSV export
- Statistical method — Z-score outlier detection
- Data source — NHAI / MoRTH public reports

## Author
Ashish Patel | B.Tech Civil Engineering | NIT Raipur
