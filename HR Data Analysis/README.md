# HR Data Analysis Dashboard

HR Data Analysis Dashboard Documentation

Company Name: Afame Technologies

Project Overview:

This HR Data Analysis Dashboard provides insights into employee attrition, showcasing trends by age, gender, education, salary, and job role. The purpose is to help the HR department better understand attrition patterns, thereby aiding in employee retention and workforce management.

Steps Involved:
1. Data Cleaning:
	Removed Unnecessary Columns: Unrelated columns were removed to streamline the dataset, allowing a focused analysis of factors influencing attrition.
	Corrected Data Types: Ensured all data columns were appropriately formatted (e.g., numerical columns for salary, categorical for departments).

2. Data Transformation:
	Calculated Columns:
  Salary Slab: Categorized salary data into slabs for easy comparison (e.g., Up to 5K, 5K-10K, 10K-15K, 15K+).
  Age Group: Grouped ages into categories (e.g., 18-25, 26-40, 41-50, 51+).

DAX Code Examples:
SalarySlab = IF(Salary <= 5000, "Up to 5K", IF(Salary <= 10000, "5K-10K", IF(Salary <= 15000, "10K-15K", "15K+")))
AgeGroup = IF(Age <= 25, "18-25", IF(Age <= 40, "26-40", IF(Age <= 50, "41-50", "51+")))

3. Slicers/Filters:
Department Slicer: Added a slicer to filter data by department (e.g., Human Resources, R&D, Sales). This enables users to view attrition data specific to each department, facilitating a more detailed analysis.

4. Key Visuals:
- Total Employee: Shows the total number of employees.
- Total Attrition: Displays the count of employees who left the organization.
- Attrition Rate: Percentage of total attrition relative to the overall employee count.
- Average Age: Average age of employees.
- Average Salary: Average salary across the organization.
- Average Year at Company: Average tenure of employees within the organization.

Conclusion:
The HR Data Analysis Dashboard provides critical insights into employee attrition, segmented by demographics and job-related factors. By analyzing data such as attrition by education, salary, and age, the HR department can identify patterns and make informed decisions to reduce turnover. This dashboard supports proactive measures to enhance employee retention and optimize HR strategies.
