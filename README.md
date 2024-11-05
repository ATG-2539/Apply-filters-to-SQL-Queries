# Apply filters to SQL queries

## Project description

I will demonstrate my ability to obtain specific information about employees, their machines, and the departments they belong to from the database by applying filters to SQL queries.

## Retrieve after-hours failed login attempts

Obtain all unsuccessful login attempts after 18:00.

SELECT \*   
    \-\> FROM log\_in\_attempts  
    \-\> Where login\_time \> '18:00' AND success \= FALSE;

**Image goes here**

## Retrieve login attempts on specific dates

To obtain all login attempts on 2022-05-09 and the day before 2022-05-08.

\> SELECT \*   
    \-\>   
    \-\> FROM log\_in\_attempts   
    \-\>   
    \-\> WHERE login\_date \= '2022-05-08' OR login\_date \= '2022-05-09';

**Image goes here**

## Retrieve login attempts outside of Mexico

Pull all logins that did not originate in Mexico.

\> SELECT \*  
    \-\> FROM log\_in\_attempts  
    \-\> Where NOT country LIKE 'MEX%';

**Image goes here**

## Retrieve employees in Marketing

obtain the information about employees in the 'Marketing' department who are located in all offices in the East building

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where department \= ‘Marketing’ AND office LIKE ‘East%’;

**Image goes here**

## Retrieve employees in Finance or Sales

Locate information on the employees in the Finance or the Sales department.

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where department \= ‘Sales’ OR department \= ‘Finance’;    

**Image goes here**

## Retrieve all employees not in IT

Pull information about employees who are not in that department.

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where NOT department \= ‘Information Technology’;

**Image goes here**

## Summary

I demonstrated the ability to filter through data in a database for practical use cases.  
