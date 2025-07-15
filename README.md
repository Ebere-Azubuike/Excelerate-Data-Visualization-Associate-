# Excelerate-Data-Visualization-Associate- Project
This project gives a detailed analysis of every user that has ever registered on the Excelerate internship portal. 

# Project Objectives
The goal is to help Excelerate make decisions on how to structure their internship opportunities based on users that sign in into their platfrom.

# Data Sourcing/Description
Two datasets were provided by Excelerate platform which were used for this analysis and they included:
1. User data - shows list of users who has ever created an account for internship on Excelerate platform
2. Opportunity wise data - shows every user who signed up on Excelerate platform 

# Data Cleaning/Transformation
This included a comprehensive overview of data preprocessing techniques essential for data analysis such as data cleaning, normalization and handling null values which were done using Microsoft Excel, with further transformations using Python for data feature engineering and one-hot encoding.


A. Data cleaning involved correcting errors, handling missing values, and removing duplicates. ​
Data integration combined datasets from various sources, addressing format and structure differences. ​
User data consists of 27,563 rows with 8 columns, detailing user demographics and signup information. ​
Opportunity-wise data which initially had 20323 rows, reduced to 11482 after removing duplicates based on profile ID. ​

B. Handling Outliers and Anomalies
Identifying and managing outliers is crucial for maintaining data integrity and ensuring accurate analysis. ​

Outliers in the rewards amount column were identified using the Interquartile Range (IQR) method.
Values below Q1 - 1.5IQR and above Q3 + 1.5IQR were flagged as outliers.
Majority of reward amounts were null, with values ranging from $0 to $2500. ​
<img width="827" height="676" alt="image" src="https://github.com/user-attachments/assets/ea718697-6eb8-4905-9de4-6015cc0b0082" /> <img width="786" height="636" alt="image" src="https://github.com/user-attachments/assets/68ac53c9-ea02-4059-ab6c-b5a955ba5a44" />


C. Normalization and Scaling of Features
Normalizing and scaling features ensures consistency and improves model performance. ​

Null values in the gender column were filled with the modal value "male." ​
Rows with null entries in "Current student status" were removed to maintain data quality. ​
Reward amounts and skill points were normalized and standardized for analysis.
<img width="1087" height="656" alt="image" src="https://github.com/user-attachments/assets/34e8ffb9-aedd-4246-82c5-4155d1ff47c4" />
<img width="1086" height="660" alt="image" src="https://github.com/user-attachments/assets/feff1185-f721-4952-b61a-8143b00843bc" />
<img width="1088" height="655" alt="image" src="https://github.com/user-attachments/assets/6c33bf5f-dc6f-4aca-a337-4fdb587d8fbf" />
<img width="1094" height="656" alt="image" src="https://github.com/user-attachments/assets/438b8d9a-1566-459d-8424-6db27edc6e29" />

Null values in user data were addressed by filling or removing entries as necessary. ​
Opportunity-wise data had null entries filled with modal values based on completed opportunities. ​
Categorical types with no completed status were assigned zero for skill points and rewards. ​

D. Feature Engineering for Enhanced Analysis
Feature engineering introduces new variables to improve dataset insights and model performance. ​
<img width="1112" height="840" alt="image" src="https://github.com/user-attachments/assets/d4ac1206-cc84-400b-90a8-7e5f9a8d85b5" />

Columns for opportunity name, skill points, and reward amounts were highlighted for analysis. ​
Unique opportunity occurrences were counted, and averages for skill points and rewards were calculated. ​
Ratios of reward to skill points were derived for further analysis. ​

E. One-Hot Encoding for Categorical Variables
One-hot encoding transforms categorical variables into a binary format suitable for analysis. ​
One-hot encoding was performed for the "Gender" column, creating separate columns for "Male" and "Female." 
<img width="972" height="862" alt="image" src="https://github.com/user-attachments/assets/288eb889-83c4-46b7-98cc-b6634e40f080" />

# Comparative Analysis of User Demographics
Comparative analysis reveals demographic differences and trends among user groups. ​

<img width="1065" height="617" alt="image" src="https://github.com/user-attachments/assets/8a2ac80c-3072-4fdf-9755-71ae4a4dd480" />
The user base spans 170 countries, with India, Nigeria, USA, Pakistan, and Ghana having the highest frequencies.



<img width="1063" height="661" alt="image" src="https://github.com/user-attachments/assets/9b062ee2-8828-43be-9607-5e3a6323d783" />
Graduate program students had the highest completion rates for opportunities. ​




<img width="1085" height="625" alt="image" src="https://github.com/user-attachments/assets/99463feb-dae3-448a-bce1-ffd172817235" />
Internship opportunities were the most preferred, with 7,966 entries recorded.

# Data Visualization and Presentation
The summary of findings where later visualized on Google Looker Studio and presentations were summarized on powerpoint slides
