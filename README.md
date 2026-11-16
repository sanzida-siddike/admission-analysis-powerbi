# Admission Trends & Decision Analysis

An interactive Power BI dashboard that explores what influences university admission decisions across departments, gender, GPA and test scores.

![Dashboard preview](images/Capture.PNG)

> **Note:** This is a small practice dataset (200 applicants), so the findings are indicative only and should not be treated as statistically conclusive.

---

## Project Overview

The goal of this project is to answer a simple question: **which applicant attributes are linked to getting accepted?**

I built a one-page dashboard with slicers so a user can filter by admission status, department, GPA range and gender, and see all visuals update instantly.

## Key Numbers

| Metric | Value |
|---|---|
| Total applicants | 200 |
| Accepted | 44 |
| Rejected | 156 |
| Overall acceptance rate | 22% |

## Key Insights

1. **Test score is the clearest differentiator.** Accepted applicants average **88.7**, rejected applicants average **74.8**, a gap of about **14 points**. The gap holds in every department.
2. **Acceptance rate varies by department.** CSE is highest (10 of 37, about 27%) and English is lowest (5 of 29, about 17%).
3. **Gender rates are fairly close.** Male: 23 of 95 (about 24%). Female: 21 of 105 (about 20%).
4. **Recommendation strength shows no clear effect.** Acceptance was about 21% (Strong), 22% (Average) and 23% (Weak).
5. **Extracurricular activity does not help in this data.** Acceptance was about 19% with extracurriculars and 25% without.

## Dataset

- **File:** `final_admission_dataset.xlsx` (200 rows, 9 columns)
- **Source:** _Add the source here (e.g. Kaggle link, or "Synthetic dataset created for practice")_

| Column | Description |
|---|---|
| `ID` | Applicant ID |
| `Gender` | Male / Female |
| `GPA` | Grade point average (2.50 to 3.99) |
| `TestScore` | Admission test score |
| `Extracurricular` | Yes / No |
| `Recommendation` | Strong / Average / Weak |
| `Department` | CSE, SWE, EEE, PHARMACY, ENGLISH, BBA |
| `Weight` | Applicant weight (kg) |
| `AdmissionStatus` | Accepted / Rejected |

## Dashboard Contents

- **KPI cards:** total applicants, accepted, rejected, acceptance rate
- **Admission status by department** (clustered bar chart)
- **Overall admission distribution** (donut chart)
- **Department-wise average test score** (accepted vs rejected)
- **Gender-wise admission status** (bar chart)
- **GPA effects on admission status** (decomposition tree)
- **Average test score by GPA and admission status** (line chart)
- **Slicers:** Admission Status, Department, GPA range, Gender

## Tools Used

- Power BI Desktop
- DAX (measures such as acceptance rate)
- Excel (data source)

## How to Use

1. Clone or download this repository.
2. Open `Admission_Dashboard.pbix` in Power BI Desktop.
3. If Power BI asks for the data source, point it to `final_admission_dataset.xlsx`.
4. Use the slicers on the left to filter the dashboard.

## Repository Structure

```
├── README.md
├── final_admission_dataset.xlsx
├── Admission_Dashboard.pbix
└── images/
    └── dashboard.png
```

## Limitations

- Only 200 records, so small differences between groups may be due to chance.
- No statistical tests were applied; insights come from descriptive analysis.
- The dataset may not reflect real admission policies.

## Possible Next Steps

- Add a logistic regression in Python to measure each factor's effect on acceptance.
- Run a t-test on test scores between accepted and rejected groups.
- Publish the dashboard online and add the link here.

## Author

**Sanzida Siddike**
M.Sc. in Software Engineering | Python · SQL · Power BI
GitHub: [sanzida-siddike](https://github.com/sanzida-siddike) · Email: sanzidasiddike138@gmail.com
