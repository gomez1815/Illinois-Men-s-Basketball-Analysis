# 🏀 Illinois Men’s Basketball Analytics (2024–25)

### Author: Taketo Horigome  

---

## 📌 Project Overview

This project provides a data-driven approach to improve Illinois Men’s Basketball performance by:

- 📊 Recommending the most effective 5-man lineups based on advanced metrics
- 👑 Identifying the team’s MVP using a custom efficiency-weighted scoring model
- 🧠 Clustering opponents by style of play and suggesting tailored lineup strategies

By leveraging publicly available stats from BartTorvik, this tool helps coaches and GMs make smarter rotation, scouting, and player development decisions.

---

## 📚 Data Sources

All data was sourced from [BartTorvik.com](https://barttorvik.com/) for the 2024–25 NCAA season, including:

- Illinois player season averages (ORTG, BPM, Usage%, shooting%)
- Team lineup performance metrics
- Opponent efficiency statistics (Adj ORtg, Adj DRtg, TO%, etc.)

---

## 🧠 Methodology

### 🔹 1. Lineup Optimization
Calculated composite scores for all 5-man lineups using normalized metrics:  
`Avg_ORTG`, `BPM`, `AST`, `3P%`, `2P%`, `TO%`, `Usage%`  
→ Visualized top-performing lineups via heatmaps, radar charts, and bar graphs.

### 🔹 2. MVP Model
Built a custom metric using:
- Offensive Rating (ORtg)
- Box Plus-Minus (BPM)
- Usage Rate (USG%)

→ Identified **Tomislav** as the team’s most impactful player, followed by **Morez** and **Kylan**.

### 🔹 3. Opponent Clustering
Used K-Means clustering (K=3) on opponent stats to group them into:
- Cluster 0 – High Offense
- Cluster 1 – High Defense
- Cluster 2 – Weak Defense

→ Calculated Illinois’s win rate by cluster and recommended best lineup per opponent type.

---

## 💡 Key Insights

- ✅ **Top lineup**: Tomislav, Will, Tre, Morez, Ben (highest offensive synergy and lowest TO%)
- 👑 **MVP**: Tomislav dominated in BPM and usage efficiency
- 🎯 **Opponent prep**: 100% win rate vs weak defenses; lower performance vs high-defense teams
- 📋 **Game-ready recommendations**: Suggested optimal lineup based on opponent cluster

---

## 🔧 Tools Used

- **Python** (Jupyter Notebook)
- `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `plotly`


---

## 📬 Contact

Taketo Horigome  
University of Colorado Boulder | Statistics & Data Science  
📧 liverdom@icloud.com
📎 https://www.linkedin.com/in/taketo-horigome-29b26532b/

---
