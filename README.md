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
1. Gender Distribution Insights
- Organization-wide: A significant gender imbalance was found, with male employees making up over 70% of the workforce.
- By Region:
  • Region A had the highest concentration of male employees.
  • Region C showed relatively better gender balance.
- By Department:
  • Engineering and Production departments were male-dominated.
  • HR and Customer Support had a more even gender distribution or a female majority.
2. Performance Ratings by Gender
- Male employees were more frequently rated as 'High Performers'.
- A disproportionate number of females were rated as 'Average' or below.
- Potential bias in performance evaluation is suspected.
3. Gender Pay Gap Analysis
- A clear gender pay gap exists across all three regions.
- Male employees consistently earned more than females in the same roles.
- Departments of concern: Engineering, Finance, and Management.
- Region A had the largest overall pay disparity, while Region C had the least.
4. Minimum Salary Compliance
- Regulation requires a minimum salary of $90,000.
- Many employees fall below this benchmark, particularly in Region B.
- Most employees are in the $50,000–$70,000 and $70,000–$90,000 bands.
- Few employees earn above $90,000, indicating a compliance issue.
5. Bonus Allocation & Total Compensation
- Bonuses allocated based on performance ratings.
- High performers received the highest bonuses.
- Total compensation revealed further gender disparity.
- Region A had the highest total payout; Region C had the lowest.


## Key Recommendations
1. Implement Gender Equality Training and review performance appraisal criteria for bias.
2. Revise Compensation Structures to address gender pay gaps and ensure equity.
3. Raise all employee salaries below $90,000 to meet regulatory compliance.
4. Monitor HR Data Continuously using HR analytics dashboards.
5. Develop DEI Policies and set measurable diversity targets.


## Conclusion
My analysis brought clarity to the root causes of the gender inequality crisis at Palmoria. The data-driven insights and visualizations empowered leadership to take concrete, actionable steps toward fairness, equality, and compliance — safeguarding the company’s brand, morale, and international expansion goals.



  



