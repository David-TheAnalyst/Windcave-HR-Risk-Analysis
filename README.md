# Windcave-HR-Risk-Analysis (2020-2024)


<div align="center">
  <img src="https://github.com/David-TheAnalyst/Windcave-HR-Risk-Analysis/blob/main/Windcave%20Employee%20Metric%20.png" alt="Flowpal Sales Dashboard Additional View" width="1000" height="600">
</div>


## **Introduction:**
 
This analysis shifts the focus from simply reporting HR metrics to decoding Windcave's core talent footprint. The goal was to perform a rigorous, data-driven evaluation of the employee lifecycle, specifically targeting the health of the workforce across three critical dimensions: workforce stability, compensation equity, and future succession potential. The core goal is to transition from observations to quantifiable strategic insights that empower executive leadership to optimize human capital management and mitigate looming structural risks.


Windcave is currently facing a silent stability crisis. Key performance indicators (KPIs) show that Employee Turnover Rate (13%) and overall Average Tenure (2.37 years) are critically out of alignment, falling significantly below industry benchmarks (8-10% turnover and 3-5 years tenure). This misalignment signals a dangerous leakage of institutional knowledge, a failure to retain developed talent, and an elevated operational risk that demands immediate executive attention and corrective action.

The analysis utilized a single, comprehensive Human Resources Log (EEID-level data) capturing employee demographics and career events. The core methodology involved advanced data manipulation and aggregation techniques within Microsoft Excel.

## **Story of Data:**

The dataset was acquired from a publicly available repository on Kaggle, detailing a snapshot of all active and inactive employees spanning from 2020-2024.

The data is structured primarily at the Employee-ID (EEID) level, with each row representing a unique employee's record. Columns are organized to capture the entire employee lifecycle (Hire Date, Exit Date, Status) alongside static attributes (Gender, Department, Job) and dynamic compensation data (Bonus, Annual Salary).

Whilst the analysis relies heavily on the quality of the exit date data for accurate turnover calculation. A known limitation is the absence of quantitative Performance Data which prevents a definitive correlation between bonus allocation and measurable performance.

**Important Features and Their Significance**

-	Dependent Variables (Outcomes): Age, Hire, Exit, Bonus, Status (Active/Inactive). These were crucial for measuring stability, attrition patterns, and financial impact.
-	Independent Variables (Drivers): Department, Gender, and Job. These were used to segment the dependent variables to identify localized issues (e.g., low tenure in Marketing).

## **Data Splitting and Preprocessing:**

I ensured there were no blank rows and duplicate value while cleaning the data. I also saw to it that all date fields (Hire, Exit) were in a consistent date format and each EEID represented a unique employee record for accurate headcount.

All missing Exit dates were assumed to be Active employees and Missing Bonus values were treated as zero or not applicable, requiring conditional formulas to correctly calculate bonus allocation and averages.

Several new variables were created using Excel formulas while transforming:
-	Tenure (in years)
-	Age Group
	 

## **Pre-Analysis:**

This part of the project was focused on capturing the core narrative of the dataset. It gave me a high-level view of the data quality, the industry context, and what success looks like for stakeholders.

**Independent (Categorical):** Age, Hire, Exit, Bonus, Status (Active/Inactive). These were crucial for measuring stability, attrition patterns, and financial impact.

**Dependent (Metrics):** Department, Gender, and Job. These were used to segment the dependent variables to identify localized issues (e.g., low tenure in Marketing).

**Industry Context:** A Large-Scale Corporation / Tech Company industry setting a high benchmark for talent retention (low turnover, high tenure) which also emphasizes the criticality of functional roles.
**Stakeholders:** Key recipients and beneficiaries of the findings include:
-	HR Department: Responsible for policy implementation and target setting (turnover, tenure).
-	Department Heads: Accountable for localized retention issues (Accounting, Marketing).
-	Finance Department: Responsible for managing the bonus pool and compensation equity.
-	Executive Leadership: Responsible for strategic planning and mitigating succession risk.

I then listed every potential analysis/ question I wanted to explore, pairing each with the expected pre-insight and potential insight. 


The insights generated from this report would enable the company to optimize human capital, directly impacting core business goals by reducing replacement costs, improving institutional knowledge retention, and ensuring fair compensation, which drives overall performance and productivity.

## **In-Analysis:**

The in-analysis phase focused on Identifying the key trend In how the company is optimizing its human capital.

-	The 13% turnover rate suggested a systemic issue with retention strategies.

-	The headcount was heavily skewed, with Engineering dominating both active (56%) and inactive (55%) staff, indicating a high concentration and high-risk dependency.
 
-	Tenure Inconsistency: A significant gap existed between the overall average tenure (2.37 years) and the critically low tenure in Accounting (1.50 years) and Marketing (1.55 years).
 
-	The high concentration of employees in the 36–45 age bracket, coupled with underrepresentation in the younger 26–30 group, pointed to a potential succession risk driven by a lack of a structured talent pipeline.
 
-	The disproportionate allocation of the bonus pool to Engineering (55.34%) suggested a strong correlation between department size (rather than strictly performance) and incentive share.
 
These key trends raised critical questions about fairness and sustainability:

-	Is the compensation truly equitable if Sales/Marketing (revenue drivers) receive significantly lower bonus shares than Engineering (cost center)?
-	What are the root causes driving the exceptionally low tenure in non-technical departments like Accounting?


Based on the early findings (high turnover and low tenure), preliminary recommendations were:

1.	Targeted engagement surveys in high-attrition departments.
2.	Review of Q1 hiring/exit data to identify seasonal triggers for high attrition.

## **Post-Analysis and Insights:**

The detailed analysis confirmed the initial observations, solidifying the severity of the human capital risks:

-	The overall 13% turnover rate and 2.37 years average tenure were confirmed to be non-compliant with industry standards (8−10% turnover, 3−5 years tenure).

-	The low tenure in Accounting (1.50 years) and Marketing (1.55 years) was statistically verified, confirming the need for localized interventions.

-	The finding that 55.34% of bonuses went to Engineering, while critical revenue drivers received proportionally less, was confirmed, requiring immediate reform to link incentives to performance KPIs.

-	The observation that younger (26–30) and older (51–60) groups are significantly underrepresented was validated, confirming the imminent succession risk.

-	A notable positive confirmation was the finding of near-perfect gender diversity (49.87% Male, 50.13% Female), which is a strength to be maintained and leveraged. 

-	The seasonal exit peaks in Q1 2021 and Q1 2023 were identified as significant, suggesting a failure point during critical business or compensation cycles.
 

## **Data Visualizations & Charts:**

Below is a centralized HR Metric Dashboard was created, consolidating the Turnover Rate, Average Tenure, Gender Ratio, and a visual representation of the Age Group by Active Employee to provide Executive Leadership with an immediate, high-level overview of workforce health.

 <div align="center">
  <img src="https://github.com/David-TheAnalyst/Windcave-HR-Risk-Analysis/blob/main/Windcave%20Employee%20Metric%20.png" alt="Flowpal Sales Dashboard Additional View" width="1300" height="auto">
</div>

To interact with the live Dashboard, Click [Here](https://github.com/David-TheAnalyst/Windcave-HR-Risk-Analysis/blob/main/Task%2025A%20OjoDavidShola.xlsx)

**Key Metrics Displayed (KPIs):** 
-	Total Employee: 792
-	Active Employee: 691
-	Inactive Employee: 101
-	Average Tenure: 2.37

**Charts and Graphs:**

**Scatter Plot:** 
-	Discount Percentage vs. Profit: This mandatory visualization provides the irrefutable evidence of the 12% "discount cliff" and the negative 83% margin.

**Pie Chart:** 
-	Staffing percentage by Gender

**Line Chart:** 
-	Hiring and Exiting Trend Over Time 

**Column Chart:** 
-	Age Group By Active Employee 
-	Average Tenure (year) By Department 
-	Bonus Allocation By Department

**Bar Chart:**
-	Departmental Staffing Level


## **Actionable Recommendations:**

The findings translate into eight mandatory, actionable recommendations for optimizing Windcave's human capital.

-	Implement structured retention strategies (onboarding, career development, pulse surveys).

-	Create structured career progression and internal mobility programs and conduct pulse surveys in low-tenure departments.

-	Build structured graduate and early-career pipelines, ensuring 20−30% of new hires are early-career talent.

-	Review and restructure the performance incentive system and Introduce transparent KPIs to link rewards to measurable contribution.

-	Reduce concentration risk by diversifying the workforce while building targeted Engineering retention levers and succession plans.

-	Conduct detailed exit interviews to identify root causes of Q1 spikes and align onboarding/engagement initiatives to preemptively improve retention during these critical business cycles


## **Conclusion:**

The analysis confirms that Windcave’s primary challenge lies in workforce stability, evidenced by turnover exceeding benchmarks and critically low tenure in key non-technical departments. While the gender ratio is a significant strength, compensation structures require urgent reform to ensure fairness based on performance and contribution.

However, the analysis was limited by the available data. Specifically, the lack of quantitative, normalized employee performance data prevents the definitive calculation of performance-adjusted bonus equity. 

## **Future Research:**

Future research should focus on:

1.	A deeper dive into salary variances across specific job roles and seniority levels by gender.

2.	Detailed investigation into the causes of low tenure in Accounting/Marketing and the recurring Q1 exit spikes.

3.	Analyzing the number of job title changes to quantify career progression opportunities within different departments.


## **References** 

-	Employee Dataset [(Kaggle)](https://github.com/David-TheAnalyst/Windcave-HR-Risk-Analysis/blob/main/Kaggle%20Employee%20Dataset.xlsx)
-	Microsoft Excel (Analytical Tool)


<h3 align="left">Connect with me on Socials:</h3>
<p align="left">
<a href="https://linkedin.com/in/david ojo" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="david ojo" height="30" width="40" /></a>
<a href="https://twitter.com/david_ojo_1" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="david_ojo_1" height="30" width="40" /></a>
<a href="https://medium.com/@davidojo" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/medium.svg" alt="@davidojo" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/davidojo-j3v" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="davidojo-j3v" height="30" width="40" /></a>
</p>

Thanks for stopping by!

