
Objective : Retrieve a list of all user credentials via SQL Injection.

methodology : 

	Tools used : Burp (Proxy,HTTP history,Repeater)

	1. In the HTTP history, you will find a GET request with "search?q=" in the URL. Copy the entire content of this request

	2. Paste the content into repeater, on top,after the "search?q=" add a this "apple'))UNION%20SELECT%20email,password,3,4,5,6,7,8,9%20FROM%20Users--", this SQL payload forces the database to return all Users Data

	3. Finaly, send the request. UNION is used to add another SQL query, 20% is used to add space. For UNION, it is important to have the same number of columns returned










