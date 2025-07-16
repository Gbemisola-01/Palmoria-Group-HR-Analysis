# Palmoria-Group-HR-Analysis
This project presents a comprehensive HR analytics case study for Palmoria Group, a Nigerian manufacturing company facing critical gender inequality and pay gap challenges. The analysis leverages Power BI to uncover hidden patterns in employee data across regions and departments.

## Objectives
* Investigate gender distribution and identify imbalance across the organization.

* Analyze performance ratings for potential gender bias.

* Detect gender-based salary disparities and assess compliance with the minimum wage regulations.

* Segment employee salaries into bands for detailed pay distribution analysis.

* Calculate bonus allocations based on performance ratings.

* Provide actionable insights and data-driven recommendations to promote workplace equity. 

### Tools used & Skills
Microsoft PowerBI Desktop for interactive dashboards and visualizations

Data Cleaning: Filtering null values, assigning generic gender tags

Power Query Editor for advanced metrics and calculations

HR Analytics for real-world insights on diversity, equity, and compliance



### Steps Taken
![PALMORIA DASHBOARD](https://github.com/user-attachments/assets/67887c8b-f7c8-4712-9118-2017def2f859)


![Table view](https://github.com/user-attachments/assets/5a5d5c70-e4fe-4b86-a3d8-f96f98addeb6)


![Bonus Rule Raw Data](https://github.com/user-attachments/assets/eeaa2630-d6cc-4229-a2aa-be59158973e3)


* Get the First Dataset from Excel (Bonus Rules) and then click on Transform Data.
* On the Power Query Editor, right click on Department and click on Unpivot other Columns.
* Rename the columns: Attribute - Ratings, Values - Bonus %                      



* Get the Second Dataset from Text\CSV (Employee Data) and then load unto the Power Query Editor.
* Click on the drop down on Department and uncheck NULL.
![Department 1](https://github.com/user-attachments/assets/24288c58-1324-4b73-8199-06b16e8cb6ba)
![Department 2](https://github.com/user-attachments/assets/ff9abf83-dd16-420e-a0a6-d68f017b545f)

* Click on Salary drop down and uncheck NULL.
![Salary 1](https://github.com/user-attachments/assets/3626e232-98b0-4bff-9a56-f1a71c9226f2)
![Salary 2](https://github.com/user-attachments/assets/ef803bb7-e51f-44b0-9315-b693ff281932)
![Salary 3](https://github.com/user-attachments/assets/7cf70241-82a8-402b-85ac-544a751ec161)

* Right click on Gender and click on Replace Values to find Blanks and replace with UNKNOWN.
  ![Gender 1](https://github.com/user-attachments/assets/85761fd1-a791-4d2f-9a33-bc4664ce0e19)
![Gender 2](https://github.com/user-attachments/assets/c08e58c8-da11-4a2b-894d-1a3c664d2ec7)


* Merge queries as New together by clicking on similar columns.
* Click on the drop down on the new column created and uncheck Select All, and check the Bonus Rules %
* Right click on the Bonus % column and click Replace Values to find NULL and replace with 0
![Merge 1](https://github.com/user-attachments/assets/32ce6f10-885f-4825-a7e0-2f8004d5ae5a)
![Merge 2](https://github.com/user-attachments/assets/dcfd972e-f570-40fe-977f-50209abb84b7)


* Add Custom Column for Bonus, =([Salary]*[Bonus Rules %])
![Bonus](https://github.com/user-attachments/assets/71cf2c86-caa3-4f5a-a060-98fe20892947)

* Add Custom Column for New Salary, =([Salary]+[Bonus])
![New Salary](https://github.com/user-attachments/assets/2b2df132-26b3-4321-9206-5d1bb209efe7)

* Add Condidtional Column for Salary Band
![Salary Band](https://github.com/user-attachments/assets/5e5ef0a6-e814-4d39-bf62-e1ad5169c4ab)

* Add Conditional Column for Compliance rate with the $90000 Minimum Wage
![Compliance Rate](https://github.com/user-attachments/assets/2efd6a6e-88a6-4d86-8cf7-351614de2b42)

## Outcome
The investigation into gender inequality and pay structure within Palmoria Group revealed critical disparities and compliance concerns. After deep analysis of the HR data provided by the CHRO, the following key outcomes emerged:


1. Gender Distribution Analysis

Overall Gender Distribution

Out of a total of 875 employees, gender was identified as follows:

- Female: 337 (38.5%)

- Male: 312 (35.7%)

- Unknown: 226 (25.8%) – grouped as Undisclosed in this report.

By Region

- Kaduna: Highest female representation (female > male)

- Abuja: Near parity between male and female

- Lagos: More male employees, with a significant portion of undisclosed gender

By Department

Departments such as Research & Development, Procurement, and Accounting show better gender balance, while Training, Marketing, and Legal are more female-dominant. However, departments like Product Management and Engineering have very low female participation.

2. Performance Rating by Gender

Performance ratings were categorized into Very Good, Good, Average, and Poor:

- Males: Received the majority of Very Good and Good ratings

- Females: Received more Average ratings (420 out of total average ratings)

This points to a possible rating bias, where men are more frequently rated higher despite relatively even representation.

3. Salary Structure and Gender Pay Gap Analysis

Average Salary by Gender

- Male: $79.32K (35.09%)

- Female: $72.45K (32.84%)

- Undisclosed: $72.25K (31.96%)

This reveals a clear pay gap, with males earning $6.87K more on average than females.

Average Salary by Department

- Highest Paid: Training ($78K), Business Development ($77K)

- Lowest Paid: Legal ($71K), Product Management ($72K)

Most departments fall below the new regulatory threshold of $90,000.

Average Salary by Location

- Kaduna: $76K

- Lagos: $74K

- Abuja: $72K

Kaduna leads with the highest average salary, yet none of the regions meet the $90K compliance mark.

4. Regulatory Compliance & Salary Band Analysis

Compliance with $90K Regulation

- Compliant Employees: 607 (69.4%)

- Non-Compliant: 268 (30.6%)

The organization does not fully comply with the new regulation requiring all employees to earn a minimum of $90K.

Salary Band Distribution

- A majority of employees fall within the $70K – $80K band.

- Very few are in the $90K – $100K or higher ranges.

This pattern suggests a uniformly low salary structure, potentially creating dissatisfaction among staff.

5. Bonus Allocation Based on Performance Ratings

- Average Bonus: $2.51K

Bonus allocations are performance-linked. Using the given rules (not shown on dashboard), we assigned:

  - Very Good: Highest bonus rate

  - Good: Moderate bonus

  - Average and Poor: Minimal or no bonus

These allocations result in a widening gap when total compensation is considered.

Total Compensation = Base Salary + Bonus

- Males not only earn higher base salaries but also receive higher bonuses due to better performance ratings, exacerbating gender pay inequality.




Key Insights Summary

Insight Area	Finding

Gender Distribution	Female representation is strong but uneven across departments/regions

Performance Ratings	Males dominate higher performance ratings

Salary Comparison	Males earn ~$7K more than females on average

Regulation Compliance	30.6% of employees earn below mandated $90K

Pay Band	Majority fall within $70K–$80K band

Total Compensation	Males benefit disproportionately from bonuses



Recommendations

1. Gender Equality Programs

- Implement internal awareness and mentorship programs to promote female advancement.

- Investigate causes of rating disparities and conduct bias training for managers.



2. Review Performance Appraisal Process

- Revisit appraisal frameworks to ensure fairness and transparency.

- Establish a gender-balanced review committee to evaluate performance objectively.



3. Salary Adjustment Plan

- Develop a phased plan to raise salaries below $90K.

- Introduce salary bands with defined progression criteria.



4. Compliance Enforcement

- Mandate a review of all salaries to ensure full compliance.

- Set quarterly salary compliance targets.



5. Data Transparency

- Encourage employees to update missing gender data.

- Improve HR record-keeping and reporting processes.

Conclusion

Palmoria Group has a dedicated workforce and strong female presence. However, significant gender-based disparities in ratings and compensation could undermine morale and brand reputation if left unaddressed. This report provides management with a roadmap to create a more equitable and compliant workplace.

