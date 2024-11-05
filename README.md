# Apply filters to SQL queries

## Project description

I will demonstrate my ability to obtain specific information about employees, their machines, and the departments they belong to from the database by applying filters to SQL queries.

## Retrieve after-hours failed login attempts

Obtain all unsuccessful login attempts after 18:00.

SELECT \*   
    \-\> FROM log\_in\_attempts  
    \-\> Where login\_time \> '18:00' AND success \= FALSE;

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/failed%20login%20filter.JPG)

## Retrieve login attempts on specific dates

To obtain all login attempts on 2022-05-09 and the day before 2022-05-08.

\> SELECT \*   
    \-\>   
    \-\> FROM log\_in\_attempts   
    \-\>   
    \-\> WHERE login\_date \= '2022-05-08' OR login\_date \= '2022-05-09';

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/login%20attempts%20on%20specific%20dates.JPG)

## Retrieve login attempts outside of Mexico

Pull all logins that did not originate in Mexico.

\> SELECT \*  
    \-\> FROM log\_in\_attempts  
    \-\> Where NOT country LIKE 'MEX%';

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/login%20attempts%20outside%20of%20Mexico.JPG)

## Retrieve employees in Marketing

obtain the information about employees in the 'Marketing' department who are located in all offices in the East building

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where department \= ‘Marketing’ AND office LIKE ‘East%’;

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/employees%20in%20Marketing%20East.JPG)

## Retrieve employees in Finance or Sales

Locate information on the employees in the Finance or the Sales department.

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where department \= ‘Sales’ OR department \= ‘Finance’;    

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/Retrieve%20employees%20in%20Finance%20or%20Sales.JPG)

## Retrieve all employees not in IT

Pull information about employees who are not in that department.

\> SELECT \*  
    \-\> FROM employess  
    \-\> Where NOT department \= ‘Information Technology’;

![](https://github.com/ATG-2539/Apply-filters-to-SQL-Queries/blob/main/Retrieve%20all%20employees%20not%20in%20IT.JPG)

## Summary

I demonstrated the ability to filter through data in a database for practical use cases.  
