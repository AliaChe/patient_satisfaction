# Patient Satisfaction Analysis

## Project Overview

This project analyzes patient satisfaction data collected from different hospital services to identify the key factors that influence overall patient satisfaction.

Using exploratory data analysis (EDA) and visualization techniques, the study investigates the impact of:

- Waiting time
- Communication quality with medical staff
- Pain management effectiveness
- Hospital service department

The objective is to provide actionable insights that can help healthcare institutions improve patient experience and satisfaction.

---

## Repository Structure

```text
patient_satisfaction/
│
├── data/
│   └── patient_satisfaction_dataset.csv
│
├── notebook/
│   └── patient_satisfaction_analysis.ipynb
│
├── requirements.txt
│
└── README.md
```

---

## Dataset Description

The dataset contains patient feedback collected after hospital visits.

### Features

| Column | Description |
|----------|-------------|
| patient_id | Unique patient identifier |
| age | Patient age |
| sex | Patient gender |
| service | Hospital department visited |
| wait_time_minutes | Waiting time before consultation (minutes) |
| communication_score | Communication quality score (1–10) |
| pain_management_score | Pain management score (1–10) |
| overall_satisfaction | Overall satisfaction score (1–10) |

### Score Interpretation

| Score | Meaning |
|---------|---------|
| 1 | Very poor |
| 10 | Excellent |

---

## Objectives

The analysis aims to answer the following questions:

1. How is patient satisfaction distributed?
2. Does waiting time affect satisfaction?
3. How important is communication quality?
4. How does pain management influence satisfaction?
5. Are some hospital services rated better than others?
6. Which factors show the strongest correlation with patient satisfaction?

---

## Technologies Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Installation

Clone the repository:

```bash
git clone https://github.com/AliaChe/patient_satisfaction.git

cd patient_satisfaction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebook/patient_satisfaction_analysis.ipynb
```

---

## Exploratory Data Analysis

The notebook includes:

### 1. Satisfaction Distribution

Histogram of overall satisfaction scores.

Main observation:

- Most patients provided medium satisfaction ratings around 6.
- Extremely low and extremely high ratings are relatively rare.

---

### 2. Waiting Time Analysis

Distribution of patient waiting times.

Main observation:

- Most patients waited less than 20 minutes.
- A small number experienced very long waits (>200 minutes).
- Waiting times are strongly right-skewed.

---

### 3. Pain Management Analysis

Distribution of pain management scores.

Main observation:

- Scores are distributed across the full rating range.
- No strong concentration around a specific value.

---

### 4. Satisfaction vs Key Factors

Relationships between:

- Communication score and satisfaction
- Waiting time and satisfaction
- Pain management and satisfaction

Main findings:

- Better communication is associated with higher satisfaction.
- Better pain management is associated with higher satisfaction.
- Longer waiting times are associated with lower satisfaction.

---

### 5. Service-Level Satisfaction

Boxplot comparison of satisfaction scores across hospital services.

Main findings:

- Surgery receives the highest satisfaction ratings.
- Pediatrics shows the lowest variability in patient experience.
- Internal Medicine ratings are generally concentrated between 5 and 7.

---

### 6. Correlation Analysis

Correlation heatmap between numerical variables.

Variables analyzed:

- wait_time_minutes
- communication_score
- pain_management_score
- overall_satisfaction

Main findings:

- Negative correlation between waiting time and satisfaction.
- Positive correlation between communication quality and satisfaction.
- Positive correlation between pain management and satisfaction.

---

## Key Insights

### Communication Quality Matters

Communication with healthcare professionals is one of the strongest drivers of patient satisfaction.

Potential improvements:

- Communication training programs
- Clear explanations of treatments and procedures
- Increased patient engagement

### Efficient Pain Management Improves Experience

Patients reporting better pain management consistently report higher satisfaction levels.

Potential improvements:

- Standardized pain assessment protocols
- Faster response to pain-related concerns
- Regular follow-up evaluations

### Long Waiting Times Reduce Satisfaction

Extended waiting periods are associated with lower satisfaction scores.

Potential improvements:

- Appointment scheduling optimization
- Better patient flow management
- Real-time waiting time communication

### Consistency Across Services

Pediatrics demonstrates highly consistent patient experiences, while other services show greater variability.

Potential improvements:

- Identify best practices from consistently performing departments
- Share successful workflows across services

---

## Future Work

Potential extensions of the project include:

- Predictive modeling of patient satisfaction
- Regression analysis to quantify factor importance
- Patient segmentation by demographics
- Service-specific satisfaction prediction
- Dashboard creation using Power BI or Tableau
- Statistical significance testing

---

## Example Visualizations

The notebook generates:

- Histograms
- Scatter plots
- Line plots
- Boxplots
- Correlation heatmaps

These visualizations help identify trends and relationships affecting patient satisfaction.

---

## Conclusion

The analysis highlights three major determinants of patient satisfaction:

1. Communication quality
2. Pain management effectiveness
3. Waiting time duration

Improving communication practices and reducing waiting times represent the most impactful opportunities for enhancing patient experience across hospital services.

---
