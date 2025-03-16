# Doctor Complaints Analysis Using Zero-Inflated Modeling in R

## Overview 
This project analyzes patient complaints against doctors using statistical modeling techniques implemented in **R**. The goal is to identify and understand factors that influence patient complaints and situations when complaints are absent. 

Specifically, the analysis focuses on:
- Factors affecting the number of complaints when they occur (count data).

I used a **Zero-Inflated Negative Binomial (ZINB)** approach, ideal for modeling count data with many zeros and substantial variability (overdispersion). This method provides meaningful insights into both complaint frequency and patient satisfaction.

## Features  
✔ **Exploratory Data Analysis** - Clear visualizations (histograms, boxplots, scatterplots) to explore the data.  
✔ **Zero-Inflated Modeling** - Separately modeling the occurrence of zero complaints and the number of complaints when they occur.  
✔ **Interaction Terms** - Identifying nuanced relationships between predictors such as patient visits, doctor’s residency status, working hours, gender, and revenue.  
✔ **Diagnostic Checks** - Residual analysis and rootograms to verify model validity.

## Key Insights and Practical Recommendations
Complaint Drivers:
- Increased patient visits significantly increase complaints.
- Male doctors tend to receive more complaints compared to female doctors.
- Resident and non-resident doctors react differently to changes in working hours.

Practical Recommendations:
- Residents: Ensure adequate supervision during working hours to reduce complaints.
- Experienced Doctors: Limit excessively long hours to avoid increased patient complaints.
- Gender-specific Support: Tailor training and resources considering differences in how male and female doctors respond to workload changes.

This analysis helps healthcare organizations better manage resources, enhance patient satisfaction, and implement targeted support strategies based on clear statistical evidence.

## How to Reproduce the Analysis  
### Step 1: Clone this repository
```bash
git clone https://github.com/your_username/doctor-complaints-analysis-r.git
cd doctor-complaints-analysis-r
```
### Step 2: Install required R packages
install.packages(c("pscl", "AER", "car", "lattice"))

### Step 3: Run the analysis
Open analysis/doctor_complaints_analysis.Rmd in RStudio and click the Knit button to reproduce the analysis and generate the HTML report.


