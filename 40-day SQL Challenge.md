## 40-day SQL Challenge with [Abiodun Sanni](https://www.linkedin.com/in/abiodun-sanni-emmanuel)

#### DAY ONE
_Given the table below, write a query to return employees that have spent at least 25 years in the company._
_Link to the data can be found_ [_here_](https://lnkd.in/daTBPMrw).
_You can also query the table from_ [_here_](https://lnkd.in/d-BUCy5W).

Data Field: employee_id
            first_name
            last_name
            email
            phone_number
            hire_date
            job_id
            salary
            commission_pct
            manager_id
            department_id
            
SELECT *
FROM Employees
HAVING DATEDIFF(year, GETDATE(), hire_date) >= 25;
            
