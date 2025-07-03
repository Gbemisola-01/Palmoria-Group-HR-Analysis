# Palmoria-Group-HR-Analysis

How I cleaned the dataset and work on identifying the gender inequality in the Palmoria Group HR Department.

## THE PROBLEM
The Palmoria Group, a manufacturing company based in Nigeria is embroiled in issues bordering on gender inequality in its 3 regions. Unfortunately, the media recently published in the news with the headline "Palmoria, the Manufacturing Partriarchy". This doesn't look good for the owners of the business based on their ambition to scale the business to other regions and even oversea. Cases like this can only spiral downwards revealingother issues like gender pay gap amongst other possible issues.

## TASK GIVEN
To identify key areas within the business that could spring up issues and address them immediately. As an HR Analytics expert, the company's was analyzed and recommendations for management's attention was given.

## THE PROCESS

### Tools used & Techniques
Microsoft PowerBI Desktop - Used for Data Extraction (ETL), Visual Analysis and Dashboard

Power Query Editor - Used for Advanced Data Cleaning and Calculations


### Steps Taken

![Bonus Rule Raw Data](https://github.com/user-attachments/assets/eeaa2630-d6cc-4229-a2aa-be59158973e3)




* Get the First Dataset from Excel (Bonus Rules) and then click on Transform Data.
* On the Power Query Editor, right click on Department and click on Unpivot other Columns.
* Rename the columns: Attribute - Ratings, Values - Bonus %                      
* Then Load your Data.

  


* Get the Second Dataset from Text\CSV (Employee Data) and then load unto the Power Query Editor.
* Click on the drop down on Department and Salary Columns respectively, and uncheck NULL.
* Right click on Gender and click on Replace Values to find Blanks and replace with UNKNOWN.
  

* Merge Datasets together by clicking on similar columns.
* Click on the drop down on the new column created and uncheck Select All, and check the Bonus Rules %
* Right click on the Bonus % column and click Replace Values to find NULL and replace with 0
  

* Add Custom Column for Bonus, =([Salary]*[Bonus Rules %])
* Add Custom Column for New Salary, =([Salary]+[Bonus])
* Add Condidtional Column for Salary Band


* Then Load Data for Visualization on the Table View (Canvas)


  



