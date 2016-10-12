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
9. SELECT COUNT(InvoiceDate) FROM Invoice WHERE DATE(InvoiceDate) LIKE "2009%"
SELECT SUM(Total) FROM Invoice WHERE DATE(InvoiceDate) LIKE "2009%"
SELECT COUNT(InvoiceDate) FROM Invoice WHERE DATE(InvoiceDate) LIKE "2011%"
SELECT SUM(Total) FROM Invoice WHERE DATE(InvoiceDate) LIKE "2011%"
10. SELECT COUNT(Quantity) FROM InvoiceLine WHERE InvoiceLineId = 37
11. SELECT COUNT(InvoiceId), InvoiceId FROM InvoiceLine GROUP BY InvoiceId
12. SELECT Track.Name, InvoiceLine.InvoiceLineId FROM InvoiceLine 
JOIN Track ON InvoiceLine.TrackId = Track.TrackId
GROUP BY InvoiceLine.InvoiceLineId
13. SELECT InvoiceId, Track.Name, Artist.Name FROM InvoiceLine 
JOIN Track ON InvoiceLine.TrackId = Track.TrackId 
JOIN Album ON Track.AlbumId = Album.AlbumId
JOIN Artist ON Album.ArtistId = Artist.ArtistId
14. SELECT Count(*) FROM Invoice
GROUP BY BillingCountry
15. SELECT Playlist.Name, Count(*) Count FROM Track 
JOIN PlaylistTrack ON PlaylistTrack.TrackId = Track.TrackId
JOIN Playlist ON Playlist.PlaylistId = PlaylistTrack.PlaylistId
GROUP BY Playlist.Name
16. SELECT Track.Name, Album.Title, MediaType.Name, Genre.Name FROM Track 
JOIN Album ON Track.AlbumId = Album.AlbumId 
JOIN MediaType ON Track.MediaTypeId = MediaType.MediaTypeId
JOIN Genre ON  Track.GenreId = Genre.GenreId 
17. SELECT InvoiceId, Count(*) Count FROM InvoiceLine 
GROUP By InvoiceId
18. SELECT Employee.FirstName || " " || Employee.LastName AS "Name", SUM(Invoice.Total)AS "Money" FROM Employee
JOIN Customer ON Employee.EmployeeId = Customer.SupportRepId
JOIN Invoice ON Customer.CustomerId = Invoice.CustomerId
JOIN InvoiceLine ON Invoice.InvoiceId = InvoiceLine.InvoiceId
JOIN Track ON InvoiceLine.TrackId = Track.TrackId
JOIN Genre ON Track.GenreId = Genre.GenreId
GROUP BY Employee.EmployeeId
19.
20.
21.
22.
23.
24.
25.
26.
27.
