Python CA1 Web scraping

The goal is to scrape pay data from salary.com for different roles in various counties throughout Ireland.

The website used for this assignment is https://www.salary.com. BeatifulSoup has been used to parse the HTML content.

The task was carried out in two steps:
i) Extracting information for a single job role in Dublin
ii) Extracting information for multiple job roles across different counties in Ireland. So, for each job role, salary information was extracted across different counties. 21 job roles and six different counties were considered for this activity 

Following data extraction [126 rows and 11 features], the data was analysed and inspected for missing values, data types of the features, unique classes of the categorical features and summary statistics of the numerical features.

The following data-cleaning steps were carried out:
i) Converting the datatypes for the features 'percentile25_salary', 'median_salary' and 'percentile75_salary' from 'object' to 'integer.'
ii) Splitting the 'location' variable into two separate variables, 'county' and 'country.'
iii) Creating a new feature, 'last_reviewed_date' that contains the date part from 'last_reviewed_datetime.'

The clean data was finally uploaded to the MongoDB Atlas server. A new database called 'salary database' and a collection named 'salary' was created. As a last check, the data from the MongoDB server was imported back into the Python environment, and an additional feature, 'id', was discovered.

