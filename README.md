# HR Attrition Analysis
**Tools:** Microsoft Excel • Power BI | **Type:** Business Analysis Dashboard

## Business Problem
A company with 1,470 employees has an attrition rate of 16.1% - 
above the healthy industry benchmark of 10–15%. HR leadership needs 
to understand which employees are leaving, why they are leaving, and 
which interventions will have the greatest impact on retention.

## Dataset
- Source: [IBM HR Analytics Dataset — Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- 1,470 employee records, 35 variables
- Key fields: Attrition, Department, MonthlyIncome, OverTime, 
  JobSatisfaction, Age, YearsAtCompany

## Data Preparation
- Created calculated columns in Power BI (DAX) for Income Band 
  and Age Band to enable segmentation analysis
- Built Attrition Rate measure using DAX: 
  employees who left ÷ total employees
- Verified attrition counts against raw data for accuracy

## Analysis Approach
Built pivot analysis in Excel then visualised in Power BI 
to answer 5 business questions:
1. Which department has the highest attrition risk?
2. Does overtime correlate with attrition?
3. Is compensation a driver of attrition?
4. Does job satisfaction predict attrition?
5. Which age group is most at risk?

## Key Findings

### Finding 1 - Sales department highest risk
Sales has the highest attrition rate at 20.6% - 1 in 5 Sales 
employees leaves annually. HR (19.0%) is also above company 
average. R&D appears highest in raw numbers but has the lowest 
rate (13.8%) due to its larger headcount.

### Finding 2 - Overtime is the strongest attrition predictor
Employees working overtime leave at 30.5% vs 10.4% for those 
who don't - making overtime employees 3× more likely to leave. 
With 416 employees currently on overtime, this is the single 
highest risk factor in the business.

### Finding 3 - Compensation drives early attrition
Employees earning below $3,000/month have a 28.6% attrition 
rate - more than triple the rate of employees earning above 
$10,000 (8.9%). Lower job levels are disproportionately 
affected.

### Finding 4 - Low satisfaction doubles attrition risk
Employees with low job satisfaction leave at 22.8% vs 11.3% 
for very highly satisfied employees. Notably, even satisfied 
employees show elevated attrition when combined with overtime 
and low income - suggesting retention requires addressing 
multiple factors simultaneously.

### Finding 5 - Youngest employees leaving at nearly 40%
Employees under 25 have a 39.2% attrition rate - more than 
double the company average. Early career employees are leaving 
before the company recoups recruitment and training investment, 
suggesting insufficient career development pathways for 
junior staff.

## Business Recommendations

1. **Audit and reduce overtime immediately** - Identify teams 
   running consistent overtime and redistribute workload or 
   hire additional headcount. Target: reduce overtime workforce 
   from 416 to under 200. Estimated impact: could reduce overall 
   attrition rate by 3–5 percentage points.

2. **Review compensation for below $3K income band** - A targeted 
   salary review for lower job levels would cost significantly 
   less than replacing them. Average replacement cost exceeds 
   6 months salary per employee.

3. **Invest in early career development for under-25s** — 
   Introduce structured career pathways, mentorship programmes, 
   and 6-month progression reviews for junior staff. A 39.2% 
   attrition rate in this group represents both a cost and a 
   lost talent pipeline.

## Dashboard
![HR Attrition Dashboard](dashboard.png)

## Skills Demonstrated
- Data segmentation using calculated columns in DAX (Power BI)
- Attrition rate measure built from scratch using DAX DIVIDE 
  and FILTER functions
- Interactive dashboard with cross-filtering slicers
- Multi-factor analysis connecting department, income, overtime 
  and satisfaction drivers
- Business report writing — translating data findings into 
  costed recommendations for HR leadership
