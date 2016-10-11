#### Answers

1. SELECT FirstName || "" ||  LastName AS name,country FROM Customer WHERE NOT country = "USA"
2. SELECT FirstName || "" ||  LastName AS name,country FROM Customer WHERE country = "Brazil"
3. SELECT Customer.FirstName || " " || Customer.LastName AS Name, InvoiceDate, BillingCountry, InvoiceId FROM Invoice 
JOIN Customer ON Invoice.CustomerId = Customer.CustomerId
WHERE BillingCountry = "Brazil"

4.
5.
6.
7.
8.
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
