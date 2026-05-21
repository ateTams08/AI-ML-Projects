# Voting Bloc Analysis: Market Basket Analysis on 2022 PH Senatorial Elections

**Course:** Artificial Intelligence | University of Santo Tomas
**Authors:** Geronimo • Gianan • Oyales • Villanueva | 2DSA2

---

## Overview

Applied Market Basket Analysis (MBA) and Association Rule Mining to the 
2022 Philippine Senatorial Elections dataset. Instead of grocery items, 
each province is treated as a transaction and the top 8 senatorial 
candidates per province as items — revealing which senators were 
consistently voted together across the Philippines.

## Dataset

- **Source:** 2022 Philippine National and Local Elections (Figshare, CC BY 4.0)
- **Size:** 105,971 precinct-level records → aggregated to 90 province-level transactions
- **Candidates covered:** 64 senatorial candidates

## Key Findings

### Strongest Pairs (2-itemsets by support)
| Senator Pair | Support | Meaning |
|---|---|---|
| Legarda + Tulfo | 93.3% | Appeared together in 93% of provinces |
| Legarda + Padilla | 91.1% | Appeared together in 91.1% of provinces |
| Padilla + Tulfo | 88.9% | Appeared together in 88.9% of provinces |

### Strongest Trio
- **Legarda + Padilla + Tulfo** appeared together in **86.7% of provinces**

### Association Rules
- Provinces voting for Padilla + Villanueva + Legarda + Tulfo had an 
  **80% probability** of also voting for Escudero + Gatchalian (lift: 1.71)
- Strongest individual association: **Villanueva → Escudero** (lift: 1.53)

### Political Insight
Results closely mirror the **UniTeam coalition** (BBM-Sara Duterte slate) 
from the 2022 elections — candidates from the same political alliance 
consistently appeared together across provinces, confirming data-driven 
evidence of coordinated voter behavior.

## Tools

`Python` `pandas` `mlxtend` `matplotlib` `seaborn` `Apriori algorithm`
