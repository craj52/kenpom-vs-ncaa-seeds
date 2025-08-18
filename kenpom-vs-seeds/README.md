# KenPom vs NCAA Seeds
Analyzing which better predicts NCAA tournament outcomes: KenPom ratings or NCAA seeds

---

## Overview
This project evaluates whether **KenPom efficiency ratings** or **NCAA tournament seeds** better predict March Madness outcomes.  
The analysis spans **2015–2025**, focusing specifically on games where the two methods disagreed to see which approach more accurately identified the winner.

---

## Data & Methods

### Data Sources
- **KenPom Premium** (team efficiency metrics: AdjEM, seeds, etc.)  
- **NCAA Tournament results** (2015–2025)  

### Cleaning
- Standardized team names across sources with a comprehensive mapping dictionary  
- Applied year-specific naming fixes (e.g., NC State in 2015/2018, McNeese in 2024)  

### Merging
- Linked tournament games with KenPom data  
- Added efficiency ratings (AdjEM) and seeds for both teams in each matchup  

### Predictions
- **KenPom method:** Higher AdjEM wins  
- **Seed method:** Lower (better) NCAA seed wins  

### Evaluation
- Focused only on games where KenPom and seeds disagreed  
- Compared accuracy of both methods in those matchups  

---

## Results (2015–2025)

- **Total games:** 630  
- **Disagreements:** 59 (9.4% of all games)  

### Accuracy when KenPom vs. Seeds disagree
- **KenPom:** 44.1%  
- **Seeds:** 37.3%  

### Accuracy by Confidence (AdjEM gap)
- **Low (0–3):** KenPom 46%, Seeds 40% (N=48)  
- **Medium (3–6):** KenPom 14%, Seeds 43% (N=7)  
- **High (6+):** KenPom 75%, Seeds 0% (N=4)  

---

## Visuals
Bar charts included in the notebook:  
- Accuracy when KenPom vs. Seeds disagree  
- Accuracy by confidence level (AdjEM gap)  

---

## 🏀 Key Takeaway
KenPom provides a **modest overall edge**, and its advantage grows substantially in games where efficiency gaps are larger.  
This suggests that advanced efficiency metrics can add real predictive value beyond traditional NCAA seeding.


