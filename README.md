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
  
* As some employees have multiple titles in our data, to get the latest title of each employee, we use DISTINCT ON in SQL query.

* COUNT() and GROUP BY function is used to find the number of retirement-age employees by there title.


### Mentorship program eligiblity :

* Three different table - employees table, dept_emp table and title table has been joined using JOIN and filtered by BirthDate to get the number of employees who are eligible for mentorship program.

* Below is the SQL code for the query.


##Summary: 

### The number of retiring employees per title :

* Below is the final output data of retiring employees per title -


* From the results, there are 90398 employees comes under silver tsunami list.

* As the list seems to be huge, we can further break down by sorting the retiring employees based on the department and the list can be sent to each department managers and they can decide on next steps.
     * For the Department - Quality Management, we have total of 6136 retiring employees
     * For the Department - Marketing, we have total of 6047 retiring employees
     * This can be repeated for other departments 

### Mentorship program eligiblity :

* Below query used for getting title count of employees eligible for mentorship program.

From this data we can check if the company needs the position to be replaced/promote by current employee or it needs a new recruit.Once they have a replacement for the current employee, they can start the mentorship program.
     

