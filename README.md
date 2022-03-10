# Pewlett-Hackard-Analysis_new

## Overview of the analysis:
The analysis is for Pewlett Hackard - a large company boasting several employees, as they have several employees retiring in near future, so the below two new analysis is done for future-proofing the company -

* The number of retiring employees per title - By determining the number of employee titles, the company can soon open the position and start recruiting based on the position titles.

* Employees who are eligible to participate in a mentorship program - By calculating the eligibility, we can start the knowledge transfer to the next employee/new recruit to retain vital knowledge that employee has learned over the course of their careers.


## Results: 

### The number of retiring employees per title :

Below are the steps performed to find number of retirement-age employees per title

* First we will get the number of retirement-age employees by filtering the data by Birthdate of employees who were born between 1952 and 1955.
  Below is the SQL code to retrieve the data -
  
  ![1](https://user-images.githubusercontent.com/92698873/157734254-19d029fd-c4e9-4543-8eeb-efc9820d5c71.png)
  
* As some employees have multiple titles in our data, to get the latest title of each employee, we use DISTINCT ON in SQL query.

![2](https://user-images.githubusercontent.com/92698873/157734339-e1bda52f-7998-4a46-a296-e65da79a9867.png)

* COUNT() and GROUP BY function is used to find the number of retirement-age employees by there title.

![3](https://user-images.githubusercontent.com/92698873/157734386-8ce9e353-f020-4bd3-bb96-2da7c47bd34a.png)

### Mentorship program eligiblity :

* Three different table - employees table, dept_emp table and title table has been joined using JOIN and filtered by BirthDate to get the number of employees who are eligible for mentorship program.

* Below is the SQL code for the query.

![d2](https://user-images.githubusercontent.com/92698873/157734844-16af2ba3-4974-4534-9ac0-3c971443674c.png)

##Summary: 

### The number of retiring employees per title :

* Below is the final output data of retiring employees per title -

![d2_1](https://user-images.githubusercontent.com/92698873/157768950-71baab59-e870-4f09-92e7-ec1110f01df5.png)

* From the results, there are 72,458 employees comes under silver tsunami list.


* As the list seems to be huge, we can further break down by sorting the retiring employees based on the department and the list can be sent to each department managers and they can decide on next steps.
     * For the Department - Quality Management, we have total of 4865 retiring employees

![qualitymanaq](https://user-images.githubusercontent.com/92698873/157769153-fb3db22a-15d0-4141-bef2-7f8820d4d6ef.png)

![qualitymanaqcount](https://user-images.githubusercontent.com/92698873/157769283-71de9f95-9371-4814-b0c0-ccc556fc56a4.png)

     * This can be repeated for other departments 

![Department list](https://user-images.githubusercontent.com/92698873/157735139-08462ce5-c6ad-4e66-a189-d28a6e879c06.png)

### Mentorship program eligiblity :

* Below query used for getting title count of employees eligible for mentorship program.

![Screenshot 2021-12-11 210430](https://user-images.githubusercontent.com/92698873/157769439-170fa117-ce5c-461f-99a8-d630bedd7cc8.png)
![D3_1](https://user-images.githubusercontent.com/92698873/157769488-b19c087b-88be-4f1e-81ee-64c549727211.png)


From this data we can check if the company needs the position to be replaced/promote by current employee or it needs a new recruit.Once they have a replacement for the current employee, they can start the mentorship program.
     

