#### Answers

1. SELECT FirstName || "" ||  LastName AS name,country FROM Customer WHERE NOT country = "USA"
2. SELECT FirstName || "" ||  LastName AS name,country FROM Customer WHERE country = "Brazil"
3. SELECT Customer.FirstName || " " || Customer.LastName AS Name, InvoiceDate, BillingCountry, InvoiceId FROM Invoice 
JOIN Customer ON Invoice.CustomerId = Customer.CustomerId
WHERE BillingCountry = "Brazil"
4. SELECT * FROM Employee Where title = "Sales Support Agent"
5. SELECT DISTINCT BillingCountry FROM Invoice
6. SELECT * FROM Invoice 
JOIN Customer ON Invoice.CustomerId = Customer.CustomerId
WHERE BillingCountry = "Brazil"
7. SELECT FirstName || " " || LastName AS Name, Title, InvoiceId FROM Employee 
INNER JOIN Invoice i WHERE Title == "Sales Support Agent" 
8. SELECT Invoice.Total, Customer.FirstName, Customer.Country, Employee.FirstName FROM Invoice 
JOIN Customer ON Invoice.CustomerId = Customer.CustomerId
JOIN Employee ON Customer.SupportRepId = Employee.EmployeeId
9.
10.
11.
12.
13.
14.
15.
16.
17.
18.
19.
20.
21.
22.
23.
24.
25.
26.
27.
