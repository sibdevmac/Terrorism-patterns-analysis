# Global Terrorism Intelligence Analytics (1970–2020)

## Introduction

Terrorism remains one of the most significant security challenges faced by modern societies. While many studies examine terrorism through political, economic, religious, or social lenses, this project approaches the issue from a data analytics perspective.

The objective of this study is to identify historical patterns of terrorist incidents, evaluate geographical and organizational trends, analyze factors associated with successful attacks, and develop data-driven recommendations for reducing terrorism risk.

## Aim

To develop a comprehensive terrorism intelligence framework that identifies temporal, geographical, organizational, and tactical patterns of terrorist incidents and predicts future terrorism risk using historical data.

## Link
https://www.kaggle.com/datasets/START-UMD/gtd
---

# Objectives

1. How has global terrorism changed over time?
2. Which countries face the highest terrorism burden?
3. Which attack types are most deadly?
4. Which weapons cause the greatest casualties?
5. Are suicide attacks more lethal?
6. Which targets are attacked most frequently?
7. Which terrorist groups are most active and deadliest?
8. Where are global terrorism hotspots?
9. What factors contribute to successful attacks?
10. Which recommendations could lower terrorism risk?

---

# Assumptions

* The analysis is conducted strictly using the dataset.
* Personal, political, religious, and ideological biases are excluded from the analytical process.
* Findings represent historical relationships within the data and should not be interpreted as causal conclusions.
* Terrorism is influenced by numerous geopolitical and social factors that may not be fully captured within the dataset.

---

# Data Preprocessing

The dataset was examined for missing values before analysis.

df.fillna(0, inplace=True)

Preprocessing steps included:

* Handling missing values
* Creating casualty metrics
* Feature engineering
* Geographical aggregation
* Machine learning preparation
* Risk score generation

---

# Analysis

## 1. How Has Global Terrorism Changed Over Time?

The temporal analysis revealed that terrorism existed at relatively low levels during the early years of the dataset but increased substantially during specific geopolitical periods.

### Key Findings

* Significant increase around 1979.
* Historical peak around 1992 with more than 5,000 attacks.
* Decline between 1998 and 2004.
* Rapid growth between 2005 and 2014.
* Global peak around 17,000 incidents during 2014.
* Declining trend after major international counterterrorism campaigns.

### Historical Interpretation

| Period    | Possible Historical Context                                 |
| --------- | ----------------------------------------------------------- |
| 1979      | Iranian Revolution, Soviet-Afghan War, Grand Mosque Seizure |
| 1990s     | Ethnic insurgencies and regional conflicts                  |
| 2001–2004 | Global counterterrorism operations                          |
| 2011–2014 | Arab Spring aftermath and regional instability              |
| Post-2014 | International campaigns against extremist organizations     |

### Insight

The findings suggest that terrorism frequently expands during periods of geopolitical instability, power vacuums, and prolonged conflict.

---

## 2. Which Countries Face the Highest Terrorism Burden?

The analysis identified several countries experiencing disproportionately high terrorism activity.

### Most Affected Countries

* Iraq
* Afghanistan
* Pakistan
* India
* Syria
* Peru
* Sri Lanka

### Insight

Countries experiencing prolonged insurgencies, civil conflicts, and political instability tend to experience significantly higher terrorism burdens.

---

## 3. Which Attack Types Are Most Deadly?

The attack type analysis showed substantial differences in lethality.

### Key Findings

* Hijackings generated the highest average casualties.
* Barricade incidents produced elevated fatality rates.
* Armed assaults remained consistently lethal.
* Bombings were the most frequent attack type but not necessarily the deadliest.

### Insight

Attack frequency and attack lethality are not always correlated.

---

## 4. Which Weapons Cause the Greatest Casualties?

Weapon analysis indicated:

* Explosives are the most frequently used weapons.
* Firearms contribute significantly to global casualties.
* Chemical weapons are extremely rare.

### Insight

Explosives and firearms remain the dominant tools used in terrorist incidents globally.

---

## 5. Are Suicide Attacks More Lethal?

A two-sample t-test was conducted to compare casualties between suicide and non-suicide attacks.

### Results

```text
T-statistic = 11.54
```

### Findings

* Suicide attacks produce significantly higher casualty counts.
* Most incidents still result in relatively low casualty numbers.
* Suicide attacks create a substantially higher average impact.

### Insight

Suicide attacks are associated with significantly greater lethality than non-suicide attacks.

---

## 6. Which Targets Are Attacked Most Frequently?

Target analysis showed that civilians remain the most common victims of terrorism.

### Most Common Targets

1. Private Citizens & Property
2. Military
3. Police
4. Government Institutions
5. Businesses

### Insight

Soft targets continue to be the most vulnerable category globally.

---

## 7. Which Terrorist Groups Are Most Active and Deadliest?

Several organizations appeared repeatedly among the most active groups.

### Major Groups Identified

* Taliban
* ISIL
* Shining Path
* Boko Haram
* New People's Army (NPA)
* Farabundo Martí National Liberation Front (FMLN)

### Insight

Both ideological and separatist organizations contribute significantly to global terrorism patterns.

---

## 8. Where Are Global Terrorism Hotspots?

Geospatial analysis and heatmaps identified major terrorism concentrations.

### Major Hotspots

* Middle East
* South Asia
* Parts of Africa

### Insight

Terrorism is geographically concentrated rather than evenly distributed across the world.

---

## 9. What Factors Contribute to Successful Attacks?

A Random Forest model was used to identify factors associated with successful attacks.

### Important Features

* Attack Type
* Weapon Type
* Target Type
* Region
* Unknown or surprise attack characteristics

### Insight

Successful attacks are strongly associated with tactical decisions, target selection, and regional conditions.

---

## 10. Which Recommendations Could Lower Terrorism Risk?

A scenario-based simulation was conducted using historical data.

### Baseline Risk Score

```text
342,197.40
```

### Scenario Analysis

| Scenario            | Risk Score | Reduction (%) |
| ------------------- | ---------- | ------------- |
| Baseline            | 342,197.40 | 0.00          |
| Reduce Success Rate | 290,867.79 | 15.00         |
| Reduce Casualties   | 274,817.15 | 19.69         |
| Reduce Hotspots     | 281,648.58 | 17.69         |

### Findings

🥇 Reduce Casualties → 19.69%

🥈 Reduce Hotspots → 17.69%

🥉 Reduce Success Rate → 15.00%

### Insight

Reducing casualty severity provides the greatest reduction in overall terrorism risk, followed by hotspot-focused interventions.

---

# Conclusion

This project demonstrates how data analytics can be applied to study terrorism from a historical and intelligence perspective.

Key findings indicate that:

* Terrorism is closely associated with geopolitical instability and regional conflicts.
* Risk is concentrated within specific countries and regions.
* Explosives and firearms remain the most common attack methods.
* Suicide attacks produce significantly greater casualties.
* Civilians remain the most frequent targets.
* Casualty reduction strategies produce the greatest overall reduction in terrorism risk.

The analysis highlights the importance of evidence-based risk assessment and demonstrates how historical data can be used to identify patterns, evaluate vulnerabilities, and support strategic decision-making.

---

# Author

Sibankar Saha
---
